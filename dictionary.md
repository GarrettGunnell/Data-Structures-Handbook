# Dictionary

A dictionary is an unordered, non-sequential, collection of data that is composed of key-value pairs. This means that each element of the dictionary has a key that's associated with a particular value (written as key:value).

## In Memory

In memory a dictionary looks like: \[TO DO\]

## Operations

A dictionary is capable of:

* **Add:** Add an element to the dictionary.
    * The average complexity of this operation is O(1) as dictionaries are functionally hash tables, adding an item to the dictionary is constant. If the hashing function is really, really bad, then the complexity can degenerate become O(n).
* **Get:** Get an element from the dictionary by key, if it exists.
    * The complexity of this operation, like adding, is also O(1) due to the properties of hash tables.
* **Remove:** Delete an element in the dictionary.
    * Deletion is also O(1) like add and get, but can also degenerate to O(n).
* **In:** Check whether or not the dictionary contains a particular item.
    * Just like add, delete, and get, this operation is also O(1).


## Use Cases

Dictionaries are useful when you want instant insertion, retrieval, and removal, and do not care for the order that a list provides or the uniquity of sets.

Dictionaries are not so useful when you need your data ordered like it would be in a list.

## Examples

```python
#Instantiation
example_dictionary = {'example':20, 'value':30}

#Adding an item to the dictionary
example_dictionary['new'] = 40

#Getting an item
print(example_dictionary['example'])

#Removing an item
del example_dictionary['new']

#In
print('example' in example_dictionary)
```
