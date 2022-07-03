# Stack

![Stack](/images/stack.png)

Stack is a linear data structure which follows a particular order in which the operations are performed. _The order may be LIFO(Last In First Out) or FILO(First In Last Out)._ <br>

**Important facts:**

* First-in, last-out (FILO) data structure.
* Equivalent of a real-life pile of papers on desk.
* In stack terms, to insert is to push, and to remove is to pop.
* Often implemented on top of a linked list where the head is used for both insertion and removal. Can also be implemented using dynamic arrays.

**Pros:**
* Fast insertions and deletions: O(1).

**Cons:**
* Access and search are O(n).

**Notable uses:**
* Maintaining undo history.
* Tracking execution of program functions via a call stack.
* Reversing order of items.

**Time complexity (worst case):**

* Access: ```O(n)```
* Search: ```O(n)```
* Insertion (pushing): ```O(1)```
* Deletion (popping): ```O(1)```

**Implementation in Java :**
```
Stack<E> stack = new Stack<E>();
```
_Here E is the type of the object_.