# LU Decomposition without zero on the diagonal

## AIM:
To write a program to use LU Decomposition to find L and U matrix.
## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. import numpy library using import statement. 
2. From scipy package import lu().
3. Get input from user and pass it as an array. 
4. Get P, L U martix using lu().
5. print L and U matrix.

## Program:
```
# To print L and U matrix
import numpy as np
from scipy.linalg import lu
#import scipy
A = np.array(eval(input()))
P, L , U = lu(A)
#P,L,U = scipy.linalg.lu(A)
print(L)
print(U)
/*
Program to find the LU Decomposition of a matrix.
Developed by: Kiran J
RegisterNumber: 21500363
*/
```

## Output:

![lu](ex1.png)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

# LU Decomposition to solve a matrix

## AIM:
To write a program to use LU Decomposition to solve a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
 ### Step 1:
Import numpy library using import statement.

### Step 2:
From scipy package import lu_factor() and lu_solve().

### Step 3:
Get two inputs from user and pass it as matrix array.

### Step 4:
Find lu and pivot value of first matrix using lu_factor().

### Step 5:
Find solution of the matrix by using lu_solve() by passing lu, pivot values as first argument and second matrix as second argument.

### Step 6:
Print the solution.


## Program:
```
 '''Program to solve a matrix using LU decomposition.
Developed by: Kiran J
RegisterNumber: 21500363
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
B = np.array(eval(input()))
lu, pivot = lu_factor(A)
x = lu_solve((lu,pivot),B)
print(x) 
```

## Output:

![lu](ex12.png)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.



