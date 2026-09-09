# LU Decomposition 
# NAME: SUNDARESH.K
# REG.NO: 212225220111
## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program and import the required library (numpy).
2. Initialize the matrix for which the LU decomposition needs to be found.
3. Apply LU Decomposition
4. Display the results

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: K.SUNDARESH
RegisterNumber: 212225220111
*/
```
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: K.SUNDARESH
RegisterNumber: 2122252220111
*/
```
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
b= np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:
(i) To find the L and U matrix
<img width="952" height="822" alt="image" src="https://github.com/user-attachments/assets/8332d0bc-85ea-4a92-9080-1d7c4460ef2e" />

(ii) To find the LU Decomposition of a matrix
<img width="772" height="605" alt="image" src="https://github.com/user-attachments/assets/602c31ba-b7f7-4253-bafa-322e3a07b5da" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

