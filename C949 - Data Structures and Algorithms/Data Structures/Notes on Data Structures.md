# General  Notes
- A **Data Structure** is a way of organizing, storing, and performing operations on data.
	- Operations performed on a data structure include
		- *Accessing or updating stored data*
		- *Searching for specific data*
		- *Inserting new data*
		- *Removing data*
The following provides a list of basic data structures:
![[Pasted image 20250522204229.png]]

# [[1. Lists]]
## **Definition & Overview**
A **list** is an **abstract data type (ADT)** that represents a **finite, ordered collection of elements** where duplicates are allowed.
- Elements can be accessed, inserted, or removed at any position in the list.
- Lists are **linear**—there’s a first element, a last element, and a clear sequence in between.
- The **abstract** part means we care about _what_ lists do, not _how_ they’re implemented.
**Common operations on a List ADT:**
- Insert (add) an element
- Remove (delete) an element
- Retrieve (access) an element
- Update (change) an element
- Search (find) for an element
- Determine the size (length)
- Check if empty or full
> **Important:** In Python, the built-in `list` is a _concrete_ implementation of the list ADT.
## **Key Concepts & Properties**
- **Order Matters:** The position of each element is meaningful (`list[0]` is not `list[1]`).
- **Duplicates Allowed:** The same value can appear more than once.
- **Dynamic Size:** Lists can grow and shrink.
- **Indexing:** Each element has an index; Python uses zero-based indexing.
- **Mutability:** Lists in Python can be modified after creation (unlike tuples).
- **Homogeneous vs. Heterogeneous:** Lists can store any data type (even mixed types), but in practice, most lists are homogeneous for consistency and safety.
**List ADT ≠ Array:**
- The list ADT is a theoretical concept.
- Arrays are a _way to implement_ the list ADT (other ways include linked lists, etc.).
- Lists focus on _behavior_; arrays focus on _structure_.
## Python Examples
- #### Creating Lists
```python
# Empty list
my_list = []

# List with elements
numbers = [10, 20, 30, 40]

# Mixed data types
mixed = [1, "hello", 3.14, True]
```
- #### Accessing Lists
```python
print(numbers[0])  # 10
print(numbers[-1]) # 40 (last element)
```
- #### Adding Elements
```python
numbers.append(50)      # [10, 20, 30, 40, 50]
numbers.insert(2, 25)   # [10, 20, 25, 30, 40, 50]
```
- #### Removing Elements
```python
numbers.pop()       # Removes and returns last item (50)
numbers.remove(25)  # Removes the first occurrence of 25
```
- #### Updating Elements
```python
numbers[0] = 5      # Changes first item to 5
```
- #### Searching
```python
if 30 in numbers:
    print("30 is in the list")
```
- #### Length
```python
len(numbers)        # Number of elements in list
```
- #### Iterating
```python
for num in numbers:
    print(num)
```
## Best Practices and Formatting
- **Use Descriptive Variable Names**:
```python
user_ids = [101, 102, 103]
```
- **Prefer list comprehension for generating/modifying lists**:
```python
squares = [x**2 for x in range(10)]
```
- **Avoid modifying a list while iterating over it which can lead to unexpected behavior
## Connections to other topics:
- **Linked Lists:** Another way to implement the List ADT, with different performance tradeoffs.
- **Stacks & Queues:** Specialized types of lists with restricted access patterns. 
- **Array vs. List:** Arrays have fixed size and type; Python lists are dynamic.
- **Big O Analysis:** Performance of list operations depends on the underlying implementation (array, linked list, etc.).
- **Recursion & Lists:** Lists are often used as parameters or return values in recursive algorithms.
# [[2. Stacks and Queues]]

# [[3. Hash Tables]]
# [[4. Trees]]
# [[5. Balanced Trees]]
# [[6. Heaps and Treaps]]
# [[7. Sets]]
# [[8. Graphs]]
# [[9. B-Trees]]


