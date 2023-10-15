# Java Programming Fundamentals

## 1. Java Development Kit (JDK) Installation{#t1}

The Java Development Kit (JDK) is a software package that provides the tools needed for developing, testing, and running Java applications. Here's a step-by-step guide on how to install JDK:

1. **Download JDK**:
   - Visit the [official Oracle JDK download page](https://www.oracle.com/java/technologies/javase-downloads.html).
   - Select the appropriate version for your operating system (Windows, macOS, Linux).
   - Follow the on-screen instructions to download the installer.

2. **Install JDK**:
   - Run the downloaded installer.
   - Follow the installation wizard's prompts. You can choose the default settings for most options.
   - Once the installation is complete, verify the installation by opening a command prompt or terminal and typing `java -version`. It should display the installed Java version.

## 2. Eclipse Installation {#t2}

Eclipse is a widely used integrated development environment (IDE) for Java development. It provides a range of features to facilitate Java programming. Here's how to install Eclipse:

1. **Download Eclipse**:
   - Visit the [official Eclipse download page](https://www.eclipse.org/downloads/).
   - Choose the "Eclipse IDE for Java Developers" package.
   - Select the appropriate version for your operating system.
   - Download the installer.

2. **Install Eclipse**:
   - Run the downloaded installer.
   - Follow the installation wizard's prompts. You can choose the default settings for most options.
   - Once the installation is complete, launch Eclipse.

## 3. Writing Your First Java Program {#t3}

Now that you have the JDK and Eclipse set up, let's write a simple Java program:

1. **Open Eclipse**:
   - Launch Eclipse from the start menu or desktop shortcut.

2. **Create a New Java Project**:
   - Go to `File` > `New` > `Java Project`.
   - Give your project a name (e.g., `HelloWorld`).
   - Click `Finish`.

3. **Create a New Java Class**:
   - In the `src` folder of your project, right-click and select `New` > `Class`.
   - Enter a name for your class (e.g., `HelloWorld`).
   - Check the box that says `public static void main(String[] args)` to create a main method.
   - Click `Finish`.

4. **Write Your Java Program**:
   - In the editor, you'll see the skeleton of your class with the `main` method.
   - Add the following code to print "Hello, World!" to the console:
     ```java
     public class HelloWorld {
         public static void main(String[] args) {
             System.out.println("Hello, World!");
         }
     }
     ```

5. **Run Your Program**:
   - Right-click on the file in the Package Explorer and select `Run As` > `Java Application`.
   - You should see "Hello, World!" printed in the console.

Congratulations! You've successfully written and executed your first Java program.

## 4. Primitive Data Types in Java {#t4}

In Java, primitive data types represent single values, and they are not objects. They include:

- `byte`: 8-bit integer
- `short`: 16-bit integer
- `int`: 32-bit integer
- `long`: 64-bit integer
- `float`: 32-bit floating point
- `double`: 64-bit floating point
- `char`: 16-bit Unicode character
- `boolean`: Represents true or false

Example:

```java
int num = 10;
double pi = 3.14;
char letter = 'A';
boolean isJavaFun = true;
```

## 5. Arithmetic Operators in Java {#t5}

Arithmetic operators perform mathematical operations on numerical values. They include `+` (addition), `-` (subtraction), `*` (multiplication), `/` (division), and `%` (modulo).

Example:

```java
int a = 10;
int b = 5;
int sum = a + b; // sum = 15
int difference = a - b; // difference = 5
int product = a * b; // product = 50
int quotient = a / b; // quotient = 2
int remainder = a % b; // remainder = 0
```

## 6. Logical and Bitwise Operators {#t6}

Logical operators perform operations on boolean values. They include `&&` (logical AND), `||` (logical OR), and `!` (logical NOT).

Bitwise operators perform operations on individual bits of integers. They include `&` (bitwise AND), `|` (bitwise OR), `^` (bitwise XOR), `~` (bitwise NOT), `<<` (left shift), and `>>` (right shift).

Example:

```java
boolean a = true;
boolean b = false;
boolean result1 = a && b; // result1 = false (logical AND)
boolean result2 = a || b; // result2 = true (logical OR)
boolean result3 = !a; // result3 = false (logical NOT)

int x = 5; // Binary representation: 0101
int y = 3; // Binary representation: 0011
int bitwiseAnd = x & y; // bitwiseAnd = 1 (Bitwise AND)
int bitwiseOr = x | y; // bitwiseOr = 7 (Bitwise OR)
int bitwiseXor = x ^ y; // bitwiseXor = 6 (Bitwise XOR)
```

## 7. Relational Operators in Java {#t7}

Relational operators compare two values and return a boolean result. They include `==` (equal to), `!=` (not equal to), `>` (greater than), `<` (less than), `>=` (greater than or equal to), and `<=` (less than or equal to).

Example:

```java
int p = 5;
int q = 7;
boolean isEqual = (p == q); // isEqual = false
boolean isNotEqual = (p != q); // isNotEqual = true
boolean isGreater = (p > q); // isGreater = false
boolean isLess = (p < q); // isLess = true
boolean isGreaterOrEqual = (p >= q); // isGreaterOrEqual = false
boolean isLessOrEqual = (p <= q); // isLessOrEqual = true
```

## 8. If - Condition {#t8}

The `if` statement allows you to execute a block of code if a specified condition is true.

Example:

```java
int num = 10;
if (num > 5) {
    System.out.println("Number is greater than 5");
}
```

## 9. Nested If - Condition {#t9}

You can use nested `if` statements to handle multiple conditions.

Example:

```java
int num = 10;
if (num > 5) {
    if (num < 15) {
        System.out.println("Number is between 5 and 15");
    }
}
```

## 10. Typecasting {#t10}

Typecasting is the process of converting a value from one data type to another. In Java, there are two types of typecasting: implicit (automatic) and explicit (manual).

### Explicit Typecasting

Explicit typecasting is when you manually convert a value from one type to another. This is done by specifying the target type in parentheses before the value.

Example:

```java
double myDouble = 5.5;
int myInt = (int) myDouble; // Explicit typecasting, myInt will be 5
```

Here, we're converting a `double` value (`5.5`) to an `int`. The fractional part is truncated, resulting in `5`.

### Implicit Typecasting

Implicit typecasting, also known as widening or automatic type conversion, occurs when Java automatically converts a smaller data type to a larger data type. This happens without the need for any explicit instructions.

Example:

```java
int myInt = 5;
double myDouble = myInt; // Implicit typecasting, myDouble will be 5.0
```

In this example, an `int` value (`5`) is automatically converted to a `double` without any explicit casting. This is because a `double` can hold a wider range of values than an `int`.

**Note**: Implicit typecasting can be done when:

- The data types are compatible.
- The target type has a larger range than the source type.

For example, you can implicitly cast from `byte` to `short`, `int`, `long`, `float`, or `double`.

Keep in mind that implicit typecasting can result in loss of precision or range, so be cautious when converting between different data types.

If you try to perform an implicit typecast from a wider data type to a narrower one, you may need to use explicit casting, and there may be a risk of losing data.

```java
double myDouble = 5.5;
int myInt = (int) myDouble; // Explicit typecasting, myInt will be 5
```

Here, we're converting a `double` value (`5.5`) to an `int`. The fractional part is truncated, resulting in `5`.

