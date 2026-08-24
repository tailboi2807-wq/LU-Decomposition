# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries (numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor(), to get the solutions
5. End the program

## Program:
(i) To find the L and U matrix
```
*/
Program to find the L and U matrix.
Developed by:MUKESH M
RegisterNumber: 212225240093
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
matrix = np.array(eval(input()))
P,L,U = lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: MUKESH M
RegisterNumber: 212225240093
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu = lu_factor(matrix)
result = lu_solve((piv,lu),constant)
print(result)

```

## Output:
<img width="1217" height="463" alt="image" src="https://github.com/user-attachments/assets/ff774e56-c222-43fc-a376-7dc23a9c421d" />
<img width="1225" height="246" alt="image" src="https://github.com/user-attachments/assets/494ea16e-d29a-4193-b2b4-eae37cdf3b39" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

