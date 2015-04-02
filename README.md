# Chord-implementation
*Each terminal represents a node


This project contains two executable files: chord, query

In chord, I implemented a chord and realized the function Join and Kill:
   To create the first node in the chord insert format like: ./chord 8001
   To Join an existing chord insert format like: ./chord 8002 127.0.0.1 8001
   To read the status of a node(IP, port, predecessor, successor) type "print" in stdin.
   To kill a node(node exit abruptly) type "kill" in stdin.

   You could use "print" to see the updated node info after a while
   The searches in the chord are through fingertable

* after Join and Kill, please wait a moment for the chord to adjust.
* Do not Kill or Join too quickly.

In query, I realized the function Search:
   To search a file in the chord(you need to execute the chord first) from a specific node(127.0.0.1, 8001) insert the format like: ./query 127.0.0.1 8001
   To search the successor of a file(a string as a file name) type the name of the file in stdin. And the successor will be printed out.
   To exit type "quit" in stdin.
   If the specific node is not in the chord, "Not Found" will be printed out.

The IPs in this project are all 127.0.0.1 
