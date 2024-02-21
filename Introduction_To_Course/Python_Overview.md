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


# Working with Dates and Time
```python
import datetime as dt
import time as tm
import datetime as dt
import time as tm
#time returns the current time in seconds since the Epoch. (January 1st, 1970)

tm.time()
#Convert the timestamp to datetime.

dtnow = dt.datetime.fromtimestamp(tm.time())
dtnow
#Handy datetime attributes:

dtnow.year, dtnow.month, dtnow.day, dtnow.hour, dtnow.minute, dtnow.second  # get year, month, day, etc.from a datetime
#timedelta is a duration expressing the difference between two dates.

delta = dt.timedelta(days=100)  # create a timedelta of 100 days
delta
date.today returns the current local date.

today = dt.date.today()
today - delta  # the date 100 days ago
today > today - delta  # compare dates
today > today - delta  # compare dates
```
## Importing Modules

First, import the necessary modules:

```python
import datetime as dt
import time as tm
```

## Getting Current Time

```python
tm.time()
```

This function call returns the current time in seconds since the Epoch (January 1st, 1970).

## Converting Timestamp to datetime

```python
dtnow = dt.datetime.fromtimestamp(tm.time())
```

This converts the timestamp to a datetime object.

## Accessing datetime Attributes

```python
dtnow.year, dtnow.month, dtnow.day, dtnow.hour, dtnow.minute, dtnow.second
```

These lines demonstrate accessing various attributes of the datetime object.

## Creating a Timedelta Object

```python
delta = dt.timedelta(days=100)
```
This creates a timedelta object representing a duration of 100 days.

## Getting Today's Date

```python
today = dt.date.today()
```

This retrieves the current local date.

## Performing Date Arithmetic

```python
today - delta  # the date 100 days ago
```

Subtracting delta from today gives the date 100 days ago.

## Comparing Dates

```python
today > today - delta  # compare dates
```

This line compares today's date with the date 100 days ago using the greater than operator.

This guide provides a basic overview of handling dates and times in Python using the datetime module.

