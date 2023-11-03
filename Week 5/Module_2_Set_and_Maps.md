# Module 2: Sets and Maps

## 1. HashSet

**HashSet**:
- Implementation of the `Set` interface using a hash table.
- Does not allow duplicate elements.
- Provides constant-time performance for basic operations like add, remove, contains, etc.

Example:
```java
import java.util.HashSet;

HashSet<String> fruits = new HashSet<>();
fruits.add("Apple");
fruits.add("Banana");
fruits.add("Orange");
```

## 2. LinkedHashSet

**LinkedHashSet**:
- Implements the `Set` interface with a combination of a hash table and a doubly-linked list.
- Maintains the insertion order of elements.
- Slightly slower than `HashSet` due to the added maintenance of the linked list.

Example:
```java
import java.util.LinkedHashSet;

LinkedHashSet<Integer> numbers = new LinkedHashSet<>();
numbers.add(5);
numbers.add(2);
numbers.add(8);
```

## 3. TreeSet

**TreeSet**:
- Implementation of the `SortedSet` interface.
- Stores elements in a sorted order (defined by natural ordering or a custom `Comparator`).
- Implemented using a Red-Black tree, providing log(n) time complexity for most operations.

Example:
```java
import java.util.TreeSet;

TreeSet<String> names = new TreeSet<>();
names.add("Alice");
names.add("Bob");
names.add("Charlie");
```

## 4. Iterating over Sets

You can iterate over sets using a for-each loop or an iterator.

Example:
```java
HashSet<String> fruits = new HashSet<>();
fruits.add("Apple");
fruits.add("Banana");
fruits.add("Orange");

for (String fruit : fruits) {
    System.out.println(fruit);
}
```

## 5. HashMap

**HashMap**:
- Implements the `Map` interface using a hash table for key-value pairs.
- Does not allow duplicate keys; each key maps to at most one value.
- Provides constant-time performance for basic operations.

Example:
```java
import java.util.HashMap;

HashMap<String, Integer> ages = new HashMap<>();
ages.put("Alice", 30);
ages.put("Bob", 25);
ages.put("Charlie", 35);
```

## 6. TreeMap

**TreeMap**:
- Implementation of the `SortedMap` interface.
- Stores entries in a sorted order based on the keys.
- Provides log(n) time complexity for most operations.

Example:
```java
import java.util.TreeMap;

TreeMap<String, Integer> ages = new TreeMap<>();
ages.put("Alice", 30);
ages.put("Bob", 25);
ages.put("Charlie", 35);
```

## 7. Iterating on Maps

You can iterate over maps using a for-each loop or an iterator.

Example:
```java
HashMap<String, Integer> ages = new HashMap<>();
ages.put("Alice", 30);
ages.put("Bob", 25);
ages.put("Charlie", 35);

for (Map.Entry<String, Integer> entry : ages.entrySet()) {
    System.out.println(entry.getKey() + ": " + entry.getValue());
}
```
