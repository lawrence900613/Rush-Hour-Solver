# Rush Hour Solver
This application is designed to solve the puzzle in rush hour game. It used the linkedlist and hashmap as fudenmental data strucutre to record every possilbe board situation and the breath-first search to find the all possible solution to return the fastest one.
# Steps to solve puzzle
Initial : Create a linkedlist with initial puzzle board. Create a hashmap to store visited board in the following step

Step 1 : If linkedlist is not empty, remove the first board in the linkedlist and store it as current board. 

Step 2 : Checking whether the current board had been solved or not. If it has been solved, stop the program and return the solution.

Step 3 :  Move every car in the board with different moving steps, whenever each car move steps (no matter how long the step is), it will create a new board and program will check whether the new board is visited or not(in hashmap). If the new board haven’t been visited , adding the new board to linkedlisted and hashmap(it will prevent adding same board to the linedlisted)

Step 4 : Whenever the car move successfully(adding to linkedlist), the created new bored will store the solution steps. (carname + Direction + length) and go back to step2.


