# Readings

## [Primitives vs Objects](https://www.baeldung.com/java-primitives-vs-objects)

Java has a two-fold type system.

Primitives which are int and boolean.

And Reference types which are Integer and Boolean.

```Java

Integer j = 1;          // autoboxing
int i = new Integer(1); // unboxing

```

Below are primitive type variables that have impact on memory.

```java

boolean – 1 bit
byte – 8 bits
short, char – 16 bits
int, float – 32 bits
long, double – 64 bits

```

## [Exceptions in Java](https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html)

### What Is an Exception?

the term execption is short for "exceptional event".

> An exception is an event, which occurs during the execution of a program, that disrupts the fnormal flow of the program's instructions.

I learned that when there is an error inside of a method, that method creates an object and gives it to the runtime system which has information on the error.

## The Catch or Specify Requirement

Valid Java programming language code must honor the Catch or SPecify Requirement.

- A try statement that catches the exception. The try must provide a handler for the exception.
- A method that specifies that it can throw the exception. The method must provide a trows clause that lists the exception.

Code that does not honor the Catch or Specify will not compile the code.

### The Three kinds of exceptions

- checked exception will basically notify the user when something that is declared in a file but it doesn't exist.

- error will throw a error message when it cannot read a certain file

- runtime exception are not subject to the Catch or Specify Requirement

## [Using Scanner to read in a file in Java](https://docs.oracle.com/javase/tutorial/essential/io/scanning.html)