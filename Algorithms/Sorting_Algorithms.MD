# Sorting Algorithms

| Algorithms  | Best  | Average  | Space  |
|---|---|---|---|
| Bubble Sort  | O(n)  | O(n^2)  | O(1)  |
| Insertion Sort  | O(n)  | O(n^2)  | O(1) |
| Selection Sort  | O(n^2)  | O(n^2)  |  O(1) |
| Quick Sort  | O(nlog(n))  | O(nlog(n))  | O(log(n))  |
| Heap Sort  | O(nlog(n))  | O(nlog(n))  |  O(1) |
| Merge Sort | O(nlog(n))  | O(nlog(n))  | O(n)  |



<br>

## **Merge Sort**

```
private void mergesort(int low, int high) {
         if (low < high) {
                 int middle = low + (high - low) / 2;
                 mergesort(low, middle);
                 mergesort(middle + 1, high);
                 merge(low, middle, high);
           }
 }

private void merge(int low, int middle, int high) {
          for (int i = low; i <= high; i++) {
                 helper[i] = numbers[i];
         }
          int i = low;
         int j = middle + 1;
         int k = low;
         while (i <= middle && j <= high) {
               if (helper[i] <= helper[j]) {
                     numbers[k] = helper[i];
                    i++;
              } else {
                     numbers[k] = helper[j];
                     j++;
               }
               k++;
         }
         while (i <= middle) {
               numbers[k] = helper[i];
               k++;
                i++;
          }
     }
```

## **Quick Sort**

```
private void quicksort(int low, int high) {
         int i = low, j = high;
         int pivot = numbers[low + (high-low)/2];
         while (i <= j) {
                 while (numbers[i] < pivot) {
                       i++;
                 }
                 while (numbers[j] > pivot) {
                        j--;
                  }
                   if (i <= j) {
                       exchange(i, j);
                       i++;
                       j--;
                  }
         }
          if (low < j)
                 quicksort(low, j);
         if (i < high)
                 quicksort(i, high);
}
```

## **Insertion Sort**

```
void insertionSort(int arr[]) {
  int n = arr.length;
  for (int i = 1; i < n; ++i) {
      int key = arr[i];
      int j = i - 1;
      while (j >= 0 && arr[j] > key) {
           arr[j + 1] = arr[j];
           j = j - 1;
      }
      arr[j + 1] = key;
   }
}
```

