### See also: [[Abstract Data Types]], [[Abstract Data Type (ADT)]], [[Algorithm(s)]], [[7. Lists and Dictionaries]], [[2. Stacks and Queues]], [[7. Sets]]
- An Abstract Data Type is a data type described by predefined user operations without explanation
	- "insert data at rear" or "add to front"
- Example: A list is a common ADT for holding ordered data
	- operations include append, remove, search, and print
- Commonly implemented using arrays or linked lists data structures
---
- Abstraction means to have a user interact with an item at a high-level with lower-level internal details hidden from the user
- ADTs support abstraction by hiding the underlying implementation details and providing a well-defined set of operations
- ADTs enable programmers to focus on higher-level operations and algorithms, improving programmer efficiency
---
- ADT Data Structures:
	- **Lists**: An ADT for holding data that utilize **arrays** and **linked lists** as underlying data structures
		- Common ADT for holding ordered data and having operations
		- List index beings a 0
		- Python commands include Append, Insert, InsertAfter, Search, Length, Sort, Print
	- **Dynamic Array**: An ADT for holding ordered data and allowing indexed access and utilize the **array** as an underlying data structure
		- Array based list will dynamically allocate the array 
		- The **prepend** operation for an array based list inserts a new item at the start of the list
		- Given the index of an item in an array-based list the **remove-at**operation removes the item at that index
			- When removing an item at index X each item after X is moved down by 1 position
	- **Stack**: An ADT in which items are only inserted or removed from the **top** that uses the underlying data structure **linked list**
		- Operations included push, pop, and peak
		- A stack is last-in-first-out (LIFO) ADT
	- **Queue**: An ADT in which items are inserted at the end of a queue and removed from the front of the queue and uses a **linked list** as an underlying data structure
		- Insert to the end, removed from the front first-in-first-out (FIFO) ADT
		- Operations include enqueue and dequeue
		- Like your spotify queue or waiting in line at a store
	- **Deque**: Pronounced as "deck" can be inserted and removed from both the front and the back and the push-front operation inserts an item at the front and a push-back operation inserts an item at the back. Uses a **linked list** as an underlying data structure
		- operations include PushFront, PushBack, PopFront, PopBack, PeekFront, PeekBack, IsEmpty, and GetLength
		- Stands for a "**Double-Ended Queue**"
	- **Set**: A set is for an unordered collection of **NON-Duplicate** items that uses a binary search tree and hash table as the underlying data structures. Its a collection of distinct elements 
		- Set Add operation adds an element
	- **Bag**: Similar to a set but uses **Arrays and Linked Lists** as underlying data structures and they **DO** allow duplicate items
		- Common operations for both include find, insert, and remove
	- **Priority Queue**: A queue where each item has a priority and items with higher priority are closer to the front of the queue than items with lower priority and uses **Heaps** as underlying data structures
		- Enqueue operation inserts an item such that the item is closer to the front than all items of lower priority **does not mean higher number**
		- Dequeue operation removes an returns the item at the front of the queue which has the highest priority
	- **Dictionary**: Associates or maps keys with values and uses **hash tables and binary search trees as underlying data structures** they contain references to objects as key-value pairs
		- Each key is associated with a value much like each word in dictionary stating a definition
		- operations include `my_dict[key]`, `my_dict[key] = value`, `del my_dict[key]`, `key in my_dict`
---
