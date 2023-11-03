# Module 1: Lists

## 1. ArrayList

`ArrayList` is a dynamic array implementation in Java. It allows for the dynamic resizing of the underlying array to accommodate the addition or removal of elements.

```java
import java.util.ArrayList;

ArrayList<String> names = new ArrayList<>();
names.add("Alice");
names.add("Bob");
names.add("Charlie");
```

Here, we create an `ArrayList` of strings and add elements to it.

## 2. Linked List Structure

A linked list is a data structure where each element (node) holds a reference to the next node. Unlike arrays, linked lists do not have a fixed size.

```java
class Node {
    int data;
    Node next;
}
```

This is an example of a basic node structure for a linked list.

## 3. LinkedList

`LinkedList` is a doubly-linked list implementation in Java. It allows for efficient insertion and deletion of elements anywhere in the list.

```java
import java.util.LinkedList;

LinkedList<Integer> numbers = new LinkedList<>();
numbers.add(10);
numbers.add(20);
numbers.add(30);
```

Here, we create a linked list of integers and add elements to it.

## 4. ArrayList vs. LinkedList

- `ArrayList`:
  - Implements dynamic arrays.
  - Efficient for random access and iteration.
  - Slower for inserting or deleting elements in the middle.

- `LinkedList`:
  - Implements doubly-linked lists.
  - Efficient for inserting or deleting elements.
  - Slower for random access and iteration.

The choice between `ArrayList` and `LinkedList` depends on the specific requirements of your program.

## 5. List Iterator

A `ListIterator` allows you to iterate over a `List` and perform various operations like adding, removing, and replacing elements.

```java
import java.util.ArrayList;
import java.util.ListIterator;

ArrayList<String> names = new ArrayList<>();
names.add("Alice");
names.add("Bob");
names.add("Charlie");

ListIterator<String> iterator = names.listIterator();

while (iterator.hasNext()) {
    String name = iterator.next();
    System.out.println(name);
}
```

In this example, we create an `ArrayList` of names and use a `ListIterator` to iterate through the list.