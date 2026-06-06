# Bubble Sort

## Overview

Bubble Sort is a simple comparison-based sorting algorithm that repeatedly compares adjacent elements and swaps them if they are in the wrong order. The process continues until the array is sorted.

## Algorithm

1. Traverse the array from left to right.
2. Compare adjacent elements.
3. Swap them if they are in the wrong order.
4. Repeat the process for all elements.
5. Continue until no swaps are needed.

## Java Implementation

```java
import java.util.*;
class file{ 
public static void bubbleShort(int numbers[]){
for(int turn = 0; turn<numbers.length; turn++){ // outer loop (n)
for(int j = 0; j<numbers.length -1-turn; j++){ // inner loop (n-1)
if(numbers[j] > numbers[j + 1]){  // current element(numbers[j] is bigger than next elemenr[j+1] then current element goes to next positon or go ahead
// conditon or loop of swapping the numbers or array

int temp = numbers[j];
numbers[j] = numbers[j+1];
numbers[j+1] = temp;
}
}
}
}
// create a new function to print array or numbers
public static void printNumbers(int numbers[]){
for(int i = 0; i<numbers.length; i++){
System.out.print(" " +numbers[i]);
}
System.out.println();
}

public static void main(String args[]){
int numbers[] = {5, 3, 8, 4, 2};
bubbleShort(numbers);
printNumbers(numbers);
}
}
```

## Time Complexity

| Case    | Complexity |
| ------- | ---------- |
| Best    | O(n)       |
| Average | O(n²)      |
| Worst   | O(n²)      |

## Space Complexity

* O(1)

## Advantages

* Easy to understand and implement
* No extra memory required
* Stable sorting algorithm

## Disadvantages

* Inefficient for large datasets
* High time complexity compared to advanced sorting algorithms

## Example

Input:

```text
[5, 3, 8, 4, 2]
```

Output:

```text
[2, 3, 4, 5, 8]
```












import java.util.*;
class file{ 
public static void bubbleShort(int numbers[]){
for(int turn = 0; turn<numbers.length; turn++){ // outer loop (n)
for(int j = 0; j<numbers.length -1-turn; j++){ // inner loop (n-1)
if(numbers[j] > numbers[j + 1]){  // current element(numbers[j] is bigger than next elemenr[j+1] then current element goes to next positon or go ahead
// conditon or loop of swapping the numbers or array

int temp = numbers[j];
numbers[j] = numbers[j+1];
numbers[j+1] = temp;
}
}
}
}
// create a new function to print array or numbers
public static void printNumbers(int numbers[]){
for(int i = 0; i<numbers.length; i++){
System.out.print(" " +numbers[i]);
}
System.out.println();
}

public static void main(String args[]){
int numbers[] = {};
bubbleShort(numbers);
printNumbers(numbers);
}
}
