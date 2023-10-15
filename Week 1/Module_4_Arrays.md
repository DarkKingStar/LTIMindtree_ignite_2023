# Module 4: Arrays

## 1. Arrays in Java

An array in Java is a collection of elements of the same type, stored in contiguous memory locations. It allows you to store multiple values under a single variable name.

```java
int[] numbers = {1, 2, 3, 4, 5};
```

Here, we have an array named `numbers` containing five integers.

## 2. Array Object

In Java, arrays are objects. They have a length property and can be passed to methods like any other object.

```java
int[] numbers = new int[5]; // Array of length 5
```

This creates an array of integers with a length of 5. The elements will be initialized to their default values (0 in this case).

## 3. Modified/Enhanced "For" loop

The enhanced `for` loop (also known as the "for-each" loop) simplifies iterating over arrays or collections.

```java
int[] numbers = {1, 2, 3, 4, 5};
for (int num : numbers) {
    System.out.println(num);
}
```

This loop iterates through each element in the `numbers` array and prints its value.

## 4. Array Exercise

**Exercise**: Write a program that finds the largest element in an array.

```java
int[] numbers = {10, 5, 7, 25, 15};
int max = numbers[0]; // Assume the first element is the largest

for (int i = 1; i < numbers.length; i++) {
    if (numbers[i] > max) {
        max = numbers[i]; // Update max if a larger element is found
    }
}

System.out.println("The largest element is: " + max);
```

## 5. Two-dimensional (2D) Arrays

A 2D array in Java is an array of arrays. It is used to represent tables or matrices.

```java
int[][] matrix = {
    {1, 2, 3},
    {4, 5, 6},
    {7, 8, 9}
};
```

Here, `matrix` is a 3x3 array.

## 6. Two-dimensional (2D) Array Exercise

**Exercise**: Write a program to find the sum of all elements in a 2D array.

```java
int[][] matrix = {
    {1, 2, 3},
    {4, 5, 6},
    {7, 8, 9}
};

int sum = 0;

for (int[] row : matrix) {
    for (int num : row) {
        sum += num;
    }
}

System.out.println("The sum of all elements is: " + sum);
```

This program calculates the sum of all elements in the `matrix` array.

[prev](./Module_3_Looping%20Statements%20in%20Java.md)                    [next](./Module_5_Strings%20StringBuilder%20and%20StringBuffer.md)