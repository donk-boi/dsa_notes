##### Binary Search Tree
- A BST is a special binary Tree
- Left Child node is <= parent
- Right Child node is >= parent
- Enables fast searching for an item
	- **O(logN)**
- see also [[2. Binary Search]], [[Trees, Heaps, and Hashtables]], [[4. Trees]], [[5. Balanced Trees]]
---
##### Special Binary Trees
- **Full** - every node contains 0 or 2 children
- **Complete** - all levels, except possibly the last level contain all possible nodes and all nodes in the last level are as far left as possible
- **Perfect** - all internal nodes have 2 children and all leaf nodes are at the same level
	- **internal node** is a node with at least one child
	- a **leaf node** is a node without a child
	- **ancestors** are parents of a node and their parents and so on until the root
---
##### BST - Skewed is the Problem
- A Skewed tree that only goes in one direction and while it could be a valid tree and meet all the requirements to still be a tree, it could have all the internal nodes go in a single direction which eventually becomes a **linear search** as opposed to a **BST**
##### AVL: A Balanced Tree
- A **BST** with a *height-balance property* and specific operations to re-balance when inserting or removing
- Nodes **balance factor** is the left sub-tree's height minus the right sub-tree's height
- Balanced nodes have a value from -1 to 1
- A tree (or sub-tree) with just one node has **a height of 0**
- Minimizing binary tree height yields fastest searches, insertions, and removals
- The height begins at the node being examined and goes to the farthest/deepest node
- An AVL can store the sub-tree height as a member of each node
##### Altering the AVL Tree
- Insertions and deletions are performed the same way as a standard BST
- However if an AVL height violations occurs, rotations take place to balance
---
##### Red-Black Trees
- Self-balancing by either doing rotations or recoloring the nodes
- Each node is either Red or Black. Every nodes stores one extra bit for color
	- i.e. 0 denotes black, 1 denotes red 
- The root node and leaves (NIL) are always black
- Red nodes cannot have red children (i.e. no consecutive reds)
- Every path from node to NIL descendants have same number black nodes 
- New nodes begin as red
##### Red-Black Operations
- Searching - No change from standard BST
- Insert - May require rotations
- Deletion - May require rotations
- All of these operations occur at **O(logN)**
##### Comparison: AVL vs. Red-Black Trees
- AVL:
	- More balanced requiring more rotations especially for a large tree
	- Fast search (AVL tree **guarantees O(logN) time**)
	- More complex rotations
- Red-Black Trees
	- Red-Black are less balanced, require less rotations (maximum of 2)
	- Require more searching? Use AVL
	- Faster insertions and deletions
	- O(logN) *average* time for searching
	- Fewer rotations
---
