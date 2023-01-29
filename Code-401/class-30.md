## Hash Tables

### Intro to Hash Tables

1. Hash - a has is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array
2. Buckets - a bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could peotentially contain multiple key/value pairs if a collision occurs.
3. Collisions - a collision is what happens when more than one key gets hashed to the same location of the hashtable

- Hashtables are a data structure that use key/value pairs. This means every Node or Bucket has both a key and a value.
- The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value. This is done through what we call a hash. A hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.
- Since we are able to hash our key and determine the exact location where our value is stored, we can do a lookup in an O(1) time complexity. 
  - In any array, we could access the information of any element in the array if we already know the index, but usually we don't know the index and thus have to loop through each element in the array to find what we're looking for, which greatly decreases efficiency.
- Instead of adding elements to an array from beginning to end, a hash map uses a 'hash function' to place each item at a precise index location, based off its key.
- The hash function essentially takes a key and returns an integer. We use that integer to determine where the key/value pair should be placed in the array. The hash code is calculated in constant time and writing to an array at one index is O(1), so the hash map has O(1) access.
- The hash code is used again to read something from the hash map. Take the key, and run it through the hash code to get a number, and use that number to index the array. Calculating the hash code and reading an array at that index is all constant time, so the hash map has O(1) read access.

**Creating a Hash Table**
A hashtable is traditionally created from an array. 1024 is a good length to minimize collisions.

- Create an empty list to hold the hashtable:
  `table = [None] * 1024`
- Create the hash function:
  1. add or multiply all the ASCII values 
  2. mutliply that total by a prime number such as 599
  3. use modulo to get the remainder of the result, when divided by the length of the array.
  4. insert into the array at that index

  Example:
![hash-func-ex.](img/hash-func-example.png)

- Collisions:
  - If two keys resolved to the same index, the two calls to `.Add(key, val` with different keys would overwrite each other.
  - This can be solved by changing the initial state of the buckets. Instead of starting them all as null/None, we can initialize a `LinkedList` in each one. Now if two keys resolve to the same index in the array, their key/value pairs can each be stored as separate nodes in a linked list.
  - Since different keys can lead to the same bucket, it's important to store the entire key/value pair in the bucket, not just the value.

- Hash maps do this to store values:
  - accept a key
  - calculate the hash of the key
  - use modulus to convert the hash into an array index
  - store the key with the value by appending both to the end of a linked list
- Hash maps do this to read values:
  - accept a key
  - calculate the hash of the key
  - use modulus to convert the has into an array index
  - use the array index to access the LinkedList representing the bucket matching that index
  - search through the bucket looking for a node with a key/value pair that matches the key you were given

**Methods**
- `set()`
  - When adding a new key/value pair to a hashtable:
    1. send the key to the `hash()` method
    2. once you determine the index of where it should be placed, go to that index
    3. check if something exists at that index already, if not, add the key/value pair at that index
    4. if something already exists at that index, add the new key/value pair to the data structure within that bucket (add it to the end of the linked list)
- `get()`
  - takes in a key, gets the hash, goes to the index specified. Iterate through the bucket at that index, see if the key exists, and return the value
- `has()`
  - accepts a key, and returns a bool whether or not that key exists inside the hashtable. The best way to do this is to have this method call the `hash()` method and check if the given key can be found at the index returned by the `hash()` method.
- `keys()`
  - returns an array of unique hash keys
- `hash()`
  - accepts a key as a string, conducts the hash, and then returns the index of the array where the key/value pair should be placed.

**Using Python's built-in dict() class**
```
# create an empty hash table
table = dict()

# insert key-value pairs into the table
table["key1"] = "value1"
table["key2"] = "value2"
table["key3"] = "value3"

# retrieve values from the table using their keys
print(table["key1"]) # prints "value1"
print(table["key2"]) # prints "value2"
print(table["key3"]) # prints "value3"

# update the value of an existing key
table["key1"] = "new_value1"

# check if a key is in the table
if "key1" in table:
    print("key1 is in the table")

# remove a key-value pair from the table
del table["key1"]

# check the lenght of the dict
print(len(table))
```
- Dicts are dynamic and automatically resize themselves as needed to accomodate new key-value pairs
- You can also use the `get()` method to retrieve the value of a key without raising an error if the key is not found in the dict, you can also pass a default value to return if the key is not present:
  `value = table.get("key1", "default_value")`
- Dicts also have useful methods like `items()`, `keys()`, and `values()` to iterate through keys, values or both:
  ```
  for key in table.keys():
    print(key)

  for value in table.values():
    print(value)
    
  for key, value in table.items():
    print(key, value)

  ```

### What is a Hash Table? *(video)*

- One way to deal with collisions is to create a linked list at the index and "chain" the elements together that get mapped to the same index

### Basics of Hash Tables

- Hashing is implemented in two steps:
  1. An element is converted into an integer using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
  2. The element is stored in the hash table where it can be quickly retrieved using the hashed key
    hash = hashfunc(key)
    index = hash % array_size
  - In this method, the hash is independent of the array size and then it is reduced to an index (a number between 0 and array_size - 1) by using the modulo operator (%)

- A Hash function is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table. The values returned by a hash function are called hash values, hash codes, hash sums, or simply hashes.
- A good hash function must meet the following requirements:
  1. Easy to compute: it should be easy to compute and must not become an algorithm in itself
  2. Uniform distribution: it should provide uniform distribution across the hash table and should not result in clustering
  3. Less collisions: try to avoid multiple elements getting mapped to the same hash value


### Sources

[Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)<br>
[What is a Hash Table?](https://www.youtube.com/watch?v=MfhjkfocRR0)<br>
[Basics of Hash Tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)<br>
[Hash Table Wiki](https://en.wikipedia.org/wiki/Hash_table)<br>
[The Oracle](https://chat.openai.com/chat)