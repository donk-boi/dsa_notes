##### Linear vs. Binary Search
- **Linear Search** is an algorithm that starts from the beginning of a list and checks each element until the search key is found or the end of the list is reached
	- It works on **sorted** and **unsorted data**
- Binary Search starts in the **middle**, if that is not the correct result, the search repeats on the remaining left or right sub-list depending on if the middle element was greater than or less than the request. The process repeats until the number is found or until all searching is exhausted
	- It only works on **sorted** data
	- It uses the **divide and conquer** approach
---
##### Why and How to Sort Data
- Unsorted data must rely on linear search to find data
	- Not suitable for large data sets 
	- time consuming O(N)
- Sorted data has many algorithms available for searching
	- Scalable for large data sets
	- Faster average time O(logN)
- Sorting:
	- The process of converting a list of elements into ascending or descending order, such as arranging papers in alphabetical order or envelopes by ascending zip codes
	- Various methods exist for sorting data some which are more efficient than others
	- This includes
		- Bubble Sort
		- Selection Sort
		- Quick Sort
		- Merge Sort
		- Radix Sort
---
##### Bubble Sort
- **Bubble Sort:**
	- A sorting algorithm that iterates through a list, comparing and swapping adjacent elements if the second element is less than the first element
	- Each iteration moves the largest element into sorted position
		- Because of the nested loops, bubble sort has a runtime of **O(N^2)**
		- Bubble sort is often considered impractical for real-world use because many faster sorting algorithms exist
---
##### Selection Sort
- **Selection sort:**
	- A sorting algorithm that treats the input as two parts, a sorted part and an unsorted part.
	- It repeatedly finds the lowest value and swaps it with the current element being examined moving it from the unsorted part to the end of the sorted part
		- Selection sort includes nested loops and has a runtime of **O(N^2)**
---
##### Insertion Sort
- **Insertion Sort:**
	- A sorting algorithm that treats the input as two parts, sorted and unsorted
	- It repeatedly moves the next value from the unsorted part to the sorted part where it is then move into the proper location
		- Insertion sort includes nested loops (for and while) which makes its runtime **O(N^2)**
---
##### Quick Sort
- **Quick Sort:**
	- Repeatedly partitions the input into low and high parts (each part unsorted) and then recursively sorts each of those parts
	- To partition the input, quick sort chooses a pivot to divide the data into low and high parts
		- The **Pivot** can be any value within the array being sorted
	- Once the pivot is chosen, the array is divided into two parts
	- Items to the left are less than the pivot while items to the right are greater
	- The values in each partition are not necessarily sorted
	- Values equal to the pivot may appear in either or both of the partitions
		- Has a runtime of **O(NlogN)**
---
##### Merge Sort 
- **Merge Sort:**
	- A sorting algorithm that divides a list into two halves, recursively sorts each half, and then merges the sorted halves to produce a sorted list
	- The recursive partitioning continues until a list of one element is reached as a list of one element is already sorted
		- Has a runtime of **O(NlogN)**
---
##### Radix Sort
- **Radix Sort:**
	- A sorting algorithm designed specifically for integers
	- The algorithm makes use of a concept called buckets and is a type of bucket sort
	- Any array of integer values can be sub-divided into buckets by using the integer value's digits
	- A bucket is a collection of integer values that all share a particular digit value
		- Has a runtime of **O(n)
---