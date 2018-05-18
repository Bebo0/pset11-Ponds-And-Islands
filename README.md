pset 11 from CPSC 110 - Computation, Programs, and Programming.

Finds the number of islands and ponds on a square map.

Given an n x n list, the program goes through every element in the master list, if the element has not been visited, it 
creates the position of all adjacent blocks, up to 4 blocks (depending on whether the blocks are viable (not off the map) or not). The program 
then matches the positions with a block state (true/island or false/pond) from the preserved master list and checks if 
these blocks are the same state as the original block. If they are, the program repeats the process (creates the 4 positions...) 
until there are no more blocks that can be recursed over, in which case, the master recursion advances to check where the 
next unvisited block is and repeats the process over it.
