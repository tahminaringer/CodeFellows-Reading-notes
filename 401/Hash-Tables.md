# Hash Tables

## Terminology

- **Hash** - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
  - is the ability to encode the key that will eventually map to a specific location in the data structure and easily retrieve the value
- **Buckets** - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
- **Collisions** - A collision is what happens when more than one key gets hashed to the same location of the hashtable.
  - solved by changing the initial state of the bucket and initializing a LinkedList in each one and key-value pairs can be stored as a node.

- **Why use hash table** Hold unique values and act as a dictionay or library
- Each node/bucket has a key and a value(key value pair)

- **Hash Maps** 
  - **Store value**
    - accept a key
    - calculate the hash of the key
    - use modulus to convert the hash into an array index
    - store the key with the value by appending both to the end of a linked list
  - **Read a Value**
    - accept a key
    - calculate the hash of the key
    - use modulus to convert the hash into an array index
    - use the array index to access the short LinkedList representing a bucket
    - search through the bucket looking for a node with a key/value pair that matches the key you were given

- **Internal Methods**
  - `Add()`
  - `Find()`
  - `Contains()`
  - `GetHash()`