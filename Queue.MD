# Queue

![Queue](/images/queue.png)

A Queue is a linear structure which follows a particular order in which the operations are performed. _The order is First In First Out (FIFO)._ <br>

**Important facts:**

* Modeled after a real-life queue: first come, first served.
* First in, first out (FIFO) data structure.
* Similar to a linked list, the first (last added) node is called the tail, and the last (next to be removed) node is called the head.
* Two fundamental operations are enqueuing and dequeuing:
    * To enqueue, insert at the tail of the linked list.
    * To dequeue, remove at the head of the linked list.
* Usually implemented on top of linked lists because they're optimized for insertion and deletion, which are used to enqueue and dequeue elements.

**Pros:**
* Constant-time insertion and deletion.

**Cons:**
* Access and search are O(n).

**Notable uses:**

* CPU and disk scheduling, interrupt handling and buffering.

**Time complexity (worst case):**
* Access: ```O(n)```
* Search: ```O(n)```
* Insertion (enqueuing): ```O(1)```
* Deletion (dequeuing): ```O(1)```

**Implementation in Java :**
```
Queue<­E> queue = new Linked­List();
```
_Here E is the type of the object_.

<hr>

**Basic Operations on Queue:**

* **void enqueue(int data)**: Inserts an element at the end of the queue i.e. at the rear end.
* **int dequeue()**: This operation removes and returns an element that is at the front end of the queue.

**Auxiliary Operations on Queue:**

* **int front()**: This operation returns the element at the front end without removing it.
* **int rear()**: This operation returns the element at the rear end without removing it.
* **int isEmpty()**: This operation indicates whether the queue is empty or not.
* **int size()**: This operation returns the size of the queue i.e. the total number of elements it contains.  

<hr>

| Operations           |   Complexity  |
|----------------------|---------------|
| Enque(insertion)     |      O(1)     |
| Deque(deletion)      |     O(1)      |
| Front(Get front)     |      O(1)     |
| Rear(Get Rear)       |     O(1)      |

<hr>
