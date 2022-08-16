# Readings

## Why it matters

I think knowing the different types of loop matters when it comes to coding because there will be instances where one type of loop is not effective when it comes to problem solving. Maybe the best loop to solve the problem is a for loop or a While loop.

[Different types of loops in Java](https://www.baeldung.com/java-loops)

The different types of loops in java consit of

1. For loop - which is a control structure that allows it to repate certain operations by incrementing and evaluating a loop counter

```Java
//simple for loop
for(int let i = 0; i < 2; i++){
    System.out.println("Simple for loop: i = " + i);
}


//labeled for loop
aa: for(int i = 1; i <= 3; i++){
    if (i == 1)
    continue;
    bb: for (int j = 1; j <= 3; j++){
        if (i == 2 && j == 2){
            break aa;
        }
        System.out.println(i + " " + j)
      }
}

```

2. While loop - it repeats a statement or a block of statements while its controlling boolean-expression is true.

```Java

int i = 0;
while (i < 5) {
    System.out.println("While loop: i = " + i++);
}

```

3. Do-While loop - is like a while loop execpt the first condition evaluation happens after the first iteration of the loop.

```Java

int i = 0;
do {
    System.out.println("Do-While loop: i = " + i++);
} while (i < 5);

```

## Arrays

An array is used to store a collection of data of the same type.

```Java

//delcaring array Variables
dataType[] arrayRefVar;

//Another example
dataType[] arrayRefVar = new dataType[arraySize];

//Example of a double array
double[] myList = new double [10]

//You can proccess arrays with for loop or foreach

public class TestArray {

   public static void main(String[] args) {
      double[] myList = {1.9, 2.9, 3.4, 3.5};

      // Print all the array elements
      for (int i = 0; i < myList.length; i++) {
         System.out.println(myList[i] + " ");
      }
     
      // Summing all elements
      double total = 0;
      for (int i = 0; i < myList.length; i++) {
         total += myList[i];
      }
      System.out.println("Total is " + total);
      
      // Finding the largest element
      double max = myList[0];
      for (int i = 1; i < myList.length; i++) {
         if (myList[i] > max) max = myList[i];
      }
      System.out.println("Max is " + max);  
   }
}

//example of a foreach 
public class TestArray {

   public static void main(String[] args) {
      double[] myList = {1.9, 2.9, 3.4, 3.5};

      // Print all the array elements
      for (double element: myList) {
         System.out.println(element);
      }
   }
}

```

## Things I want to know more about

I want to know more about on how to decide which type of loop would be more effective when solving a problem.