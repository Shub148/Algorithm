# Selection Sort

## Overview

Selection Sort is a simple comparison-based sorting algorithm that repeatedly finds the smallest element from the unsorted portion of the array and places it at the beginning.

## Algorithm

1. Find the minimum element in the unsorted part of the array.
2. Swap it with the first unsorted element.
3. Move the boundary of the sorted portion one position to the right.
4. Repeat until the entire array is sorted.

## Java Implementation

```java
import java.util.*;
class file {
public static void selectionSort(int numbers[]){
for(int turn = 0; turn<numbers.length - 1; turn++){
int minNumbers = turn; // initialized minimum numbers is equal to current element
for(int j = turn + 1; j<numbers.length; j++){  // j is equal to i+ 1 which means the element ahich is present at i is already sorted 
if(numbers[minNumbers]> numbers[j]){
minNumbers = j;
}
}
//Swap
int temp = numbers[minNumbers];
numbers[minNumbers] = numbers[turn];
numbers[turn] = temp;
}
}
// print
public static void print(int numbers[]){
    

for(int num : numbers){
    System.out.print(num + "");
}
System.out.println();
}

public static void main(String args[]){
int numbers[] = {64, 25, 12, 22, 11};
selectionSort(numbers);
print(numbers);
}
}
```

## Time Complexity

| Case    | Complexity |
| ------- | ---------- |
| Best    | O(n²)      |
| Average | O(n²)      |
| Worst   | O(n²)      |

## Space Complexity

* O(1)

## Advantages

* Easy to understand and implement
* Requires minimal memory
* Performs fewer swaps compared to Bubble Sort

## Disadvantages

* Inefficient for large datasets
* Time complexity remains O(n²) in all cases
* Generally slower than Merge Sort and Quick Sort

## Example

### Input

```text
[64, 25, 12, 22, 11]
```

### Output

```text
[11, 12, 22, 25, 64]
```

## Applications

* Educational purposes for learning sorting concepts
* Small datasets
* Situations where memory usage must be minimal

## Conclusion

Selection Sort is a straightforward sorting algorithm that works well for small datasets and educational purposes. However, for larger datasets, more efficient algorithms such as Merge Sort or Quick Sort are preferred.
