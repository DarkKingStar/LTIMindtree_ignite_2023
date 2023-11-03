# Module 3: Finalize and Garbage Collector

## 1. Finalize

**Finalize**:
- The `finalize()` method is a part of the `Object` class in Java.
- It is called by the garbage collector before it reclaims the memory occupied by an object.
- It provides an opportunity for the object to perform any necessary cleanup operations before it is garbage collected.
- It's important to note that the `finalize()` method is not guaranteed to be called promptly or at all.

Example:
```java
class Example {
    @Override
    protected void finalize() throws Throwable {
        try {
            // Cleanup code here
        } finally {
            super.finalize();
        }
    }
}
```

## 2. Garbage Collectors

**Garbage Collectors**:
- Java uses automatic garbage collection to manage memory.
- The garbage collector runs in the background and identifies objects that are no longer reachable.
- It reclaims the memory occupied by those objects.
- Different garbage collection algorithms exist, such as the Mark-and-Sweep algorithm and Generational Garbage Collection.

## 3. Demo - Garbage Collectors and Finalize

A demo can illustrate how `finalize()` is called by the garbage collector. For example:

```java
class Example {
    @Override
    protected void finalize() throws Throwable {
        System.out.println("Finalize method called");
        super.finalize();
    }
}

public class Main {
    public static void main(String[] args) {
        Example example = new Example();
        example = null; // Object is now eligible for garbage collection
        System.gc(); // Suggest to the JVM to run garbage collector
    }
}
```

In this example, we create an instance of the `Example` class. After setting it to `null`, it becomes eligible for garbage collection. By calling `System.gc()`, we suggest to the JVM to run the garbage collector.

## 4. Final Keyword

**Final Keyword**:
- `final` is a keyword in Java that can be applied to classes, methods, and variables.
- When applied to a class, it indicates that the class cannot be subclassed.
- When applied to a method, it indicates that the method cannot be overridden.
- When applied to a variable, it indicates that the variable's value cannot be changed.

Example:
```java
final class Example {
    final int value = 10;

    final void printValue() {
        System.out.println(value);
    }
}
```

## 5. Access Specifiers in Java

**Access Specifiers**:
- Access specifiers control the visibility of classes, methods, and variables in different parts of a program.
- The main access specifiers are `public`, `protected`, default (package-private), and `private`.
- They help enforce encapsulation and prevent unauthorized access to sensitive parts of the code.

Example:
```java
public class Example {
    private int privateValue;
    protected int protectedValue;
    int defaultValue;
    public int publicValue;
}
```

## 6. JARs

**JAR (Java Archive)**:
- A JAR file is a compressed file format used to distribute Java applications or libraries.
- It can contain multiple Java classes, resources, and metadata.
- JAR files are platform-independent and can be executed using the Java Runtime Environment (JRE).

To create a JAR file:
```bash
jar cvf MyJar.jar MyClass.class
```

To run a JAR file:
```bash
java -jar MyJar.jar
```