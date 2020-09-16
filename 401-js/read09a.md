# Read 9a: Stacks & Queues

[README](/README.md)

## [Stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html) --- what is a stack


- Data structure that is made up of nodes that each reference the next node in the stack but does not reference the previous node

Terms to remember"
- Push -- The ways the we put the Nodes or items into the stack
- Pop -- The way that Nodes or items are removed from the stack... They are popped. When we attempt to pop an empty stack. am exception will be raised
- Top -- this is the top of the stack 
- Peek -- when you peek, you view  the value of the top node. If you peek an empty stack, an exception will be raised
- IsEmpty -- returns true when the stack is empty, otherwise it will return false



### Remember these concepts
- FILO --- First In Last Out --- MEans that the first item added in the stack will be the last item to be popped out of the stack

- LIFO -- Last In First Out --- means that the last item added to the stack will be the first to be popped out of the stack



when you have a stack, it is O(1) because it takes as much memory to do any of the operations

when pushing, the node being added, is reassigned as the top of the stack and the original is pushed down. You need to assign the node being added to the top the property of the node below it.

Pop O(1)
- when popping, the top node is popped off and the next node is reassigned as the new top. The node that was popped off will be returned to the user. 
- when doing this, check for isEmpty, this will make sure that no exceptions are raised. Could also use the a try/catch block
- when using pop :
  1. create a reference named temp that points to the current node on top 
  2. reassign top to the value that the next property is referencing. 
  3. remove the initial 'top. node with out affecting the rest if the stack. We want to remember to clear out the next prop in current temp ref

Peek O(1)
- let you inspect the top Node of the stack
  - first check isEmpty in order to not raise an exception
IsEmpty O(1)
- do not re-assign the next property when we peek because we want to keep the reference to the next Node in the stack.

IsEmpty
- checks to see if stack is empty




What is a Queue