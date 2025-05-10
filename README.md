# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1)
## step1:
Import numpy as np to handle matrices.
Import the lu function from scipy.linalg to perform LU decomposition.
## step2:
Use eval(input()) to take a 2D list as input from the user and convert it into a NumPy array.
## step3:
Use P, L, U = lu(A) to decompose matrix A into:
P: Permutation matrix
L: Lower triangular matrix
U: Upper triangular matrix
## step4:
print the L (lower triangular) and U (upper triangular) matrices.
2)
## step1:
Import numpy for matrix creation.
Import lu_factor and lu_solve from scipy.linalg for LU decomposition and solving.
## step2:
Use eval(input()) to read both matrices from the user.
## step3:
Use lu_factor(A) to get:
lu: Combined LU matrix
piv: Pivot indices used for row permutations
## step4:
Solve the linear system Ax = B using the LU decomposition
## step5:
Print the result using print().
## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Hemalatha A
RegisterNumber:212224240056
*/
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```

(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by:Hemalatha A
RegisterNumber: 212224240056
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
piv,lu=lu_factor(A)
result=lu_solve((piv,lu),B)
print(result)
```

## Output:
![alt text](<Screenshot 2025-04-10 143524-1.png>)
![alt text](<Screenshot 2025-04-10 143609.png>)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

