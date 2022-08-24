# Readings

## [Java OO Tutorial](https://docs.oracle.com/javase/tutorial/java/concepts/object.html)

### What is an object?

Objects share two characteristics:

1. State

2. Behavior

For example a Cat's state could be the name **Moo** and it's behavior could be **meowing**

An object stores it's state in feilds and exposes their behavior through methods.

## [Classes](https://docs.oracle.com/javase/tutorial/java/javaOO/classes.html)

Below are examples pulled from the website to help and explain classes.

```Java

public class Bicycle {
        
    // the Bicycle class has
    // three fields
    public int cadence;
    public int gear;
    public int speed;
        
    // the Bicycle class has
    // one constructor
    public Bicycle(int startCadence, int startSpeed, int startGear) {
        gear = startGear;
        cadence = startCadence;
        speed = startSpeed;
    }
        
    // the Bicycle class has
    // four methods
    public void setCadence(int newValue) {
        cadence = newValue;
    }
        
    public void setGear(int newValue) {
        gear = newValue;
    }
        
    public void applyBrake(int decrement) {
        speed -= decrement;
    }
        
    public void speedUp(int increment) {
        speed += increment;
    }
        
}

```

And here is a class declaration for MoutainBike that is a subclass of the class above

```Java

public class MountainBike extends Bicycle {
        
    // the MountainBike subclass has
    // one field
    public int seatHeight;

    // the MountainBike subclass has
    // one constructor
    public MountainBike(int startHeight, int startCadence,
                        int startSpeed, int startGear) {
        super(startCadence, startSpeed, startGear);
        seatHeight = startHeight;
    }   
        
    // the MountainBike subclass has
    // one method
    public void setHeight(int newValue) {
        seatHeight = newValue;
    }   

}

```

## [Binary, Decimal and Hexadecimal Numbers](https://www.mathsisfun.com/binary-decimal-hexadecimal.html)

### Decimals

Counting decimals can be easy

for example

. = 1

.. = 2

..... = 5

.......... = 10 / just adding a 1 to the left

.......... = 11

## [Binary Numbers](https://www.mathsisfun.com/binary-decimal-hexadecimal.html)

 = 0 /start a zero

 . = 1

.. = 10 // there is no "2" in binary, so start back at 0 ...
... and add one to the number on the left

... = 11

.... = 100 // start back at 0 again, and add one to the number on the      left...
... but that number is already at 1 so it also goes back to 0 ...
... and 1 is added to the next position on the left

..... = 101

...... = 110

....... = 111

........ = 1000

## Hexadecimal Numbers

Decimal: 0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15

Hexadecimal: 0 1 2 3 4 5 6 7 8 9 A B C D E F
