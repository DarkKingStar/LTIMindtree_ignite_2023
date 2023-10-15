# Module 7: Arrays as Object, Args, and Return Value

## 1. Pass an Array as Parameters

In Java, you can pass an array as a parameter to a method. This allows you to operate on the elements of the array within the method.

```java
void printArray(int[] arr) {
    for (int element : arr) {
        System.out.print(element + " ");
    }
}
```

This method `printArray` takes an integer array `arr` as a parameter and prints its elements.

## 2. Array of Objects

Arrays can hold objects just like they hold primitive data types. For example, an array of `String` objects:

```java
String[] names = {"Alice", "Bob", "Charlie"};
```

Here, `names` is an array of `String` objects.

## 3. Array of Objects as Parameters

You can pass an array of objects as a parameter to a method.

```java
void printNames(String[] names) {
    for (String name : names) {
        System.out.println(name);
    }
}
```

This method `printNames` takes an array of `String` objects and prints each name.

## 4. Pass an Array as Return Type in a Method

You can have a method return an array as well.

```java
int[] generateNumbers() {
    int[] numbers = {1, 2, 3, 4, 5};
    return numbers;
}
```

This method `generateNumbers` returns an array of integers.

Keep in mind that arrays are reference types. When you pass an array to a method, you're actually passing a reference to the array, not a copy of the array itself. This means any changes made to the array within the method will affect the original array.

[prev](./Module_6_Object-Oriented%20Programming%20OOP%20Basics.md)                    [next](../Week%202/)
