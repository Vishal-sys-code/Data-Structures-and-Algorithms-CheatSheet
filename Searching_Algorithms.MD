# Searching Algorithms

## **Binary Search**

| Algorithm | Time  | Space  |
| :-----: | :-:   | :-:      |
| Binary Search | O(log(n))   | O(1)  |

**_Binary Search (Recursive):_**

```
public int binarySearch(int search, int[] array, int start, int end) {
   int middle = start + ((end - start) / 2);
   if(end < start) {
      return -1;
   } 

   if (search == array[middle]) {
      return middle; 
   } else if (search < array[middle]) {
      return binarySearch(search, array, start, middle - 1);
   } else {
      return binarySearch(search, array, middle + 1, end);
   }
}
```

**_Binary Search (Iterative):_**

```
public int binarySearch(int target, int[] array) {
   int start = 0;
   int end = array.length - 1;
   while (start <= end) {
      int middle = start + ((end - start) / 2);
      if (target == array[middle]) {
          return target;
      } else if (search < array[middle]) {
          end = middle - 1;
      } else {
          start = middle + 1;
      }
   }
   return -1;
}
```