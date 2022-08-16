Q1. What is hashing?<br>
Hashing is a technique used for storing, retrieving and removing information as quick as possible.<br>
It is a process of converting a arbitrary size key into fixed size value, this conversion is done via special function called Hash Function.<br>
The operation supported by hashing such as storing, retrieving and removing information and have average runtime complexity of O(1).<br>

Q2. What are Hash Function?<br>
A hash function simply takes an arbitrary size key and provides fixed size value also called as index.<br>

Q3. What is Moular Hash Function?<br>
A modular hash function takes a key and size and returns a remainder by dividing key by size.<br>
The remainder is used as an index to store the key in an array of provided size.<br>

index = key % size;

Q4. What is Hash Table?<br>
It is a generalized form of an array.<br>
It stores the data in form of key-value pair.<br>
It converts key to an index using hash function.<br>
Taking the index we store key-value in array.<br>
The primary operations supported by hashtable are -<br>
	put(key, value) : Adds key-value pair against unique key.<br>
	get(key) : Get value for the provided key.<br>
	remove(key) : Removes the key-value pair fro hashtable.<br>
Average running time is O(1).<br>

Java Collections Framework has HashMap class and HashSet class.<br>
HashMap class : if we want to deal with key-value pair.<br>
HashSet class : if we want to deal with only keys.<br>

Q5. What is Collision? <br>
The situation where a newly inserted key, maps to an already occupied slot in the hash table is called collision.<br>

How to handle Collisions? <br>
There are mainly two methods to handle collision:<br>
1) Separate Chaining : using HashNode. <br>
2) Open Addressing

Q6. What is HashNode?<br>
A HashNode class in HashTable consist of three data members:<br>
	K key : It is a unique value which help in storing data.<br>
	V value : It is the data that is stored based on location computed by key.<br>
	HashNode next : It refers to the next HashNode in chain of hash nodes.<br>

