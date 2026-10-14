# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
```
5a)
1. import os, numpy and lu from scipy.linalg
2. get the input using array() to retrieve the coeff matrix in "a"
3. using lu() retrieve the L and U matrices
4. printing the L and U matrices
5b)
1.import numpy, os and lu_factor, lu_solve from scipy.linalg
2.get the input using array() to retrieve the coeff and constant matrix in "a' and "b"
3.using lu_factor() retrieve the l and p matrices
4.using lu_solve() retrieve the solution matrix "x"
5.printing the solution matrix "x"
```
## Program:
(i) To find the L and U matrix
```
/*
'''Program to find L and U matrix using LU decomposition.
Developed by: Arvind R S
RegisterNumber: 26017022
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
P,L,U=lu(a)
print(L)
print(U) 
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
'''Program to solve a matrix using LU decomposition.
Developed by: Arvind R S
RegisterNumber: 26017022
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)
*/
```

## Output:
5a)<img width="837" height="805" alt="ex 5 a" src="https://github.com/user-attachments/assets/88f730dc-9659-43c3-b973-1a614772ef28" />
5b)<img width="562" height="635" alt="ex 5 b" src="https://github.com/user-attachments/assets/256ad89e-55ed-4a8f-a534-e577bf4066a1" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

