#### ECE 2112: Advanced Computer Programming and Algorithms
---
## **Experiment 2: Numerical Python (Numpy)**
#### Submitted by: **Jihan Harvey C. Casiedo**
#### Section: 2ECE-A
---
#### **Background of the Experiment**
##### Numpy is a popular core library that is widely used in scientific computing. It provides a high-performance multidimensional array object and tools for efficient array manipulation. In addition, it also offers sophisticated broadcasting functions, integration with C/C++ and Fortran code, and useful features for linear algebra, Fourier transforms, and random number generation.
---
#### **Objectives of the Experiment**
##### This experiment aims for students to identify the codes and functions incorporated in the Numpy library and to be able to apply and use the different codes and functions in creating a Python program using a Numpy library.
---
#### **Normalization Problem**
##### Normalization is one of the most basic preprocessing techniques in data analytics. This involves centering and scaling process. Centering means subtracting the data from the mean, and scaling means dividing by its standard deviation. 

Mathematically, normalization can be expressed as: 𝑍 = (𝑋 − 𝑥̅) / 𝜎 

In Python, element-wise mean and element-wise standard deviation can be obtained by using .mean() and .std() calls. 

##### In this problem, a random 5 x 5 ndarray is to be created and stored into variable X. Normalize X. The normalized ndarray is to be saved as X_normalized.npy

#### **Normalization Code**

``` js
import numpy as np #import numpy

X = np.random.rand(5,5) #create the 5x5 matrix

mean = X.mean() #calculate the mean
std = X.std() #calculate the standard deviation

X_normalized = (X - mean) / std #normalization formula

np.save('X_normalized.npy', X_normalized) #save the array

print("Original array (X):\n", X) #print the values
print("\nNormalized array (X_normalized): \n", X_normalized)
```

##### *Sample Result when running the code:*
![Screenshot 2024-09-10 020049](https://github.com/user-attachments/assets/5d24ce57-3b9a-4a32-8e22-a3af33538cfe)
\
