Python Core Data Structures: Dictionaries, Sets, Tuples, and Lists
Welcome to the Python Core Data Structures guide! This repository contains explanations, code examples, and best practices for working with Python's built-in data structures: Dictionaries, Sets, Tuples, and Lists.

Table of Contents
Introduction
Lists
Tuples
Sets
Dictionaries
Examples
Contributing
License
Introduction
Python offers powerful, built-in data structures that can be used to organize, store, and manipulate data efficiently. This repository provides an overview of Lists, Tuples, Sets, and Dictionaries, each of which serves unique purposes and offers specific advantages. Understanding these structures will help you write more efficient, readable, and effective Python code.

Lists
Lists are ordered, mutable sequences that can store a variety of data types. Lists are defined with square brackets [] and allow for duplicate elements. Lists are versatile and used in various applications where the order and mutability of data matter.

Basic Syntax
my_list = [1, 2, 3, "apple", 4.5]
Key Methods
append(): Adds an item to the end of the list.

my_list = [1, 2, 3]
my_list.append(4)
print(my_list)  # Output: [1, 2, 3, 4]
remove(): Removes the first occurrence of a specified element.


my_list = [1, 2, 3, 2]
my_list.remove(2)
print(my_list)  # Output: [1, 3, 2]
sort(): Sorts the list in ascending (default) or descending order.


my_list = [3, 1, 4, 2]
my_list.sort()
print(my_list)  # Output: [1, 2, 3, 4]
pop(): Removes and returns the item at the specified index (or last if none is specified).


my_list = [1, 2, 3, 4]
my_list.pop(2)
print(my_list)  # Output: [1, 2, 4]

Tuples
Tuples are ordered, immutable sequences, making them suitable for storing fixed collections of items. Tuples are defined with parentheses () and are faster than lists due to their immutability.

Basic Syntax
my_tuple = (1, 2, 3, "banana", 5.7)

Key Characteristics
Immutable: Once created, the items in a tuple cannot be modified.
Ordered: Supports indexing and slicing.
Used in cases where data should not change, such as configuration settings or fixed records.

Sets
Sets are unordered collections of unique elements, making them ideal for membership testing and removing duplicates. Sets are defined with curly braces {} or by using the set() function.

Basic Syntax
my_set = {1, 2, 3, "apple"}

Key Methods
add(): Adds an element to the set.

my_set = {1, 2, 3}
my_set.add(4)
print(my_set)  # Output: {1, 2, 3, 4}
remove(): Removes a specified element from the set.

my_set = {1, 2, 3}
my_set.remove(2)
print(my_set)  # Output: {1, 3}
union(): Returns a set containing all unique elements from both sets.

set1 = {1, 2, 3}
set2 = {3, 4, 5}
union_set = set1.union(set2)
print(union_set)  # Output: {1, 2, 3, 4, 5}
intersection(): Returns a set containing elements that are common to both sets.

set1 = {1, 2, 3}
set2 = {2, 3, 4}
intersection_set = set1.intersection(set2)
print(intersection_set)  # Output: {2, 3}

Important Notes
Sets are unordered and mutable.
Sets do not allow duplicates and are commonly used for operations like union, intersection, and difference.


Dictionaries
Dictionaries are collections of key-value pairs, allowing you to store and retrieve data by unique keys. Dictionaries are defined with curly braces {} and a colon : separates keys and values.

Basic Syntax
my_dict = {"name": "Alice", "age": 25, "city": "New York"}
Key Methods
get(): Returns the value of a specified key.

my_dict = {"name": "Alice", "age": 25}
print(my_dict.get("name"))  # Output: Alice
keys(): Returns a list of dictionary keys.


my_dict = {"name": "Alice", "age": 25}
print(my_dict.keys())  # Output: dict_keys(['name', 'age'])
values(): Returns a list of dictionary values.


my_dict = {"name": "Alice", "age": 25}
print(my_dict.values())  # Output: dict_values(['Alice', 25])
items(): Returns a list of tuples, each containing a key-value pair.

my_dict = {"name": "Alice", "age": 25}
print(my_dict.items())  # Output: dict_items([('name', 'Alice'), ('age', 25)])
update(): Updates the dictionary with another dictionary’s key-value pairs.


my_dict = {"name": "Alice", "age": 25}
new_info = {"city": "New York"}
my_dict.update(new_info)
print(my_dict)  # Output: {"name": "Alice", "age": 25, "city": "New York"}

Key Characteristics
Mutable: You can change, add, or remove key-value pairs.
Keys: Must be unique and are typically immutable types (e.g., strings, numbers, or tuples).
Values: Can be of any data type, and duplicates are allowed.
Examples
Here are a few example scripts for each data structure.

List Example
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")
print(fruits)  # Output: ["apple", "banana", "cherry", "orange"]

Tuple Example
coordinates = (10.0, 20.0)
# Attempting to modify will raise an error
# coordinates[0] = 15.0  # Raises TypeError
print(coordinates)  # Output: (10.0, 20.0)

Set Example
unique_numbers = {1, 2, 3, 4, 4}
print(unique_numbers)  # Output: {1, 2, 3, 4}


Dictionary Example
person = {"name": "John", "age": 30}
person["city"] = "New York"
print(person)  # Output: {"name": "John", "age": 30, "city": "New York"}


Contributing
Contributions are welcome! If you have improvements, examples, or explanations that could benefit others, please feel free to open a pull request or raise an issue.

License
This project is licensed under the MIT License. See the LICENSE file for details.
Happy Coding!
