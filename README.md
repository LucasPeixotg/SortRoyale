# Sort Royale

## 1. Bogosort
    Type: Inefficient and highly random
    How it works: Bogosort generates random permutations of the list until it happens to be sorted.
    Time complexity: O((n+1)!), which is incredibly inefficient.
    Use case: None in real life—it's more of a joke or theoretical curiosity.

## 2. Timsort
    Type: Hybrid sorting algorithm (merge sort + insertion sort)
    How it works: Timsort divides the list into small chunks (called runs) and uses insertion sort on these chunks. Then, it merges the runs using a merge sort.
    Time complexity: O(n log n) in the worst case, and O(n) in the best case.
    Use case: This is the default sorting algorithm used in Python's sorted() function and Java’s Arrays.sort().

## 3. Bubble Sort
    Type: Comparison-based
    How it works: It repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order.
    Time complexity: O(n²)
    Use case: Mainly for educational purposes, it's too slow for large datasets.

## 4. Selection Sort
    Type: Comparison-based
    How it works: The algorithm divides the list into a sorted and unsorted section. It repeatedly selects the smallest (or largest) element from the unsorted portion and moves it to the sorted portion.
    Time complexity: O(n²)
    Use case: Useful when memory writes are costly because it only makes O(n) swaps.

## 5. Merge Sort
    Type: Divide and conquer
    How it works: Merge sort divides the list into two halves, recursively sorts them, and merges the sorted halves.
    Time complexity: O(n log n)
    Use case: When stability (preserving the order of equal elements) is important.

## 6. Quick Sort
    Type: Divide and conquer
    How it works: Quick sort selects a pivot element and partitions the array into two sections—those smaller than the pivot and those greater. It then recursively sorts the partitions.
    Time complexity: O(n log n) on average, but O(n²) in the worst case (when the pivot selection is poor).
    Use case: Great for general-purpose sorting due to its average performance and low memory usage.

## 7. Heap Sort
    Type: Comparison-based
    How it works: The array is first turned into a heap structure (binary tree), and then the largest element (root) is swapped with the last element, reducing the heap size. This process is repeated until the heap is empty.
    Time complexity: O(n log n)
    Use case: When constant time complexity for both insertion and extraction is needed.

## 8. Insertion Sort
    Type: Comparison-based
    How it works: Insertion sort builds the sorted array one item at a time by repeatedly taking the next unsorted item and inserting it into its correct position in the sorted section.
    Time complexity: O(n²)
    Use case: For small datasets, or when the list is almost sorted.

## 9. Radix Sort
    Type: Non-comparison-based (integer sorting)
    How it works: Radix sort processes the digits of numbers starting from the least significant to the most significant, using a stable sub-sorting algorithm (like counting sort).
    Time complexity: O(nk), where k is the number of digits.
    Use case: Sorting large datasets of integers or strings.