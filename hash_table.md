# Hash Table

A hash table is a collection of items which are stored in a way that is easy to find them later (key:value pairs). Hash tables initially contain no items and each slot gets filled as items get mapped to their respective slots through something called a hash function.

## In Memory

In memory, a hash table looks like:

## Operations

A hash table is capable of:

* **Access:** Access or retrieve an item in the table according to its key.
    * The complexity of hash table operations can vary greatly depending on the implementation, but on average access is O(1) due to how the hashing function works. Sending a key through the hash function should return the location of the item it is associated with and is one operation.
* **Insert:** Add a new item to the hash table.
    * This operation has the same complexity as access.
* **Delete:** Delete an item in the hash table.
    * This operation also has the same complexity as access.

## Use Cases

Hash tables are useful when you want instant insertion, retrieval, and removal, and do not care for the order that a list provides or the uniquity of sets.

Hash tables are not so useful when you need your data ordered like it would be in a list.

## Examples

```python
#Instantiation
hash_table = HashTable()

#Insertion
hash_table.insert("Example_Key", "Example_Value")

#Access
hash_table.get("Example_Key")

#Deletion
hash_table.delete("Example_Key")
```
