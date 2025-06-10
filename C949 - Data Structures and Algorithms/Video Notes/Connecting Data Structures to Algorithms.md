##### What is an algorithm?
- A well defined , step by step procedure or set of rules for solving a problem or accomplishing a specific task
	- its a sequence of instructions that a computer can execute to achieve a desired outcome
	- Think of it like a recipe for solving a problem
---
##### What is a Data Structure?
- A specific way of organizing and storing data
- Allows for efficient access, manipulation and retrieval of information
- Different data structures are designed for different operations
---
##### Data Structures / ADT Examples
- Array
- Stack
- Queue
- Linked List
- Tree
- Graph
---
##### Relation to Algorithms
- Implementation:
	- Implemented using code that interacts with data structures to perform operations on data
- Efficiency:
	- A good data structure can enable an algorithm to operate quickly and efficiently on large data sets
- Problem Solving:
	- The right data structure for a specific problem is crucial for designing an efficient algorithm to solve it
---
##### Comparison of: Array & Linked List
- Array:
	- Ordered and indexed collection of elements
	- Fixed size (python)
	- Stored in contiguous memory locations
	- Used when we require random access to elements; when insertion and deletion are infrequent
	- O(N)
- Linked List:
	- Linear data structure consisting of nodes and pointers
	- Used when the number of elements is not known in advance
	- Used in cases when faster insertion and deletion are required
	- O(1)
---
##### Trade-offs in Data Structure Selection
- Time-Complexity:
	- Fast Access vs. Slow Modification (Arrays vs Linked Lists)
- Space-Complexity:
	- Memory usage considerations (Hash Tables vs Binary Trees)
- Ease of Use:
	- Simplicity vs. Flexibility (Arrays vs Heaps)
**Example:**
- Using a Hash Table for frequent look-ups reduces time complexity to O(1) but increases space complexity due to extra memory allocation
---
