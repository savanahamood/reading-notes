# Hash Tables

### What is a Hashtable?
A hash table, also known as a hash map, is a data structure that provides efficient insertion, deletion, and retrieval of key-value pairs. It is designed to quickly locate a value associated with a given key. Hash tables are widely used in computer science and programming because of their ability to provide constant-time average complexity for these operations, making them very efficient for managing large amounts of data.

The core concept behind a hash table involves using a hash function to convert the input key into an index within an array. This index is then used to store or retrieve the associated value. Hash functions take an input (such as a string or a number) and produce a fixed-size value (usually an integer), which serves as the index. The goal of a good hash function is to distribute keys evenly across the available array indices to minimize collisions (when multiple keys map to the same index).

### Why do we use them?
* Hold unique values
* Dictionary
* Library

### Hash tables offer the following advantages:

* Fast Data Retrieval: Hash tables provide constant-time average complexity for retrieval, insertion, and deletion operations. This makes them efficient for managing large datasets.

* Flexible Key Types: Hash tables can work with a wide range of key types, including strings, numbers, and objects.

* Key-Value Association: They establish a direct relationship between keys and values, making it easy to store and retrieve data based on meaningful identifiers.

* Dynamic Sizing: Many hash table implementations automatically resize themselves as the number of key-value pairs grows, ensuring efficient usage of memory.

### hash tables also have some limitations:

* Hash Collisions: Since hash functions map keys to finite indices, it's possible for two different keys to map to the same index. This situation is known as a collision and needs to be handled properly to maintain correct functionality.

* Space Complexity: Hash tables can consume a significant amount of memory, especially if the load factor (ratio of items to slots) is high.

* Hash Function Selection: Choosing an appropriate hash function is crucial. A poor hash function could lead to poor distribution of keys and a higher chance of collisions.



### Resources:
 [Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

[what is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0)

[basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)

[hash table wiki](https://en.wikipedia.org/wiki/Hash_table)
