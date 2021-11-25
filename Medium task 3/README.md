**This code is written in C#, i wrote this in C#(C sharp) just for fun.**




In this we can only move diagonally or forward, so to collect maximum biscuits we need to maximize the number of cells we visit. 

**This is a very famous problem and is also called the gold mine problem.**


1.If we are at the first row or last column, then we are unable to move right-up so just assign 0 otherwise assign the value of goldTable[row-1][col+1] to right_up. 
2.If we are at the last row or last column, then we are unable to move right down so just assign 0 otherwise assign the value of goldTable[row+1][col+1] to right up. 
3.Now find the maximum of right, right_up, and right_down and then add it with that mat[row][col]. At last, find the maximum of all rows and first column and return it.
