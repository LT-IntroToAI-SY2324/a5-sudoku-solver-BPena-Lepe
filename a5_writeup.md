# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?
DFS seems to be faster than BFS when solving sudoku puzzles as DFS solved the puzzle in 337 iterations while BFS solved it in 556.BFS might be preferable in problems where there is much left to be solved, while with our sudoku we have already implemented function that eliminates many wrong solutions, meaning a few deep searches would be more likely to find the solution. 


2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

We could have implemented a normal list for each of the algorithms, except we would have to implement while loops to access the data in the right order.

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

It could be applied to solving other single player games, like jigsaw puzzles or a rubiks cube, for the jigsaw puzzle it would try to solve in in chunks and for the rubiks cube the board would be transformed into a cross like 2d array where each turn would move around 8 other squares. The lessons learned from this assignment like finding places to put numbers would be useful in the real world where you might have to find a way to fit items into a certain area.
