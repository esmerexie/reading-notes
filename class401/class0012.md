# Readings

## [Spring guide: Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)

First step is to initialize with spring and in the dependencies we need to add SPRING DATA JPA and H2 DATABASE.

### Define an entitity

```java

package com.example.accessingdatajpa;

import javax.persistence.Entity;
import javax.persistence.GeneratedValue;
import javax.persistence.GenerationType;
import javax.persistence.Id;

@Entity
public class Customer {

  @Id
  @GeneratedValue(strategy=GenerationType.AUTO)
  private Long id;
  private String firstName;
  private String lastName;

  protected Customer() {}

  public Customer(String firstName, String lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
  }

  @Override
  public String toString() {
    return String.format(
        "Customer[id=%d, firstName='%s', lastName='%s']",
        id, firstName, lastName);
  }

  public Long getId() {
    return id;
  }

  public String getFirstName() {
    return firstName;
  }

  public String getLastName() {
    return lastName;
  }
}

```

## Create a simple queries

```java

package com.example.accessingdatajpa;

import java.util.List;

import org.springframework.data.repository.CrudRepository;

public interface CustomerRepository extends CrudRepository<Customer, Long> {

  List<Customer> findByLastName(String lastName);

  Customer findById(long id);
}

```

## Create an application class

```java

package com.example.accessingdatajpa;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class AccessingDataJpaApplication {

  public static void main(String[] args) {
    SpringApplication.run(AccessingDataJpaApplication.class, args);
  }

}


-----------------------------------------------------------------------
package com.example.accessingdatajpa;

import org.slf4j.Logger;
import org.slf4j.LoggerFactory;
import org.springframework.boot.CommandLineRunner;
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.context.annotation.Bean;

@SpringBootApplication
public class AccessingDataJpaApplication {

  private static final Logger log = LoggerFactory.getLogger(AccessingDataJpaApplication.class);

  public static void main(String[] args) {
    SpringApplication.run(AccessingDataJpaApplication.class);
  }

  @Bean
  public CommandLineRunner demo(CustomerRepository repository) {
    return (args) -> {
      // save a few customers
      repository.save(new Customer("Jack", "Bauer"));
      repository.save(new Customer("Chloe", "O'Brian"));
      repository.save(new Customer("Kim", "Bauer"));
      repository.save(new Customer("David", "Palmer"));
      repository.save(new Customer("Michelle", "Dessler"));

      // fetch all customers
      log.info("Customers found with findAll():");
      log.info("-------------------------------");
      for (Customer customer : repository.findAll()) {
        log.info(customer.toString());
      }
      log.info("");

      // fetch an individual customer by ID
      Customer customer = repository.findById(1L);
      log.info("Customer found with findById(1L):");
      log.info("--------------------------------");
      log.info(customer.toString());
      log.info("");

      // fetch customers by last name
      log.info("Customer found with findByLastName('Bauer'):");
      log.info("--------------------------------------------");
      repository.findByLastName("Bauer").forEach(bauer -> {
        log.info(bauer.toString());
      });
      // for (Customer bauer : repository.findByLastName("Bauer")) {
      //  log.info(bauer.toString());
      // }
      log.info("");
    };
  }

}
```

## Build an executable JAR

run the application
> ./gradlew bootRun

build the file file
>./gradlew build

run the JAR file
> java -jar build/libs/gs-accessing-data-jpa-0.1.0.jar

## [Baeldung: Comparing repositories](https://www.baeldung.com/spring-data-repositories)

### Spring Data Repositories

- CrudRepository provides CRUD functions

- PagingAndSortingRepository provides methods to do pagination and sort records

- JpaRepository provides JPA related methods such as flushing the persistence context and delete records in a batch

### Crud Repositories

```java

public interface CrudRepository<T, ID extends Serializable>
  extends Repository<T, ID> {

    <S extends T> S save(S entity);

    T findOne(ID primaryKey);

    Iterable<T> findAll();

    Long count();

    void delete(T entity);

    boolean exists(ID primaryKey);
}

```

save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
findOne(…) – get a single entity based on passed primary key value
findAll() – get an Iterable of all available entities in database
count() – return the count of total entities in a table
delete(…) – delete an entity based on the passed object
exists(…) – verify if an entity exists based on the passed primary key value

### PagingAndSortingRepository

```java

public interface PagingAndSortingRepository<T, ID extends Serializable> 
  extends CrudRepository<T, ID> {

    Iterable<T> findAll(Sort sort);

    Page<T> findAll(Pageable pageable);
}

```

### JPA repository

```java

public interface JpaRepository<T, ID extends Serializable> extends
  PagingAndSortingRepository<T, ID> {

    List<T> findAll();

    List<T> findAll(Sort sort);

    List<T> save(Iterable<? extends T> entities);

    void flush();

    T saveAndFlush(T entity);

    void deleteInBatch(Iterable<T> entities);
}


```

findAll() – get a List of all available entities in database
findAll(…) – get a List of all available entities and sort them using the provided condition
save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
flush() – flush all pending task to the database
saveAndFlush(…) – save the entity and flush changes immediately
deleteInBatch(…) – delete an Iterable of entities. Here, we can pass multiple objects to delete them in a batch

