# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import numpy library using import statement.
2. From scipy package import lu().
3. Get input from user and pass it as an array.
4. Get P,L,U matric using lu().
5. Print L and U matrix.

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

