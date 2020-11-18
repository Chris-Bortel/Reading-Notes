## Reading: Hash Tables

### Why use them

- Hash tables are cool because they can store data on two different levels, both horizontally and vertically. They are an array of linked lists that are organized by key in order to grab the keys associated value
- They are super fast and have a 0(1) time complexity

### What are they

- They are data structures that use key value pairs.
- They are composed of nodes also known as buckets
- We hash the key which sends the item to the the exact location using the index.

### How do we do it

- We hash the key into an integer, and that determines the index of the objects
- If there is another object with the same key, then we are going to move onto the next node. This is just building a linked list vertically from the array that is horizontal
