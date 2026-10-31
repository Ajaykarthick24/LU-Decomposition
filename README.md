# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5. End the program 
## Program:
(i) To find the L and U matrix

Program to find L and U matrix using LU decomposition.
Developed by: Ajay karthick M
RegisterNumber: 212225040014
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


Program to solve a matrix using LU decomposition.
Developed by: Ajay Karthick M
RegisterNumber: 212225040014

```
# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu , piv),b)
print(X)
```

## Output:

(i) To find the L and U matrix

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/70b53f06-00dc-43a6-93c7-750709930d3d" />

(ii) To find the LU Decomposition of a matrix

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/c3eaee1c-45d4-440e-81c2-2e3cb2554070" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

