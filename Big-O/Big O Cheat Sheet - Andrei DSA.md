# Big O Cheat Sheet

## Big O Notations

- **`O(1)`** **Constant Complexity** - No loops
- **`O(log N)`** **Logarithmic Complexity** - Usually searching algorithms have log `n` if they are sorted (Binary Search)
- **`O(n)`** **Linear Complexity** - for loops, while loops through `n` items
- **`O(n log(n))`** **Log Linear Complexity** - Usually sorting operations
- **`O(n^2)`** **Quadratic Complexity** - Every element in a collection needs to be compared to ever other element. Two nested loops. Three nested loops will give **`O(n^3)`**
- **`O(2^n)`** **Exponential Complexity** - Recursive algorithm that solves a problem of size `n`
- **`O(n!)`** **Factorial Complexity** - You are adding a loop for every element

## Big O Tips

- Iterating through half a collection is still **`O(n)`**
- Two separate collections: **`O(a*b)`**

## What can increase the time taken by a function?

- Operations `(+, -, *, /, %)`
- Comparisons `(</=, >/=, ==/=)`
- Looping `(for, while)`
- Outside Function call `(function())`

## Big O Rules

- Rule 1: Always worst case
- Rule 2: Remove Constants
- Rule 3: Different inputs/arguments should have different variables. A and B arrays nested would have a Big O of **`O(a*b)`**. If a function takes in 2 arrays as 2 arguments and has 2 different for loops looping over each array, Big O would be **`O(a+b)`**
  - **`+`** for steps in order
  - **`*`** for nested steps
- Rule 4: Drop non-dominant terms

## What causes Space Complexity?

- Variables
- Data Structures
- Function Calls
- Allocations
