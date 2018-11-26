# Array

An array (in this case, a dynamic array like a vector in C++ or a list in Python), is an ordered collection of data.

## In Memory

In memory, an array looks like this: \[TO DO\]

## Operations

An array is capable of:

* **Retrieval/Access:** Return a value at the specified index.
    * This operation is O(1) or constant time. Since an array variable is a pointer to the base memory address of the array and we know the size of each object stored, the address of an object is just one calculation away (base address + sizeOf(datatype) * index).
