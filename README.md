# CI2024_lab3
Third lab of the Computational Intelligence 2024 course.
The goal of this lab is to implement a solution to the n-puzzle problem using a path search algorithm. 

## A* Search
The solution is based on the A* search algorithm. The algorithm uses a priority queue implemented with a heap to store the nodes to be expanded. It stops when the goal state is reached or when there are no more nodes to expand.

As the heuristic function, I tried using 2 different functions:

* The Manhattan distance between the current state and the goal state
* An enhanced Manhattan distance that also considers the number of tiles that have a conflicting goal position (they are in the same row or column but not in the correct order)

## Considerations
Unfortunately the implementation I provided is able to solve in reasonable time only a 3x3 puzzle. For the 4x4 puzzle, the algorithm takes too long to find a solution. The problem might be due the heuristic function, which is too simplistic to solve a bigger problem or to the lack of a data structure that allows for fast retrieval of node-cost tuple. 
