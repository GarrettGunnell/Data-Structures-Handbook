# Array

An array(in this case, a dynamic array like a vector in C + + or a list in Python), is an ordered collection of data.

## In Memory

In memory, an array looks like this: \[TO DO\]

## Operations

An array is capable of:

* **Retrieval / Access:** Return a value at the specified index.
    * This operation is O(1) or constant time. Since an array variable is a pointer to the base memory address of the array and we know the size of each object stored, the address of an object is just one calculation away(base address + sizeOf(datatype) * index).
* **Append / Push_Back:** Insert a new object at the end of the array.
    * This operation is also O(1) or constant. At the cost of keeping track of the last index in the array, append becomes constant time as no objects need to be moved in the array to make room for a new object.
* **Pop / Pop_Back:** Remove the object located at the end of the array and return it.
    * This operation is the same as appending, it just deletes the object instead of adding an object.
* **Insert:** Insert an object at the specified index.
    * This operation is O(n) or linear. Since objects in an array must be moved over to make room for the object you're inserting, 'n' objects must be moved over, where 'n' is the size of the list minus the index.
* **Delete:** Delete an object at the specified index.
    * This operation is the same as inserting, but instead of moving objects forward, they must be moved backwards to fill the new empty space.
* **Index/Find:** Find an object in the array and return the index.
    * This operation is O(n) or linear. The find operation compares elements in the array until a match is found.

## Use Cases

An array is useful when you want the convenience of instant retrieval / access and know exactly where an object is located in the array.

Arrays are not so useful when you need to regularly insert and delete data(not at the end) as it can be costly when arrays are very large.

## Examples

In Python:

```python
#Instantiation
example_array = [1, 2, 3, 4]

#Adds 5 to the end of the array
example_array.append(5)

#Removes 5 from the end of the array
example_array.pop()

#Inserts a string at index 2
example_array.insert(2, "INSERT_DATA")

#Removes the string at index 2
del example_array[2]

#Prints 0 which is the index of 1
print(example_array.index(1))
```

In C++:

```C++
//Instantiation
vector<int> exampleVector = {1, 2, 3, 4};

//Adds 5 to the end of the vector
exampleVector.push_back(5);

//Removes 5 from the end of the vector
exampleVector.pop_back(5);

//Insert 0 at front
auto it = exampleVector.begin(); //Create iterator pointing to desired index
exampleVector.insert(it, 0);

//Removes 0 from the front
exampleVector.erase(myvector.begin());
```
