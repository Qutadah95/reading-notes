# Hash Tables

## What is a Hashtable?

Terminology:


1. Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. 
2. Buckets - A bucket is what is contained in each index of the array of the hashtable. 
3. Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.



## Why do we use them?

1. Hold unique values
2. Dictionary
3. Library

## What Are they ?

Hashtables are a data structure that utilize key value pairs.

## Structure

* Hashing

* Creating a Hash

* Collisions


## Internal Methods

* Add
* Find
* Contains
* GetHash

## Basics of Hash Tables


Hashing is a technique that is used to uniquely identify a specific object from a group of similar objects.

Hashing is implemented in two steps:

1. An element is converted into an integer by using a hash function.
2. The element is stored in the hash table where it can be quickly retrieved using hashed key.

## Hash function


A hash function is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table.

To achieve a good hashing mechanism, It is important to have a good hash function with the following basic requirements:

* Easy to compute: It should be easy to compute and must not become an algorithm in itself.

* Uniform distribution: It should provide a uniform distribution across the hash table and should not result in clustering.

* Less collisions: Collisions occur when pairs of elements are mapped to the same hash value.




