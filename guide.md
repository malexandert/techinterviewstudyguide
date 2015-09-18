# The Technical Interview Study Guide

## **Data Structures**
### Arrays
```python
a = [1,2,3] # Python
```
```java
int[] a = [1,2,3]; // Java
```
```
val a: Array[Int] = Array(1,2,3) // Scala
```
- Stores data elements sequentially based on an index (usually starts at 0)
- ***Static arrays*** are fixed in size from creation, while ***dynamic arrays*** can have their sizes change based on the number of elements in them currently
- Element access and insertion (assuming there is still space) in static arrays is  _O_(1). In dynamic arrays, access is _O_(1), but insertion is _O_(n). Search is _O_(n) with linear search, and _O_(log _n_) with binary search.
- **Note**: the Python "list" structure has properties of a linked list, a dynamic array, and a stack/queue

### Linked List
```python
a = [1,2,3] # Python
```
```java
LinkedList<Integer> a = new LinkedList<Integer>(); // Java
```
- Stores data in ***nodes*** that are then appended (or prepended, in the functional sense) to the list
	- Every node has reference only to the data inside it and what the next node in the list is
- List sizes are dynamic, but insertion remains _O_(1). Search is _O_(n).
- Variations in linked lists
	* **Doubly-Linked Lists**: A linked list where each node has a pointer to both the next node and the previous node
	* **Circular Linked Lists**: A linked list with a "cycle", or  a node that has a pointer to a previous node in the list
	  - The **tortoise and hare algorithm** for finding cycles in linked lists: Create two pointers,  one "tortoise" and one "hare". Make the tortoise move along the list one node at a time, and make the hare move two nodes at a time. If the tortoise and the hare are ever on the same node (before the end null), then the list has a cycle. 

