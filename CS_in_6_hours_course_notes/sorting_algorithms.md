# Sorting Algorithms

## Bubble Sort

Given an array of numbers. Each iteration will go through the array of numbers, comparing two at a time and swapping them if they're out of order.

```javascript

var array = [8, 7, 3, 5, 9, 2, 0]
// we want to reorder this array to go from smallest to larges numbers

do {
  let swapped = false;
  for (let i = 0; i < array.length - 1; i++){
    if (array[i] > array[i+1]){
      let temp = array[i];
      array[i] = array[i+1];
      array[i+1] = temp;
      swapped = true;
    }
  }
  
} while (swapped)

```

* O(n^2)
  * Worst case scenario, the algorithm will have to look at a data set of n numbers and go through that data set n times in order to sort them. 
* Inefficient algorithm because it spends time looking through data that's already sorted. If you had the following array: `[1, 2, 3, 4, 5, 6, 0]` 
  * Bubble sort will compare all the numbers that are already sorted then get to the end of the array, and move the 0 one spot to the left. This would happen n times until the 0 found its way to array[0]. This is inefficient because a lot of steps are wasted looking at sorted data, which ideally will be skipped with more efficient algorithms. 

  ## Insertion Sort








  