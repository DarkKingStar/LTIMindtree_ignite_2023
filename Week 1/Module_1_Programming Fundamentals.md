# Module 1: Programming Fundamentals

## 1. What is Programming?

Programming is the process of instructing a computer to perform specific tasks or solve problems. It involves writing sets of instructions, also known as code, using a programming language that the computer can understand and execute. Programming allows us to automate tasks, manipulate data, and create applications ranging from simple scripts to complex software.

### Example:

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

In this Java example, we have a simple program that prints "Hello, World!" to the console. This is often the first program beginners write when learning a new programming language.

---

## 2. What is Algorithm, Pseudocode, and Flowchart?

### Algorithm:

An algorithm is a step-by-step set of instructions for solving a specific problem or performing a task. It is a high-level description of the logic needed to accomplish the task, independent of any particular programming language. Algorithms are essential in problem-solving and form the basis for writing code.

### Pseudocode:

Pseudocode is a way of expressing an algorithm in human-readable language. It uses a combination of natural language and basic programming constructs to outline the logic of the solution. Pseudocode helps programmers plan and structure their code before translating it into a specific programming language.

### Example Pseudocode (Finding the maximum of two numbers):

```
function findMax(num1, num2)
    if num1 > num2 then
        return num1
    else
        return num2
    end if
end function
```

### Flowchart:

A flowchart is a visual representation of an algorithm. It uses various shapes to represent different steps or processes, with arrows indicating the flow of execution. Flowcharts are particularly useful for illustrating complex processes and understanding the flow of control in a program.

### Example Flowchart (Finding the maximum of two numbers):

```
[Start] --> (Input num1)
           --> (Input num2)
           --> [num1 > num2?] --> [Yes] --> (Output num1 as max)
                             --> [No]  --> (Output num2 as max)
           --> [End]
```

These are powerful tools that help programmers plan, communicate, and implement solutions effectively.

[next](./Module_2_Java%20Programming%20Fundamentals.md)