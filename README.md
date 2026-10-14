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
2. creating array "a" which retrieve input of the matrix 
3. using lu() function L and U are fetched
4. printing L and U
5b)
1.import os, numpy and lu_factor and lu_solve from scipy.linalg
2.creating array "a" and "b" which retrieve input of coeff and constant matrix
3.using lu_factor() retrieve the L and P matrices
4.using lu_solve retrieve the solution values in x
5.printing the solution values
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
'''5a'''<img width="837" height="805" alt="ex 5 a" src="https://github.com/user-attachments/assets/069ac2e9-2c74-4709-a98c-81e5b6973f93" />
'''5b'''<img width="562" height="635" alt="ex 5 b" src="https://github.com/user-attachments/assets/5e682715-55a8-4a19-b9d2-9c0537463524" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

