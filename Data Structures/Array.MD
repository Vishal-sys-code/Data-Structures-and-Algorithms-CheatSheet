# Arrays

![array](/images/array.png)

An array is a collection of items stored at contiguos memory location

### Important facts:
* Stores elements sequentially, one after another.
* Each array element has an index. Zero-based indexing is used most often: the first index is 0, the second is 1, and so on.
* Is created with a fixed size. Increasing or decreasing the size of an array is impossible.
* Can be one-dimensional (linear) or multi-dimensional.
* Allocates contiguous memory space for all its elements.

### Pros
* Ensures constant time access by index.
* Constant time append (insertion at the end of an array).

### Cons:
* Fixed size that can't be changed.
* Search, insertion and deletion are O(n). After insertion or deletion, all subsequent elements are moved one index further.
* Can be memory intensive when capacity is underused.

## Time complexity (worst case):
* Access: ```O(1)```
* Search: ```O(n)```
* Insertion: ```O(n)``` (append: ```O(1)```)
* Deletion: ```O(n)```

<hr>

# Dynamic Arrays

An array that can resize itself.

**Also known as**: array list, list, growable array, resizable array, mutable array, dynamic table.

### **Important facts:**
* Same as array in most regards: stores elements sequentially, uses numeric indexing, allocates contiguous memory space.
* Expands as you add more elements. Doesn't require setting initial capacity.
* When it exhausts capacity, a dynamic array allocates a new contiguous memory space that is double the previous capacity, and copies all values to the new location.
* Time complexity is the same as for a fixed array except for worst-case appends: when capacity needs to be doubled, append is O(n). However, the average append is still O(1).

**Pros:**
* Variable size. A dynamic array expands as needed.
* Constant time access.

**Cons:**
* Slow worst-case appends: O(n). Average appends: O(1).
* Insertion and deletion are still slow because subsequent elements must be moved a single index further. Worst-case (insertion into/deletion from the first index, a.k.a. prepending) for both is O(n).

## Time complexity (worst case):
* Access: ```O(1)```
* Search: ```O(n)```
* Insertion: ```O(n)``` (append: ```O(1)```)
* Deletion: ```O(n)```

<hr>