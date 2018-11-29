# Deque

A deque (double ended queue) is a queue that can add and remove items from both ends of the queue rather than just the front.

## In Memory

In memory, a deque looks like: \[TO DO\]

## Operations

A deque is capable of:

* **Enqueue (Front/Back):** Add an item to either the front of the deque or the back.
    * This operation is O(1). An explanation as to why queue operations are O(1) is found [here](queue.md).
* **Dequeue (Front/Back):** Remove an item from either the front of the deque or the back.
    * This operation is O(1) as well.

## Use Cases

A deque is useful when utilizing multiple queues at once, when one queue is moving through its contents faster than another, then you can remove items from the back of a queue to another. Deques can also be used for storing time sensitive data, such as undo history or web browser history (more recent data enters the front, and older data leaves through the back).

A deque is not so useful when you need to access data inbetween the front and the back.

## Examples

```python
#Instantiation
example_deque = Deque()

#Adding to the front
example_deque.enqueueFront(5)

#Adding to the back
example_deque.enqueueBack(10)

#Removing from the front
example_deque.dequeueFront()

#Removing from the back
example_deque.dequeueBack()
```
