# Module: Strings, StringBuilder, and StringBuffer

## 1. String Basics

In Java, a `String` is a sequence of characters that represents text. It is an immutable class, meaning that once a `String` object is created, its value cannot be changed.

```java
String greeting = "Hello, World!";
```

In this example, `greeting` is a `String` object containing the text "Hello, World!".

## 2. String Comparison Operations

String comparison operations allow you to compare two strings to determine their relationship in lexicographic (dictionary) order.

```java
String str1 = "apple";
String str2 = "banana";
int result = str1.compareTo(str2); // Compare strings lexicographically

if (result < 0) {
    System.out.println(str1 + " comes before " + str2);
} else if (result > 0) {
    System.out.println(str1 + " comes after " + str2);
} else {
    System.out.println(str1 + " is equal to " + str2);
}
```

This will print: "apple comes before banana".

## 3. String Search Operations

String search operations allow you to find substrings within a string.

```java
String sentence = "The quick brown fox jumps over the lazy dog";
int indexOfFox = sentence.indexOf("fox"); // Find the index of "fox"
System.out.println("Index of 'fox': " + indexOfFox);
```

This will print: "Index of 'fox': 16".

## 4. String (Cut) Slice Operations

You can extract a portion of a string using the `substring` method.

```java
String str = "Hello, World!";
String subStr = str.substring(7, 12); // Extract "World"
System.out.println(subStr);
```

This will print: "World".

## 5. String Replace Operations

String replace operations allow you to replace occurrences of a substring with another string.

```java
String message = "Hello, John!";
String updatedMessage = message.replace("John", "Jane");
System.out.println(updatedMessage);
```

This will print: "Hello, Jane!".

## 6. String Conversion Operations

You can convert other data types to strings using methods like `valueOf` or concatenation.

```java
int num = 42;
String strNum = String.valueOf(num);
String concatNum = "The answer is " + num;
```

Here, `strNum` will be the string "42", and `concatNum` will be "The answer is 42".

Remember, `StringBuilder` and `StringBuffer` are mutable alternatives to `String` when you need to perform a large number of modifications on a string.


[prev](./Module_4_Arrays.md)                    [next](./Module_6_Object-Oriented%20Programming%20OOP%20Basics.md)