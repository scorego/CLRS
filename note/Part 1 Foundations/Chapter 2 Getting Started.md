## The sorting problem  
Input: A sequence of n numbers `[a1, a2, ... , an]`  
Output: A permutation (reordering) `[a1', a2', ..., an']` of the input sequence such that  `a1' <=  a2' <= ... <= an'`


```
INSERTION-SORT(A, n)
for i = 2 to n
    key = A[i]
    // insert A[i] into the sorted subarray A[1: i - 1]
    j = i - 1
    while j > 0 and A[j] > key
        A[j + 1] = A[j]
        j = j -1 

    A[j + 1] = key
```

## Analyzing algorithms
Most of this book assumes a generic one-processor, random-access machine (RAM) model of computation as the implementation technology, with the  understanding that algorithms are implemented as computer programs. In the RAM model, instructions execute one after another, with no concurrent operations. The RAM model assumes that each instruction takes the same amount of time as any other instruction and that each data access-using the value of a variable or storing into a variable-takes the same amount of time as any other data access. In other words, in the RAM model each instruction or data access takes a constant amount of time-even indexing into an array.
