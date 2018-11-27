# Array

An array is a fixed, ordered collection of data. When an array is instantiated its size must be declared and it cannot be changed, but contents of the array can be modified.

## In Memory

In memory, an array looks like this: \[TO DO\]

## Operations

An array is capable of:

* **Retrieval / Access:** Return a value at the specified index.
    * This operation is O(1) or constant time. Since an array variable is a pointer to the base memory address of the array and we know the size of each object stored, the address of an object is just one calculation away (base address + sizeOf(datatype) * index).

## Use Cases

An array is useful when you know exactly how much space you need, want the convenience of instant retrieval/access and know exactly where an object is located in the array (otherwise you would have to iterate through the entire array to find what you want).

Arrays are not so useful when you are continuously adding data as arrays cannot change their size, and when you don't know what's inside the array.

## Examples

In Python:

```python
# Instantiation
example_array = [1, 2, 3, 4]

# Instant access
print(example_array[2])

# Value changing
example_array[2] = 10
```

In C/C++:

```C++
// Instantiation
int exampleArray[] = {1, 2, 3, 4, 5}

// Instant access
print(exampleArray[2])

// Value changing
exampleArray[2] = 10
```

