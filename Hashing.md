Q1. What is hashing?<br>
Hashing is a technique used for storing, retrieving and removing information as quick as possible.
It is a process of converting a arbitrary size key into fixed size value, this conversion is done via special function called Hash Function.
The operation supported by hashing such as storing, retrieving and removing information and have average runtime complexity of O(1).

Q2. What are Hash Function?<br>
A hash function simply takes an arbitrary size key and provides fixed size value also called as index.

Q3. What is Moular Hash Function?<br>
A modular hash function takes a key and size and returns a remainder by dividing key by size.
The remainder is used as an index to store the key in an array of provided size.

index = key % size;

Q4. What is Hash Table?<br>
It is a generalized form of an array.
It stores the data in form of key-value pair.
It converts key to an index using hash function.
Taking the index we store key-value in array.
The primary operations supported by hashtable are -
	put(key, value) : Adds key-value pair against unique key.
	get(key) : Get value for the provided key.
	remove(key) : Removes the key-value pair fro hashtable.
Average running time is O(1).

Java Collections Framework has HashMap class and HashSet class.
HashMap class : if we want to deal with key-value pair.
HashSet class : if we want to deal with only keys.

Q5. What is Collision? <br>
The situation where a newly inserted key, maps to an already occupied slot in the hash table is called collision.

How to handle Collisions? 
There are mainly two methods to handle collision:
1) Separate Chaining : using HashNode. 
2) Open Addressing

Q6. What is HashNode?
A HashNode class in HashTable consist of three data members:
	K key : It is a unique value which help in storing data.
	V value : It is the data that is stored based on location computed by key.
	HashNode next : It refers to the next HashNode in chain of hash nodes.

