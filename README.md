# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
	1. Get the input matrix using np.array()   
    2. Find the 2-norm of the matrix using np.linalg.norm()
	3. Print the norm of the matrix in two decimal places.
## Program:
```Python
# Register No:24901111
# Developed By:PANDEESWARAN N
# 1-Norm of a Matrix

import numpy as np
array=np.array(eval(input()))
result=np.linalg.norm(array,1)
print(result)




# 2-Norm of a Matrix

import numpy as np
array=np.array(eval(input()))
result=np.linalg.norm(array,2)
print(f"{result:.2f}")







# Infinity Norm of a Matrix

import numpy as np
array=np.array(eval(input()))
result=np.linalg.norm(array,np.inf)
print(f"{result:.2f}")





```
## Output:
### 1-Norm of a Matrix
![output](<Screenshot 2024-12-10 214747.png>)

### 2-Norm of a Matrix
![output](<Screenshot 2024-12-10 214634.png>)

### Infinity Norm of a Matrix
![output](<Screenshot 2024-12-10 214654.png>)

## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
