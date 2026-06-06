# Insertion Sort in Java

## Definition

Insertion Sort is a simple sorting algorithm that builds the final sorted array one element at a time. It works by taking each element and inserting it into its correct position among the previously sorted elements.

## Java Program

```java
import java.util.*;
class file{
public static void insertionSort(int num[]){
for(int i = 1; i<num.length; i++){
int curr = num[i]; // now store current variable temperory the value of num
int prev = i - 1; // store the value by subtracting one position from current position

// finding the correct position
while( prev>=0; && num[prev] > curr){ // if previou is grater than current and previous is grater and equal to zero then 
num[prev + 1] = num[prev]; // then previous + 1 position replaced by previous element
prev -- ; 
}
num[prev + 1] = curr;
}
}
public static void print(int num[]){
for(int i=0; i<num.length; i++){
System.out.print(num[i] + " ");
}
System.out.println();
}
public static void main(String args[]){
int num[] = { 5,4,2,1,3};
insertionSort(num);
print(num);
}
}
```

## Output

```
1 2 3 4 5
```

## Working Example

Initial Array:

```
5 4 1 3 2
```

Pass 1:

```
4 5 1 3 2
```

Pass 2:

```
1 4 5 3 2
```

Pass 3:

```
1 3 4 5 2
```

Pass 4:

```
1 2 3 4 5
```

## Time Complexity

| Case         | Complexity |
| ------------ | ---------- |
| Best Case    | O(n)       |
| Average Case | O(n²)      |
| Worst Case   | O(n²)      |

## Space Complexity

```
O(1)
```

## Advantages

* Simple to implement
* Efficient for small datasets
* Stable sorting algorithm
* In-place sorting (requires no extra memory)

## Disadvantages

* Inefficient for large datasets
* Performance decreases significantly as input size grows
