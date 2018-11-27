# Tuple

A tuple is a fixed, ordered collection of data that is immutable. A tuple's elements and size cannot be changed.

## In Memory

In memory a tuple looks like this: \[TO DO\]

## Operations

Because of its immutability, tuples are rather limited but they are capable of:

* **Retrieval / Access:** Return a value at the specified index.
    * This operation is O(1) or constant time. Since a tuple variable is a pointer to the base memory address of the array and we know the size of each object stored, the address of an object is just one calculation away (base address + sizeOf(datatype) * index).


## Use Cases

A tuple is useful when you do not want anything to change the elements or size of a container.

A tuple is not very useful when you want to change elements or insert new data.

## Examples

In Python:

```python
#Instantiation
example_tuple = (1, 2, 3, 4, 5, 6)

#Access
print(example_tuple[2])
```
