# Array

An array (in this case, a dynamic array like a vector in C++ or a list in Python), is an ordered collection of data.

## In Memory

In memory, an array looks like this: \[TO DO\]

## Operations

An array is capable of:

* **Retrieval/Access:** Return a value at the specified index.
    * This operation is O(1) or constant time. Since an array variable is a pointer to the base memory address of the array and we know the size of each object stored, the address of an object is just one calculation away (base address + sizeOf(datatype) * index).
* **Append/Push_Back:** Insert a new object at the end of the array.
    * This operation is also O(1) or constant. At the cost of keeping track of the last index in the array, append becomes constant time as no objects need to be moved in the array to make room for a new object.
* **Pop/Pop_Back:** Remove the object located at the end of the array and return it.
    * This operation is the same as appending, it just deletes the object instead of adding an object.
* **Insert:** Insert an object at the specified index.
    * This operation is O(n) or linear. Since objects in an array must be moved over to make room for the object you're inserting, 'n' objects must be moved over, where 'n' is the size of the list minus the index.
* **Delete:** Delete an object at the specified index.
    * This operation is the same as inserting, but instead of moving objects forward, they must be moved backwards to fill the new empty space.

## Use Cases

An array is useful when you want the convenience of instant retrieval/access and know exactly where an object is located in the array.
