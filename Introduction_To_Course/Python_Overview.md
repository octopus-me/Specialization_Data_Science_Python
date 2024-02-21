# Python Data Structures Overview

This guide provides an overview of Python's fundamental data structures: lists, tuples, sets, and dictionaries. Understanding these data structures is crucial for effective data manipulation and algorithm development in Python.

## Lists

Lists are ordered collections of items (which can be of different types) and are one of the most versatile data structures in Python. They can be modified after their creation (mutable), allowing for operations like adding, removing, or changing items.

### Features:
- **Ordered:** The items have a defined order, and that order will not change.
- **Mutable:** You can change, add, and remove items in a list after it has been created.
- **Allow duplicates:** Since lists are indexed, they can have items with the same value.

### Example:
```python
my_list = [1, "Hello", 3.14]
print(my_list)
```

## Tuples

Tuples are similar to lists, but they are immutable, meaning they cannot be changed after creation. They are used to store collection of items in specific order.

### Features:
- **Ordered:** The items have a defined order, and that order will not change.
- **Immutable:** Once a tuple is created, you cannot change, add, or remove items.
- **Allow duplicates:** Tuples can also have items with the same value.

### Example:
```python
my_tuple = (1, "Hello", 3.14)
print(my_tuple)
```

## Dictionaries

Dictionaries store pairs of items as key-values pairs. They are unordered collection, where each key is unique.

### Features

- **Unordered:** They are collections where items do not have a defined order.
- **Mutable:** You can chance, add, and remove pairs.
- **Keys are unique:** No two pairsr can have the same key.

  ## Example:

  ```python
  my_dict = {'name':'John', 'age':30}
  print(my_dict)
  ```


## Sets

Sets are unordered collections of unique items. They are mutable and useful for performing mathematical set operations like unions, intersection difference, and summetric difference.

### Features:

- **Unordered:** The items do not have a defined order, and their order can change.
- **Mutable:** You can add or remove items from a set.
- **No duplicates:** Sets cannot have two items with the same value.

## Example:

```python
my_set = {1,2,3,4,5}
print(my_set)
```
