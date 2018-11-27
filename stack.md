# Stack

A stack is a data structure built on an underlying container such as a list or vector that operates in a last-in first-out basis, elements that are inserted can only come out from one end of the underlying container.

## In Memory

A stack in memory looks like this: \[TO DO\]

## Operations

A stack is capable of:

* **Push:** Insert an element on top of the stack.
    * This operation is O(1) as it operates the same as append or push_back for a list/vector.
* **Pop:** Remove the top element of the stack and return it.
    * This operation is also O(1) as it operates the same as pop/pop_back for a list/vector.

## Use Cases

A stack is useful in niche scenarios when you need to store data in a LIFO fashion, such as saving a state a running program is in.

A stack is not useful when you need more functionality than a stack provides, such as accessing elements underneath the top of the stack.

## Examples

In Python:

```python
#Instantiation
example_stack = Stack()

#Push a value on to the stack
example_stack.push(20)

#Pop the top value off the stack and return it
print(example_stack.pop())
```

In C++:

```C++
//Instantiation
stack<int> exampleStack;

//Push a value on to the stack
exampleStack.push(20)

//Pop the top value off the stack and return it
print(exampleStack.pop())
```
