# List / Vector

A list (or a vector in C++) is a dynamic array that is capable of adjusting its size as more data is added to it.

## In Memory

In memory a list or vector looks like this: \[TO DO\]

## Operations

A list or vector is capable of:

* **Retrieval / Access:** Return a value at the specified index.
    * This operation is O(1) or constant time. Since a list/vector variable is a pointer to the base memory address of the list/vector and we know the size of each object stored, the address of an object is just one calculation away (base address + sizeOf(datatype) * index).
* **Append / Push_Back:** Insert a new object at the end of the list/vector.
    * This operation is also O(1) or constant. At the cost of keeping track of the last index in the list/vector, append becomes instant as no objects need to be moved in the array to make room for a new object and you don't need to find the end.
* **Pop / Pop_Back:** Remove the object located at the end of the list/vector and return it.
    * This operation is the same as appending, it just deletes the object instead of adding an object.
* **Insert:** Insert an object at the specified index.
    * This operation is O(n) or linear. Since objects in a list/vector must be moved over to make room for the object you're inserting, 'n' objects must be moved over, where 'n' is the size of the list/vector minus the index.
* **Delete:** Delete an object at the specified index.
    * This operation is the same as inserting, but instead of moving objects forward, they must be moved backwards to fill the new empty space.
* **Index/Find:** Find an object in the list and return the index.
    * This operation is O(n) or linear. The find operation compares elements in the array until a match is found and in the worst case you need to make 'n' comparisons where 'n' is the size of the list.

## Use Cases

Lists/vectors are useful when you want instant retrieval of elements, know where things are, and are only appending/popping elements.

Lists/vectors are not very useful when you need your elements sorted, are inserting and deleting inside the list/vector, and are unsure where most elements of the list/vector are indexed.

## Examples

In Python:

```python
#Instantiation
example_list = [1, 2, 3, 4]

#Adds 5 to the end of the list
example_list.append(5)

#Removes 5 from the end of the list
example_list.pop()

#Inserts a string at index 2
example_list.insert(2, "INSERT_DATA")

#Removes the string at index 2
del example_list[2]

#Prints 0 which is the index of 1
print(example_list.index(1))
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
