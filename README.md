# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. read the elements of augmented matrix into array a and b
2.calculate elements of L and U
3.print L and U matrix
4.find V by solving LV = B by forwrd substitution
5.find X by solving UX = V by backward substitution
6.print array X as the solution


## Program:
(i) To find the L and U matrix
```python
'''Program to find L and U matrix using LU decomposition.
Developed by: B KRISHNAKANTH
RegisterNumber: 23006762
'''
import numpy as np 
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
'''Program to solve a matrix using LU decomposition.
Developed by: B KRISHNAKANTH
RegisterNumber: 23006762
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A,B=eval(input()),eval(input())
lu,piv=lu_factor(A)
x = lu_solve((lu,piv),B)
print(x)
'''

## Output:
![image](https://github.com/Krishnakanth23006762/LU-Decomposition/assets/138849446/95958a4b-55a2-40c8-a407-d447270a8e89)
![image](https://github.com/Krishnakanth23006762/LU-Decomposition/assets/138849446/e12bfede-7d43-4a73-9c66-94df62f11be1)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

