Q1. What is hashing?<br>
Hashing is a technique used for storing, retrieving and removing information as quick as possible.<br>
It is a process of converting a arbitrary size key into fixed size value, this conversion is done via special function called Hash Function.<br>
The operation supported by hashing such as storing, retrieving and removing information and have average runtime complexity of O(1).<br>

Q2. What are Hash Function?<br>
A hash function simply takes an arbitrary size key and provides fixed size value also called as index.<br>

Q3. What is Moular Hash Function?<br>
A modular hash function takes a key and size and returns a remainder by dividing key by size.<br>
The remainder is used as an index to store the key in an array of provided size.<br>

index = key % size;<br>
![Screenshot (279)](https://user-images.githubusercontent.com/35030513/184872105-576f380b-26e2-49e8-a4df-1bb7554c9ba0.png)<br>

Q4. What is Hash Table?<br>
It is a generalized form of an array.<br>
It stores the data in form of key-value pair.<br>
It converts key to an index using hash function.<br>
Taking the index we store key-value in array.<br>
The primary operations supported by hashtable are : <br>
	1) put(key, value) : Adds key-value pair against unique key.<br>
	2) get(key) : Get value for the provided key.<br>
	3) remove(key) : Removes the key-value pair fro hashtable.<br>
Average running time is O(1).<br>

Java Collections Framework has HashMap class and HashSet class.<br>
HashMap class : if we want to deal with key-value pair.<br>
HashSet class : if we want to deal with only keys.<br>
![Screenshot (283)](https://user-images.githubusercontent.com/35030513/184873216-688cbcbe-a309-4c49-843b-6a2a69edba14.png)<br>

Q5. What is Collision? <br>
The situation where a newly inserted key, maps to an already occupied slot in the hash table is called collision.<br>
![Screenshot (281)](https://user-images.githubusercontent.com/35030513/184872726-4985a0da-81dd-4697-a3eb-a70b1ba4c780.png)<br>

How to handle Collisions? <br>
There are mainly two methods to handle collision:<br>
1) Separate Chaining : using HashNode. <br>
![Screenshot (282)](https://user-images.githubusercontent.com/35030513/184872614-da009785-f27b-4298-9c8d-961d5012ad07.png)<br>
2) Open Addressing

Q6. What is HashNode?<br>
A HashNode class in HashTable consist of three data members: <br>
1) K key : It is a unique value which help in storing data.<br>
2) V value : It is the data that is stored based on location computed by key.<br>
3) HashNode next : It refers to the next HashNode in chain of hash nodes.<br>
![Screenshot (278)](https://user-images.githubusercontent.com/35030513/184872756-cce793ea-73d1-4e68-bc0c-799e87750b8b.png)<br>


