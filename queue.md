# Queue

A queue is a structure built on an underlying container of ordered items (dependent on implementation) that operates in a first-in first-out basis. Items added to the queue are added to the back of the line, while removal only happens from the front of the line.

## In Memory

In memory, a queue looks like:

![Image of Queue in Memory](images/queue.png)


## Operations

A queue is capable of:

* **Enqueue:** Add an item to the queue.
    * Enqueueing an item is O(1) or constant, the reasoning can differ depending on implementation. For a linked list implementation, the queue will maintain a pointer to the back of the queue which makes enqueue instant.
* **Dequeue:** Remove an item from the queue.
    * Dequeuing an item is also O(1) like enqueue, for the same reasons.

## Use Cases

Queues, like stacks, are useful in niche scenarios where you want your data to be handled in a specific manner. Queues can be used to handle processes in the order in which they come up.

Queues are not so useful when you require more functionality than a queue provides.

## Examples

In Python:

```python
#Instantiation
example_queue = Queue()

#Enqueue
example_queue.enqueue(5)

#Dequeue
print(example_queue.dequeue())
```
