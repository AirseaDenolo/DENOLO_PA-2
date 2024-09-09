**NORMALIZATION PROBLEM**
```
import numpy as np

#Create a random 5x5 array and store it in variable X 
X = np.random.rand(5, 5) 

#Normalize the array using the formula 
x_normalized = (X - X.mean()) / X.std()

#Save the normalized ndarray as X_normalized.npy
np.save('X_normalized.npy', x_normalized)

#Print the output of the original and normalized arrays
print("Original Array:\n", X, "\nNormalized Array:\n", x_normalized)
```

**DIVISIBLE BY 3 PROBLEM**
```
import numpy as np

#Create an array of the first 100 positive integers
n = np.arange(1,101)

#Square every element
A_squared = np.square(n)

#Resize into a 10x10 ndarray
A = A_squared.reshape(10,10)

#Determine the elements divisible by 3
Div_by_3 = A[A % 3 == 0]

#Save the result as div_by_3.npy
np.save('div_by_3.npy', Div_by_3)

#Print the output of "A" and "div_by_3"
print("A =\n", A, "\nElements divisible by 3:\n", Div_by_3)
```
