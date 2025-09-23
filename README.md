# ECE2112 PA2
This repository belongs to Lanz Jeremy M. Santos of 2ECE-C, and it contains the Performance Assessment 2 for Advanced Computer Programming and Algorithms course.

# NORMALIZATION PROBLEM
- create a random 5 x 5 ndarray and store it to variable X. Normalize X. Save your normalized ndarray as X_normalized.npy

To start the numerical python code, we need to import the numpy library to access built in numerical python codes.

```python
import numpy as np #imports the numpy library to access numerical python codes.
```
<br />

The task is to create a random 5 x 5 ndarray and store it to variable X. Normalize X. Save the normalized ndarray as X_normalized.npy

We use the following codes to accomplish the requirements.

**CODES**

np.random.rand(n, n) - creates a random 5x5 ndarray where we use (row, column)

X.mean - where X is the variable used and .mean is a built in code to access the average of an input

X.std - where .std is the standard deviation

np.save - save the data into a file

<br />


**COMPILE THE CODES**

<br />

```python
X = np.random.rand(5, 5) #creates a random 5 x 5 ndarray
X_normalized = (X - X.mean()) / X.std() #computes the normalization problem using the normalization equation and storing it to "X_normalized"
np.save("X_normalized.npy", X_normalized) #saves the X_normalized data to "X_normalized.npy"
print("Original X:\n", X) #prints the original and not normalized X
print("\nMean:", mean, "Std Dev:", std) #prints the mean and the standard deviation of the ndarray
print("\nNormalized X:\n", X_normalized) #prints the final output "X_normalized"
```

<br />

**RESULT**

<br />

<img width="597" height="324" alt="image" src="https://github.com/user-attachments/assets/ad561ca9-bcf8-4650-8e05-0ab607c48e31" />

<br />
<br />

# DIVISIBLE BY 3 PROBLEM

The task is to create a 10x10 ndarray with the squares of the first 100 integers and then print the numbers that are divisible by 3

We use the following codes to accomplish the requirements:

**CODES**

np.arange(1, 101) – generates integers from 1 to 100.

** 2 – squares each integer in the sequence.

.reshape(10, 10) – reshapes the squared numbers into a 10 × 10 ndarray.

A % 3 == 0 – checks divisibility by 3.

np.save – saves the divisible numbers into a file.

<br />

**COMPILE THE CODES**

<br />

```python
squares = np.arange(1, 101) ** 2 # Generate squares of first 100 positive integers
A = squares.reshape(10, 10) #reshapes into a 10x10 ndarray with the squares of the first 100 integers
div_by_3 = A[A % 3 == 0] #selects elements from A that are divisible by 3
np.save("div_by_3.npy", div_by_3) #saves the divisible numbers into "div_by_3.npy"

print("10x10 Array A:\n", A) #prints the original array of squared numbers
print("\nElements divisible by 3:\n", div_by_3) #prints only the numbers divisible by 3
```

<br />

**RESULT**

<br />

<img width="680" height="348" alt="image" src="https://github.com/user-attachments/assets/c402f1d7-a541-4499-95f9-9c913281bab9" />

<br />

# END

**Thank you for reading my README file! If you want to see my jupyter notebook code, just access it through the attached file "SANTOS_PA2.ipynb" in the same repository as this README file.**

<br />

**VERSION HISTORY**

first version: Sep 9, 2025

current version: Sep 23, 2025

(changed whole readme and changed format into more detailed line by line explanation)
