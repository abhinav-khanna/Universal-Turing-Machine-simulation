
# Universal-Turing-Machine-simulation

Question 1.
-----------------
Simulate a single-tape Turing machine which starts with the initial tape contents as x # y where x and y are binary strings, and the tape contents when the machine halts should be z such that z is the remainder when x is divided by y. The machine should always halt. The head should point to the start position of the tape contents when it halts.

The program must print each step of the Turing machine in a line, beginning with the step counter. End each line with a new line so that the output can be parsed easily. For example, if you move right while changing a 0 to 1 on the tape during the execution of the Turing machine, then you should print as follows:
0: 0  1 R (the 0 before ":" is the step number, the next 0 is the initial tape symbol, next 1 is the modified tape symbol, and the final R is the direction of the movement.)
1: 1 1 L (step 1, when you encounter 1, don't change it, and move left)
… etc.

Example input/output behaviour:

(i) On input 11 # 10    the final tape content should be 1  (That is, the input is the decimal number 3 and 2. When you divide 3 by 2, the remainder is 1.)
(ii) On input 110 # 11    the final tape content should be 0 (That is, the input is the decimal number 6 and 3. When you divide 6 by 3, the remainder is 0.)
… etc.

Question 2.
-----------------
Simulate a single-tape Turing machine which finds the maximum degree of vertex in a given directed graph. The machine should always halt. The head should point to the start position of the tape contents when it halts. 

The initial tape contents are as follows:  

The first input is the number of vertices in the graph. This is followed by a # symbol, and then the n x n binary adjacency matrix of the graph follows. Each row of the adjacency matrix is terminated by a # symbol. 

Example input/output behaviour:
The input 10 # 1 0 # 1 1 # represents a graph with 2 vertices (represented in binary as 10 at the start of the input string) having an adjacency matrix with 2 rows. The first row is 1 0 and the second row is 1 1. The Turing machine should halt with the tape contents 10 in this case (which is the binary representation of 2, which is the maximum degree in the graph).
The program should print the step counter, followed by a : followed by the tape symbol (initial and modified) and the direction of the movement (all as described in question 1 already).

Question 1 is written in q1_2017csb1061.c
Question 2 is written in q2_2017csb1061.c
