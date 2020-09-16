# Read: 04 - Linked Lists


[README](/README.md)

Information from [What’s a Linked List, Anyway?](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)
Linked list are part a type of data structure. they are linear in type. 
- linear data structure -- there is a sequence and an order to how they are constructed and traversed. 
- I really liked the analogy of linear data structur as being liek hopscoth, in that you are unable to reach the end without going through each step. The below diagram really drove home the point for me.

![](img/Linear-vs-nonlinear-struct.png)


The reason linked list are important is that they spread out the memory usage. Linke d lists can store information in a manner that does not need to be right next to eachother. 
- This is a type of dynamic data structure -- which do not need a set amount of memory to be allocated in order to exist. Its size and shape can change as can the amount of memory in needs.



Linked lists are made up of a series of nodes. They start with the head, and and with a null node. 
- a node itself is made up of 2 parts: the data that iut holds, a reference to the next nod. 
- "a node only knows about what data it contains, and who its neighbor is." It also does not know how long the list is. This is why linked lists are able to grow and srink dynamically and why they are important for data allocation.

