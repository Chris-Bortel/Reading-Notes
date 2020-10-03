# Read 9b: 9-29-2020

[README](/README.md)

## Trees (Binary and Binary Search Trees)

#### Terminology

- Node -- Individual item/data that makes of the data structure

- Root: The first/top Node in the tree

- Left Child: Position the the left of the root or node

- Right Child: Position the the left of the root or node

- Edge: The link that is between a parent and a child node

- Leaf: A nde that does not contain any children

- Height: Determined by the number of edges from the root to the bottommost node ???? What ????

### Traversals

#### Depth First

Multiple ways to carry out depth first traversal --- each method changes the order in witch we search/print the

root. **Recursion** : This is the way that is most common to traverse through a tree --- This relies on the call stack to

navigate back up the tree when we have reached the end of a sub-path

**Pre-order**: root >> left >> right]

- `root` need to be looked at first --> This means the output value

- When preOrder is called for the first time, the root will be added top the call stack

- NEXT: read the preOrder function's code from top to bottom

- In order: left >> root >> right

- Post-order: left >> right >> root
