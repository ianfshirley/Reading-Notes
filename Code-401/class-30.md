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

**Creating a Hash**
A hashtable is traditionally created from an array. 


### What is a Hash Table? ~(video)~

- 

### Basics of Hash Tables

- 

### Hash Table Wiki

- 


### Sources

[Intro to Hash Tables]()<br>
[What is a Hash Table?]()<br>
[Basics of Hash Tables]()<br>
[Hash Table Wiki]()<br>