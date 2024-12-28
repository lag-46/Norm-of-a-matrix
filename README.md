# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
	i.one norm of a matrix

	1.Input the Matrix:

2.Read a matrix (as a list of lists) from the user.

3.Use eval(input()) to evaluate the user input and convert it into a NumPy array.
Definition of the L1 Norm:

4.For a matrix, the L1 norm is the maximum absolute column sum.
It is defined as:
∣
∣
𝐴
∣
∣
1
=
max
⁡
1
≤
𝑗
≤
𝑛
∑
𝑖
=
1
𝑚
∣
𝑎
𝑖
𝑗
∣
∣∣A∣∣ 
1
​
 = 
1≤j≤n
max
​
  
i=1
∑
m
​
 ∣a 
ij
​
 ∣
where:
𝐴
A is the matrix,
𝑎
𝑖
𝑗
a 
ij
​
  is the element in the 
𝑖
i-th row and 
𝑗
j-th column.

5.Compute the L1 Norm:

6.Use the np.linalg.norm() function with ord=1 to compute the L1 norm for the input matrix.
Output the Result:

7.Print the computed L1 norm.


ii.2-norm of a matrix

1.Input the Array:

2.Accept input from the user in the form of a list (e.g., [1, 2, 3] for a vector or [[1, 2], [3, 4]] for a matrix).
Convert the input into a NumPy array using np.array(eval(input())).
Definition of the L2 Norm:

3.For a vector, the L2 norm is the square root of the sum of the squares of its elements:
∣
∣
𝑣
∣
∣
2
=
∑
𝑖
=
1
𝑛
𝑣
𝑖
2
∣∣v∣∣ 
2
​
 = 
i=1
∑
n
​
 v 
i
2
​
 
​
 
4.For a matrix, the L2 norm corresponds to the largest singular value of the matrix (also known as the spectral norm).
Compute the L2 Norm:

5.Use np.linalg.norm(array, 2) to compute the L2 norm.
If the input is a vector, it computes the Euclidean norm.
If the input is a matrix, it computes the spectral norm.

6.Format the Result:

7.Round the computed result to two decimal places using f"{result:.2f}".
Output the Result:

8.Print the formatted result.


iii.infinity norm of a matrix

1.Input the Array:

2.Accept input from the user in the form of a list (e.g., [1, -2, 3] for a vector or [[1, 2], [-3, 4]] for a matrix).
Convert the input into a NumPy array using np.array(eval(input())).
Definition of the Infinity Norm:

3.For a vector, the infinity norm is the maximum of the absolute values of its elements:
∣
∣
𝑣
∣
∣
∞
=
max
⁡
𝑖
∣
𝑣
𝑖
∣
∣∣v∣∣ 
∞
​
 = 
i
max
​
 ∣v 
i
​
 ∣

4.For a matrix, the infinity norm is the maximum absolute row sum:
∣
∣
𝐴
∣
∣
∞
=
max
⁡
1
≤
𝑖
≤
𝑚
∑
𝑗
=
1
𝑛
∣
𝑎
𝑖
𝑗
∣
∣∣A∣∣ 
∞
​
 = 
1≤i≤m
max
​
  
j=1
∑
n
​
 ∣a 
ij
​
 ∣

5.Compute the Infinity Norm:

Use np.linalg.norm(array, np.inf) to compute the infinity norm.
For a vector, it computes the maximum absolute value of the elements.
For a matrix, it computes the maximum sum of the absolute values of the elements in each row.
Format the Result:

6.Round the computed result to two decimal places using f"{result:.2f}".
Output the Result:

7.Print the formatted result.

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
