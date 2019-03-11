# QuickSort Algorithm

As merge sort algorithm, the quick sort algorithm also works on the mechanism termed as “divide and conquer”. The concept of Quick sort is to split the array into halves as an array before a pivot value and array after pivot value. Pivot value being the reference value which is used to divide the array into parts. Multiple iterations are required to completely sort the array in some order. Every iteration comprises of passes, a pass being the unit move which ensures that by the end of any iteration the pivot value comes to its original position, as it would be in the final sorted array.

The name comes from the fact that quicksort is capable of sorting a list of data elements significantly faster than any of the common sorting algorithms.

## Quick sort Time Complexity

The time complexity of quick sort can be depicted by the recurrence relation as shown below:

**T(n) = T(k) + T(n-k-1) + O(n)**

The first two terms indicate the recursive calls, whereas the last term is for the partition. K is the number of terms that are smaller than the pivot value, and n being the total number of elements in an array. The time complexity of the sorting depends on the input array and the logic for partition.

Thus, based on the above concept the following three cases for time complexity arise:

 1. Worst Case:
The named situation arises as a result of the fact that one selects either the smallest or the largest value as the pivot. Thus, considering the said situation, the worst case would be the situation wherein the array elements are already arranged in either increasing or decreasing order. Thus, on solving the actual recurrence relation, the complexity results out to be O(n2). This means that for the array to be completely sorted one needs to compare almost all the elements.
 
 2. Best Case:
 The best case would be the one where the pivot selected is the middle element. Thus, the efforts reduce down to half altogether. Thus the complexity expression gives the result as O(nlogn).
 
 3. Average Case:
For the named case, there might be several other combinations of selecting the pivot element. Thus, one has to consider all the permutations for the same. The recurrence relation results, to O(nlogn) as well.

The Worst case scenario results in the complexity more than the complexities for any other sorting algorithms. But yet, the Quick Sort is a faster sorting algorithm than any other. Because, as per the code standards it is easier and efficient enough to implement the inner loop of the quick sort code on any real-world data.

Quick sort can be implemented in many ways as the choice of pivot might vary, thus the chance for landing in the worst case is quite a rare one.

References taken from [interviewbit](https://www.interviewbit.com/tutorial/quicksort-algorithm/).

