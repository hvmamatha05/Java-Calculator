# Java-Calculator
A simple Java-based Calculator application that performs basic arithmetic operations such as Addition, Subtraction, Multiplication, and Division using methods and user input.


## Project Overview

The Java Console Calculator is a menu-driven application developed using Java. The calculator performs basic arithmetic operations such as Addition, Subtraction, Multiplication, and Division. The application accepts user input through the console and displays the calculated result.

The project was developed to understand Java fundamentals, methods, loops, conditional statements, user input handling, and Object-Oriented Programming concepts.

---

# Objective

The objective of this project is to build a calculator using Java Console I/O and strengthen programming logic while implementing arithmetic operations using methods.

---

# Tools Used

* Java (JDK)
* Notepad
* Command Prompt
* GitHub

---

# Features

* Addition
* Subtraction
* Multiplication
* Division
* Division by Zero Validation
* Menu Driven Interface
* Continuous Execution Until Exit
* User-Friendly Console Interaction

---

# Project Workflow

```text
Start Program
      ↓
Display Calculator Menu
      ↓
Read User Choice
      ↓
Validate Choice
      ↓
Read Two Numbers
      ↓
Call Required Method
      ↓
Perform Calculation
      ↓
Display Result
      ↓
Continue or Exit
      ↓
End Program
```

## Workflow Explanation

### Step 1: Start Program

Execution begins from the main() method.

```java
public static void main(String[] args)
```

The JVM starts program execution from this method.

### Step 2: Create Scanner Object

```java
Scanner sc = new Scanner(System.in);
```

Scanner is used to receive user input from the keyboard.

### Step 3: Display Menu

The calculator displays:

* Addition
* Subtraction
* Multiplication
* Division
* Exit

### Step 4: Read User Choice

```java
choice = sc.nextInt();
```

The selected option is stored in the choice variable.

### Step 5: Validate User Choice

```java
if(choice >= 1 && choice <= 4)
```

Only valid operations are processed.

### Step 6: Read Input Numbers

```java
double num1 = sc.nextDouble();
double num2 = sc.nextDouble();
```

Double is used because it supports decimal values.

### Step 7: Execute Selected Operation

```java
switch(choice)
```

The switch statement calls the corresponding method.

### Step 8: Display Result

The returned value is displayed to the user.

### Step 9: Repeat

The do-while loop continues until the user selects Exit.

```java
while(choice != 5);
```

### Step 10: Close Application

```java
sc.close();
```

The Scanner object is closed and the application terminates.

---

# Complete Code Explanation

## Import Statement

```java
import java.util.Scanner;
```

Imports the Scanner class which is used for reading user input.

### Why Scanner?

Scanner provides built-in methods such as:

* nextInt()
* nextDouble()
* next()

for taking user input.

---

## Class Declaration

```java
public class Calculator
```

The Calculator class acts as a blueprint containing methods and application logic.

---

## Addition Method

```java
public static double add(double a, double b)
{
    return a + b;
}
```

Purpose:
Returns the sum of two numbers.

Explanation:

* public → accessible from anywhere
* static → can be called without object creation
* double → return type
* a,b → parameters

---

## Subtraction Method

```java
public static double subtract(double a, double b)
{
    return a - b;
}
```

Returns the difference between two numbers.

---

## Multiplication Method

```java
public static double multiply(double a, double b)
{
    return a * b;
}
```

Returns the product of two numbers.

---

## Division Method

```java
public static double divide(double a, double b)
{
    if(b == 0)
    {
        System.out.println("Cannot divide by zero!");
        return 0;
    }

    return a / b;
}
```

Purpose:

Performs division and prevents division-by-zero errors.

Why this validation?

Division by zero is mathematically invalid and may produce unexpected results.

---

## Main Method

```java
public static void main(String[] args)
```

The entry point of the Java application.

Program execution begins from here.

---

## Choice Variable

```java
int choice;
```

Stores the operation selected by the user.

---

## do-while Loop

```java
do
{
}
while(choice != 5);
```

Reason:

The calculator menu should appear at least once and continue until Exit is selected.

---

## Switch Statement

```java
switch(choice)
```

Used to execute different operations efficiently.

Cases:

* Case 1 → Addition
* Case 2 → Subtraction
* Case 3 → Multiplication
* Case 4 → Division

---

## Invalid Choice Handling

```java
else if(choice != 5)
{
    System.out.println("Invalid choice!");
}
```

Displays an error message for invalid menu selections.

---

## Closing Scanner

```java
sc.close();
```

Releases system resources and follows good programming practices.

---

# OOP Concepts Used

## Class

```java
public class Calculator
```

A class is a blueprint for creating objects.

---

## Methods

```java
add()
subtract()
multiply()
divide()
```

Methods improve:

* Reusability
* Readability
* Maintainability

---

## Abstraction

The user only sees:

* Menu
* Inputs
* Results

Internal calculations remain hidden.

---

## Modularity

Each operation is implemented separately, making future modifications easier.

---

# Challenges Faced

* Understanding Java syntax.
* Learning Scanner usage.
* Handling division-by-zero conditions.
* Debugging compilation errors.
* Understanding execution flow.

---

# Learning Outcomes

Through this project I learned:

* Java Fundamentals
* Methods and Functions
* Scanner Class
* Conditional Statements
* Switch Statements
* Loops
* Program Flow
* Debugging
* Basic OOP Concepts

---

# Future Enhancements

* Percentage Calculations
* Square Root Operations
* Power Calculations
* Exception Handling
* Calculation History

---

# Interview Explanation

My project is a Java-based Console Calculator Application. The application performs Addition, Subtraction, Multiplication, and Division operations. User input is handled using the Scanner class. A switch statement is used to determine which operation should be performed, and a do-while loop keeps the calculator running until the user chooses Exit. Separate methods are used for each arithmetic operation to improve code modularity and reusability. I also implemented division-by-zero validation and invalid menu choice handling. Through this project, I gained practical experience in Java programming, OOP concepts, loops, conditionals, debugging, and software development fundamentals.

---

# Common Interview Questions

### What is Method Overloading?

Method overloading means having multiple methods with the same name but different parameters.

### Why handle divide-by-zero?

To prevent invalid calculations and improve application reliability.

### Difference between == and equals()?

* == compares references/primitives.
* equals() compares object content.

### What are Java primitive data types?

byte, short, int, long, float, double, char, boolean.

### How is Scanner used?

Scanner is used for reading user input from the console.

### What is JVM?

JVM (Java Virtual Machine) executes Java bytecode.

### Why is Java Platform Independent?

Java code runs on any operating system that has a JVM.

### How do you debug a Java program?

By analyzing error messages, using print statements, and debugging tools in IDEs.

---

# Author

Mamatha 
