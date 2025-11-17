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

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them?

        The biggest thing I learned through this assignment is that I now have a much better understanding of how different classes and functions interact with one another, and also how to conceptualize nested lists and nested loops. The biggest challenge I faced was trying to understand how the Stack and Queue classes were different and how that translated over to the difference between DFS and BFS. I overcame this challenge by asking Claude to explain it to me until I understood.

2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?

        These search algorithms could be useful for solving other puzzles like crosswords or scheduling problems. DFS and BFS could help find paths in GPS navigation or plan moves in a game. Constraint satisfaction could work for class scheduling, where you have to fit classes into time slots without conflicts. The backtracking approach would be helpful anytime you need to try different options and undo bad choices.

3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?

        A Stack uses LIFO (Last In First Out), like a stack of plates where you take the top one off first. A Queue uses FIFO (First In First Out), like a line at a store where the first person in line goes first. DFS uses a Stack because it explores one path deeply before trying others. BFS uses a Queue because it checks all options at one level before moving deeper. The Stack makes DFS go deep fast, while the Queue makes BFS spread out evenly.