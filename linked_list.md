# Linked List

A linked list is an unordered collection of data composed of nodes that contain data and a pointer to the next node. Linked lists are the basis of many different data structures.

## In Memory

In memory, a linked list looks like: \[TO DO\]

## Operations

A linked list is capable of:

* **Search:** Search the list for a node, if it exists.
    * This operation is O(n) where 'n' is the number of nodes in the list.
* **Insert:** Insert a node into the list.
    * This operation is (technically) O(1), all you need to do is change the pointers of the nodes in the list. If you do not know where the end of the location of insertion then you must search for it, which is O(n).
* **Delete:** Delete a node in the list.
    * This operation has the same complexity of insertion.

## Use Cases

Linked lists are useful when rapid insertion and deletion is occurring as this can be costly with other data structures.

Linked lists are not so useful when you need quick access of data in the list.

## Examples

In Python:

```python
#Instantiation
example_linkedlist = LinkedList()

#Insertion
example_linkedlist.insert(20)

#Search
example_linkedlist.find(20)

#Deletion
example_linkedlist.delete(example_linkedlist.find(20))
```


# Circular Doubly Linked List

A more "advanced" implementation of linked list that, at the cost of more data usage, makes certain operations O(1). In this implementation, each node keeps track of the node behind it in addition to the next node, this allows for the head of the list to point to the tail and vice versa.

## In Memory

In memory, a circular doubly linked list looks like: \[TO DO\]

## Operations

A circular doubly linked list has all of the same operations as a linked list, but insertion at the tail becomes instant since the head of the list points to the tail (allowing for append and pop operations).
