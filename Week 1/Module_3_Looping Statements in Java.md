# Module 3: Looping Statements in Java

## 1. For Loop in Java

The `for` loop in Java is used to iterate over a range of values or elements. It consists of three parts: initialization, condition, and iteration.

```java
for (int i = 0; i < 5; i++) {
    System.out.println("Iteration " + i);
}
```

In this example, `i` is initialized to 0, the loop continues as long as `i` is less than 5, and after each iteration, `i` is incremented by 1.

## 2. Hands-on Exercise on the "For" Loop

**Exercise**: Write a program using a `for` loop to print the first 10 natural numbers.

```java
for (int i = 1; i <= 10; i++) {
    System.out.println(i);
}
```

## 3. Nested For Loop

A nested `for` loop is a loop inside another loop. This is useful for iterating through 2D arrays or performing more complex looping operations.

```java
for (int i = 1; i <= 3; i++) {
    for (int j = 1; j <= 3; j++) {
        System.out.println("i: " + i + ", j: " + j);
    }
}
```

This example demonstrates a nested loop where `i` and `j` iterate from 1 to 3.

## 4. Hands-on Exercise on the "Nested For" Loop

**Exercise**: Write a program using nested `for` loops to print a pattern of asterisks as follows:

```
*
**
***
****
*****
```

```java
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        System.out.print("*");
    }
    System.out.println();
}
```

## 5. While and Do While Loop in Java

The `while` loop and `do-while` loop are used for situations where you do not know in advance how many times the loop will run.

```java
int i = 0;
while (i < 5) {
    System.out.println("Iteration " + i);
    i++;
}
```

The `do-while` loop ensures that the code block inside the loop is executed at least once.

```java
int j = 0;
do {
    System.out.println("Iteration " + j);
    j++;
} while (j < 5);
```

## 6. Loop "Break" and "Continue" Statements

The `break` statement is used to exit a loop prematurely. It is often used within loops to stop the execution of the loop based on a certain condition.

The `continue` statement skips the rest of the loop's code for the current iteration and moves to the next iteration.

```java
for (int i = 0; i < 10; i++) {
    if (i == 5) {
        break; // Exit the loop when i equals 5
    }
    if (i % 2 == 0) {
        continue; // Skip even numbers
    }
    System.out.println("Iteration " + i);
}
```

## 7. Switch Statement and Implementation in Java

The `switch` statement is used to select one of many code blocks to be executed.

```java
int day = 3;
String dayName;
switch (day) {
    case 1:
        dayName = "Sunday";
        break;
    case 2:
        dayName = "Monday";
        break;
    case 3:
        dayName = "Tuesday";
        break;
    // Add more cases as needed
    default:
        dayName = "Invalid Day";
}
System.out.println("Today is " + dayName);
```

This `switch` statement checks the value of `day` and assigns the corresponding day name to `dayName`.

[prev](./Module_2_Java%20Programming%20Fundamentals.md)                    [next](./Module_4_Arrays.md) 