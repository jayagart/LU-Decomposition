# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i)
1.Input the Matrix:

Accept a square matrix 
𝐴
A as input.

Example input format (as string)

2.Convert to NumPy Array:

Use np.array() to convert the input into a NumPy array.

3.LU Decomposition:

Use scipy.linalg.lu(A) to compute the matrices 
𝑃
,
𝐿
,
𝑈
P,L,U.

4.Output the L and U Matrices:

Print the L (lower triangular matrix).

Print the U (upper triangular matrix).

(ii)
1. Input the coefficient matrix A and right-hand side vector b.
2. Convert inputs to NumPy arrays.
3. Perform LU decomposition using scipy.linalg.lu_factor:
   - Decomposes A into LU matrix and pivot indices.
4. Solve the system using scipy.linalg.lu_solve:
   - Computes x such that Ax = b using the LU decomposition.
5. Output the solution vector x.


## Program:
(i) To find the L and U matrix
```
import numpy as np
from scipy.linalg import lu
A= np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A= np.array(eval(input()))

b= np.array(eval(input()))

lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:
![image](https://github.com/user-attachments/assets/47b6f633-b769-47a4-b0a1-7a64d8b297bd)
![image](https://github.com/user-attachments/assets/395a911b-4b53-4de0-a9c7-16008e6433ab)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

