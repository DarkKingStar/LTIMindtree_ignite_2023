# Module 6: Object-Oriented Programming (OOP) Basics

## 1. Concept of Classes and Objects

Object-Oriented Programming (OOP) is a programming paradigm based on the concept of "objects", which can contain data and code. A class is a blueprint for creating objects. An object is an instance of a class.

```java
class Person {
    String name;
    int age;
}

Person john = new Person();
john.name = "John Doe";
john.age = 30;
```

Here, we define a `Person` class with `name` and `age` attributes. We then create an instance of the `Person` class named `john` and set its attributes.

## 2. Classes and Objects - Exercise 1

**Exercise**: Create a class called `Car` with attributes `make`, `model`, and `year`. Create an instance of the `Car` class and set its attributes.

```java
class Car {
    String make;
    String model;
    int year;
}

Car myCar = new Car();
myCar.make = "Toyota";
myCar.model = "Camry";
myCar.year = 2022;
```

## 3. Methods in Java

Methods in Java are blocks of code that perform a specific task. They are defined within a class and can be called to execute the code.

```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }
}
```

In this example, the `add` method takes two integers as parameters and returns their sum.

## 4. Constructor

A constructor is a special method used to initialize objects when they are created. It has the same name as the class and does not have a return type.

```java
class Person {
    String name;

    Person(String n) {
        name = n;
    }
}
```

Here, we have a constructor that takes a `String` parameter `n` and assigns it to the `name` attribute.

## 5. `this` Keyword

The `this` keyword refers to the current instance of a class. It is used to differentiate between class attributes and method parameters with the same name.

```java
class Person {
    String name;

    Person(String name) {
        this.name = name; // Use "this" to refer to the class attribute
    }
}
```

## 6. `Static` Keyword

The `static` keyword is used to create variables and methods that belong to the class rather than to any specific instance.

```java
class Counter {
    static int count = 0;

    Counter() {
        count++;
    }
}
```

In this example, `count` is a static variable that is shared among all instances of the `Counter` class.

## 7. `Final` Keyword

The `final` keyword can be applied to variables, methods, and classes. It indicates that the element cannot be modified or extended.

```java
class Circle {
    final double PI = 3.14;
}
```

Here, `PI` is a final variable and cannot be changed.

## 8. Scope of Variables

The scope of a variable is the part of the program where the variable can be accessed. Variables can have local scope (limited to a block of code) or class scope (accessible throughout the class).

```java
class Example {
    int x; // Class scope variable

    void method() {
        int y = 10; // Local scope variable
        System.out.println(x + y); // x is accessible here
    }
}
```

`x` is accessible throughout the class, while `y` is only accessible within the `method`.

[prev](./Module_5_Strings%20StringBuilder%20and%20StringBuffer.md)                    [next](./Module_7_Arrays%20as%20Object%20Args%20and%20Return%20Value.md)
