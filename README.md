# Sparse-Matrix
Generate sparese matrix representation for a sparse matrix
Representing a sparse matrix by a 2D array leads to wastage of lots of memory as zeroes in the matrix are of no use in most of the cases. So, instead of storing zeroes with non-zero elements, we only store non-zero elements. This means storing non-zero elements with triples- (Row, Column, value).

2D array is used to represent a sparse matrix in which there are three rows named as

Row: Index of row, where non-zero element is located
Column: Index of column, where non-zero element is located
Value: Value of the non zero element located at index – (row,column)

Algorithm

Step 1: Start

Step 2:Set M to number of rows in MATRIX 

Step 3: Set N to number of columns in MATRIX 

Step 4: I = 0, NNZ = 0. Declare A, JA, and IA. 
        Set IA[0] to 0 

Step 5: for I = 0 ... N-1 

Step 6: for J = 0 ... N-1 

Step 7: If MATRIX [I][J] is not zero
           Add MATRIX[I][J] to A
           Add J to JA
           NNZ = NNZ + 1
        [End of IF] 

Step 8: [ End of J loop ]
        Add NNZ to IA
        [ End of I loop ] 

Step 9: Print vectors A, IA, JA 

Step 10: Stop
