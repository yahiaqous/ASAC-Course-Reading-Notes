# Hash Tables

## What is a Hashtable?

**Hashtables are a data structure** that utilizes key-value pairs. This means every Node or Bucket has both a key and a value.

The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value. This is done through what we call a hash.

- **Hash** - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

- **Buckets** - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

- **Collisions** - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

Hashing is implemented in two steps:

- An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.

- The element is stored in the hash table where it can be quickly retrieved using a hashed key.

## Why do we use them?

- **Hold unique values**
- **Dictionary**
- **Library**

Hash maps take advantage of an array’s **O(1)** read access. Instead of adding elements to an array from beginning to end, a hash map uses a “hash function” to place each item at a precise index location, based on its key.

A **collision** occurs when more than one key hashes to the same index in an array. A “perfect hash” will never have any collisions.

Collisions are solved by changing the initial state of the buckets. Instead of starting them all as null, we can initialize a LinkedList in each one! Now if two keys resolve to the same index in the array then their key/value pairs can be stored as a node in a linked list. Each index in the array is called a “bucket” because it can store multiple key/value pairs.

Hash maps do this to store values:

- **Accept a key**
- **Calculate the hash of the key**
- **Use modulus to convert the hash into an array index**
- **Store the key with the value by appending both to the end of a linked list**

Hash maps do this to read value:

- **Accept a key**
- **Calculate the hash of the key**
- **Use modulus to convert the hash into an array index**
- **Use the array index to access the short LinkedList representing a bucket**
- **Search through the bucket looking for a node with a key/value pair that matches the key you were given**

## Internal Methods

- **_Add()_**
- **_Find()_**
- **_Contains()_**
- **_GetHash()_**
