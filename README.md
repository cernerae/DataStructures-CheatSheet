# DataStructures-CheatSheet

Data Structures everyone should know

- [DataStructures-CheatSheet](#datastructures-cheatsheet)
- [Linked List](#linked-list)
- [Array](#array)
- [Hash Table](#hash-table)
- [Stack and Queue](#stack-and-queue)
  * [Stack](#stack)
  * [Queue](#queue)
- [Graphs and Trees](#graphs-and-trees)
  * [Graphs](#graphs)
  * [Trees](#trees)
    + [Binary Search Tree (BST)](#binary-search-tree--bst-)

<hr />

# Linked List

- Contains **VALUE** and **POINTER**

```
x, y are of type ListNode. NOT in an Array

Ex: [x, ..., y]

-- Head node is "x"
---- Head node's "next" points to next Node
-- Tail node is "y"
---- Tail node's "next" points to null
```

**PROS**: Good at adding new nodes and deleting nodes  
**CONS**: Retrieval

# Array

- Continuous block of cells in computer memory side-by-side

**PROS**: Retrieval  
**CONS**: Adding elements, Searching

# Hash Table

- Uses hashing functions to store in memory
- Blocks of memory don't have to be next to each other, can be stored anywhere

**PROS**: Retrieval, Adding/Removing keys  
**CONS**: Collisions

# Stack and Queue

## Stack

- Last IN / First OUT
- **push(n)** IN, then **pop()** OFF the TOP
- Every language keeps track of the functions that have been called with a **call stack**.
- Important for Depth-first search (DFS)

## Queue

- First IN / First OUT (like a real-life queue)
- Adding an item to the end is called **enqueue-ing** and removing it from the front is called **dequeue-ing**
- Used for Breadth-first search (BFS)

**PROS**: efficient to add & remove  
**CONS**: limited use cases

# Graphs and Trees

## Graphs

- ["Graph Theory"](https://en.wikipedia.org/wiki/Graph_theory)
- Similar to linked list, where we have **NODES** pointing to other **NODES**. Except in this case, the pointers are called **EDGES**.
- Edges can also have **WEIGHTS** assigned to them
- Example: Two cities can be NODES, while the distance between them is an EDGE
- Example: Social media networks can/are stored as graphs in order to facilitate complex user relationships

<img src="https://miro.medium.com/max/1292/1*Jjd7qTNuFL9bKT4qpMRWLA.png" height="200" />

## Trees

- A special kind of hierarchical graph called a **TREE**, in which the data expands out in ONE DIRECTION.
- Example: like an HTML tree with nexted elements:

```
<div id="parent">
  <p id="child1">Hello</p>
  <p id="child2">World</p>
</div>
```

### Binary Search Tree (BST)

- Has specific rules that let us do efficient searching
- Rules
    1. 0, 1, or 2 children (left or right, or both)
    2. Left Child Node < Parent Node
    3. Right Child Node > Parent Node
- We can traverse through a tree and always know where an element is

<img src="https://media.geeksforgeeks.org/wp-content/cdn-uploads/binary-tree-to-DLL.png" height="200" />

- BST is not the perfect data structure
    - If you add elements in a weird order, it can get very "one-sided" (or imbalanced)
- However, self-balancing trees exist (these are advanced data structures):
    - [Red-black Tree](https://en.wikipedia.org/wiki/Red%E2%80%93black_tree)
    - [B-Trees](https://www.cpp.edu/~ftang/courses/CS241/notes/b-tree.htm#:~:text=A%20B%2Dtree%20is%20a,in%20database%20and%20file%20systems.)
