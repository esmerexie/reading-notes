# Readings

## [Java OO Tutorial (review Object and Class, read the rest)](https://docs.oracle.com/javase/tutorial/java/concepts/)

### What is an Object?

an object is a software bundle of related state and behavior.  An objects stores its state in fields and exposees its behavior through methods.

Methods operate on an object's internal state and serves as the primary mechanism for object-to-object communication.

### What is a class?

A class is a blueprint from which indivudual objects are created.

An example :

```java


class Bicycle {

    int cadence = 0;
    int speed = 0;
    int gear = 1;

    void changeCadence(int newValue) {
         cadence = newValue;
    }

    void changeGear(int newValue) {
         gear = newValue;
    }

    void speedUp(int increment) {
         speed = speed + increment;   
    }

    void applyBrakes(int decrement) {
         speed = speed - decrement;
    }

    void printStates() {
         System.out.println("cadence:" +
             cadence + " speed:" + 
             speed + " gear:" + gear);
    }
}

```

### [Interfaces](https://docs.oracle.com/javase/tutorial/java/IandI/createinterface.html)

### [Inheritance](https://docs.oracle.com/javase/tutorial/java/IandI/subclasses.html)

## Things I want to know more about