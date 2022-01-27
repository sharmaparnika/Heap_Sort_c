# Heap Sort in C

Heap sort is one of the sorting algorithms used to arrange a list of elements in order. Heapsort algorithm uses one of the tree concepts called Heap Tree. 

In this sorting algorithm, we use Max Heap to arrange list of elements in Descending order and Min Heap to arrange list elements in Ascending order.

Heap sort processes the elements by creating the min-heap or max-heap using the elements of the given array. Min-heap or max-heap represents the ordering of array in which the root element represents the minimum or maximum element of the array.

Heap sort basically recursively performs two main operations -

*   Build a heap H, using the elements of array.
*   Repeatedly delete the root element of the heap formed in 1st phase.

### Algorithm

    HeapSort(arr)  
    BuildMaxHeap(arr)  
    for i = length(arr) to 2  
    swap arr[1] with arr[i]  
        heap_size[arr] = heap_size[arr] ? 1  
        MaxHeapify(arr,1)  
    End  


### Heap Sort Complexity

Now, let's see the time complexity of Heap sort in the best case, average case, and worst case. We will also see the space complexity of Heapsort.

1. Time Complexity

 | Case | Time Complexity |
 | --- | --- |
 | `Best Case` | **O(n(logn))** |
 | `Average Case` | **O(n(logn))** |
 | `Worst Case` | **O(n(logn))** |
 
*   Best Case Complexity - It occurs when there is no sorting required, i.e. the array is already sorted. The best-case time complexity of heap sort is O(n logn).
*   Average Case Complexity - It occurs when the array elements are in jumbled order that is not properly ascending and not properly descending. The average case time complexity of heap sort is O(n log n).
*   Worst Case Complexity - It occurs when the array elements are required to be sorted in reverse order. That means suppose you have to sort the array elements in ascending order, but its elements are in descending order. The worst-case time complexity of heap sort is O(n log n).


Please Note - The time complexity of heap sort is O(n logn) in all three cases (best case, average case, and worst case). The height of a complete binary tree having n elements is **logn**.

2. Space Complexity

      | Space Complexity | O(1) |
      | --- | --- |
      | `Stable` | **NO** |

**Please Note** - The space complexity of Heap sort is O(1).

**Output-**

![image](https://user-images.githubusercontent.com/73773202/151413318-d50f134b-e6ff-4b5b-a921-6ee0cbdd4bc0.png)


---
