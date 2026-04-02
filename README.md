# Assignment - 4 (CSP and map coloring)

##  Overview

Implementations of key Artificial Intelligence problems using **Search Techniques** and **Constraint Satisfaction Problems (CSP)**.
The assignment covers:
1. Map Coloring (Australia)
2. Map Coloring (Telangana)
3. Sudoku Solver using CSP
4. Cryptarithmetic Puzzle (TWO + TWO = FOUR)

# 1. Map Coloring – Australia

## Problem
Color the map of Australia such that no two adjacent states have the same color.

## States
WA, NT, Q, SA, NSW, V, T

## Approach
* Modeled as a **CSP**
* Used **Backtracking Search**
* Constraints ensure neighboring states have different colors

## Key Concepts
* Variables: States
* Domain: Colors
* Constraints: Adjacency

# 2. Map Coloring – Telangana (33 Districts)

## Problem
Assign colors to all 33 districts of Telangana such that no adjacent districts share the same color.

## Approach
* CSP formulation with:
  * Variables: Districts
  * Domain: {Red, Green, Blue, Yellow}
  * Constraints: Neighbor relationships
* Solved using **Backtracking**

## Highlights
* Real-world map modeling
* Larger constraint graph
* Demonstrates the scalability of CSP

# 3. Sudoku Solver using CSP

## Problem

Solve a 9×9 Sudoku grid ensuring:
* Unique values in each row
* Unique values in each column
* Unique values in each 3×3 box

## CSP Formulation
* Variables: 81 cells
* Domain: {1–9}
* Constraints: AllDiff (rows, columns, boxes)

## Approach
* Backtracking search
* Constraint checking at each step
  
## Key Insight
Constraint propagation reduces the exponential search space.

#  4. Cryptarithmetic Puzzle

## Problem

Solve:
TWO + TWO = FOUR
Each letter represents a unique digit.

## Constraints
* All letters have distinct digits (AllDiff)
* Leading digits (T, F) ≠ 0
* The arithmetic equation must hold

## Approach
* Used permutations of digits (0–9)
* Checked validity using constraints

## Example Solution

734 + 734 = 1468

# Techniques Used

* Backtracking Search
* Constraint Satisfaction Problem (CSP)
* AllDiff Constraint
* Generate-and-Test (for cryptarithmetic)

# Possible Improvements

* MRV (Minimum Remaining Values)
* Forward Checking
* Arc Consistency (AC-3)

# Conclusion

These problems demonstrate how CSP techniques can efficiently solve:

* Graph coloring problems
* Logical puzzles
* Arithmetic constraints

By applying constraints effectively, the search space is significantly reduced, making complex problems tractable.

# Author

AI Assignment Submission
Muhammad Muzaffar Shaik
SE24UCSE252

