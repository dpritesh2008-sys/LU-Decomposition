# LU Decomposition 
~~~
Name: Branzen B V
Register No: 212225100005
~~~

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

1.Start the program

2.Import the necessary libraries(numpy,scipy.linalg)

3.Define the matrix using numpy

4.Use lu(),lu_solve(),lu_factor() to get the solutions

5.End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Ritesh DP
RegisterNumber: 212225040339
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Ritesh DP
RegisterNumber: 212225040339
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:

<img width="1237" height="580" alt="image" src="https://github.com/user-attachments/assets/de51203c-f636-4a39-b1ae-efc2ebf68765" />

<img width="1227" height="326" alt="image" src="https://github.com/user-attachments/assets/f0196e93-85e1-4ba1-ac1b-a89ef7350e54" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

