# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### (i) To find the L and U matrix
1.Start the program.

2.Import required libraries:

3.Accept matrix input from the user using eval(input()).

4.Call the lu() function from scipy.linalg to perform LU decomposition:

5.Display the results.

6.Print the L (Lower Triangular) matrix.

7.Print the U (Upper Triangular) matrix.

8.End the program.

### (ii) To find the LU Decomposition of a matrix
1.Start the program.

2.Import necessary libraries.

3.Input the coefficient matrix A (square matrix of coefficients).

4.Input the constant matrix/vector B.

5.Perform LU factorization using lu_factor(A).

6.Solve the system of equations AX = B using lu_solve((lu, pivot), B).

7.Display the solution vector X.

8.End the program.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: AHAMADH SULAIMAN M
RegisterNumber: 212224230009
*/


import numpy as np
from scipy.linalg import lu

A = eval(input())

P,L,U  = lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: AHAMADH SULAIMAN M
RegisterNumber: 212224230009
*/

import numpy as np
from scipy.linalg import lu_factor,lu_solve

A = eval(input())
B = eval(input())

lu,pivot = lu_factor(A)
result = lu_solve((lu,pivot),B)
print(result)

```

## Output:

<img width="1248" height="576" alt="image" src="https://github.com/user-attachments/assets/edd9c866-2a4c-41e9-91ea-3aaa7db79b28" />

<img width="1252" height="312" alt="image" src="https://github.com/user-attachments/assets/78c5af3c-7119-4930-a239-3b3fb3dab9dd" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

