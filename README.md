# Lab Assignment 03

In this lab you will practice writing Java code to input user data and use simple arithmetic.

Same as Lab Assignment 01 and 02, you need to set up your workspace (class and main() method).

## Let's get started!

First, let's look at the name of our .java file in the `src/` directory and name our class accordingly and remember to make it `public`.

Next, **create your main() method inside your class**. It should be the same as in Lab Assignment 01 and 02. Try writing the main() method without looking at your notes. Writing your main class and method should come to you as natural as in C++.

Now let the fun begin!

### Getting user input

To get user input in Java you must first import the **Scanner** class from the `java.util` package. Importing packages in Java must be done at the start of your code.

```java
import java.util.Scanner;

// Your code should start here.
```

Next, you must create a Scanner object inside of your main() method. This object will be used to get all of your user input regardless of their data type.

Creating an object in Java is done the same as in C++.

```java
		// Inside main() method.
		Scanner scanner = new Scanner(System.in);
```

But how do we user the scanner object to get user input?

Scanner has many built-in methods to read user input depending on the type of data we're expecting (ex: String, int, double, etc.).

| **Method** | **Description** |
| ---- | ---- |
| next() | Reads a `String` value **without spaces** from the user |
| nextLine() | Reads a `String` value from the user |
| nextByte() | Reads a `byte` value from the user |
| nextShort() | Reads a `short` value from the user |
| nextInt() | Reads an `int` value from the user |
| nextFloat() | Reads a `float` value from the user |
| nextDouble() | Reads a `double` value from the user |
| nextBoolean() | Reads a `boolean` value from the user |

The code snippet below shows how to input a float from the user.

```java
		// Inside main() method.
		float num;
		num = scanner.nextFloat();
```

For more information on the Scanner class and how it's used visit: https://www.w3schools.com/java/java_user_input.asp

### Arithmetic operations

Exactly the same as C++. Only Java has the shift arithmetic operators (<<, >>).

To learn more about Java arithmetic operators visit: https://www.w3schools.com/java/java_operators.asp

## Your Assignment

### Magic Number Calculator

Calculate a person's magic number using arithmetic operations in Java. A person's magic number is calculated by multiplying the month of their birth by the year of their birth, and taking the modulus of that result and the day of their birth. The equation is:

&emsp;**magic_number = (birth_month * birth_year) % birth_day**

Write a program that will ask the user for their name, month of birth, day of birth, and year of birth and then output their magic number.

**Expected output:**

```
Welcome to Magic Number Calculator!
Enter your name: Bob Bobbert
Enter your dob in format mm dd YY: 07 04 1776

Bob Bobbert your magic number is 0!
```

## Submit your assignment

To submit your lab assignment click on the **Source Control** icon (3 circles with 2 lines) on your leftside navbar. Next, click on the **+** symbol next to **Changes** to stage your changes. Lastly, add a commit message (ex: "First commit") and click **Commit** then **Sync Changes**. And you're done!
