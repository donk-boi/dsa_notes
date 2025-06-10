##### Trees
- Many types of trees
	- File Structures
	- Binary Trees
	- etc
- Unique properties for each
- Binary Trees
	- Heaps
- Binary Search Trees
---
##### Binary Tree Basics
- Each node has up to two children known as left and right children
- Root is the "top" node of the tree
- Internal node is a node with at least one child
- Leaf node is a node with children
- Parent node is a node that is the "parent" to a child node
	- Ancestors include the nodes parent and that parents parent and so on
##### Depth Level and Height of Trees
- The link from a node to a child is called an **edge**
- A nodes **depth** is the number of edges on the path from the root to the node
	- The Root node has a ***depth of 0***
- All nodes with the same depth from a tree **level**
- A tree's **height** is the larges depth of any node
	- A tree with just one node has a ***height of 0***
---
##### Special Binary Trees
- A binary tree is *full* if every node contains **either 0 or 2 children**
- A binary tree is *complete* if all levels except possibly the last level contain all possible nodes and all nodes in the last level are as far left as possible
- A binary tree if *perfect* if all internal nodes have **2 children** and **all leaf nodes are at the same level**
---
##### Binary Search Trees
- In a Binary Search Tree (often referred to as a **BST**) has an ordering property that any node's left subtree keys <= the node's key , and the right subtree's keys >= the node's key
	- Left nodes will be less than or equal to root/parent
	- Right nodes will be greater than or equal to root/parent
##### BST Searching
- Searching a BST in the worst case requires H + 1 comparisons meaning O(H) comparisons where H is equal to the tree's height
- A BST search may be as small as O(logN) 
	- Example: A 10,000 node list may require only 14 comparisons
- Height can be minimized by keeping all levels full (**Balanced**) except possibly the last level
##### BST In-Order Traversal
- A tree traversal algorithm visits all nodes in the tree once and performs an operation on each node
- An in-order traversal visits all nodes in a BST from smallest to largest which is useful for example to print the trees nodes in a sorted order
- Starting from the root the algorithm recursively prints the left subtree, the current node, and then the right subtree
---
##### Heaps
- Some applications require fast access to and removal of the maximum item in a changing set of items: i.e. Priority Queue
- Heaps keep the highest priority on top but does not full sort the lower nodes
- A max-heap is a compete binary tree that maintains the simple property that a nodes key is greater than or equal to the nodes children keys
- Therefore a max-heaps root always has the maximum key in the entire tree
##### Heapification
- The process in which an array or binary tree is reshaped into a heap data structure known as heapification
- Since leaf nodes already satisfy the max heap property, heapifying to build a max-heap is achieved be percolating down on every non-leaf node in reverse order
- A heap must be a complete binary tree
##### Max-Heap Insert and Remove
- An **insert** starts by inserting the node in the tree's last level and then swapping the node with its parent until no max-heap property violation occurs
	- Inserts fill a level (left to right) before adding another level so the trees height is always the minimum possible
	- The upward movement of a node in a max-heap is called percolating
- A **remove** is always a removal of the root by replacing it with last level's last node and swapping that node with its greatest child until no max-heap violation occurs
##### Heapsort Overview 
- Heapify the array into a max-heap
- Initialize an end index value to the size of array minus 1
- Repeatedly remove the maximum value, stores at the end index
- Decrement end index
- Repeat until the end index is 0
---
##### Hash Tables
- Stores unordered items by mapping or hashing each item to a location in an array
- Each element is a bucket
- In a hash table, an item's **key** is the value used to map to an index
- Keys are ideally unique
- A **hash function** computes a bucket index from the items key
##### Calculating the Hash Value
- A common hash function used the modulo operator (%) which computes the integer remainder when dividing two numbers
- see example in [[Data Structures]]
##### Hash Tables - Collisions
- Collisions occur when an item being inserted into a hash table maps to the same bucket as an existing item in the hash table 
- Chaining - each bucket has a list of items
- Probing - looks for an empty bucket elsewhere in the table
- Empty-Since-Start Bucket - has been empty since the hash table was created 
- Empty-After-Removal Bucket - had an item removed that cause the bucket to now be empty
---
