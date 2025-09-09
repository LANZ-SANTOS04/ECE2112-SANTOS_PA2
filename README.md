#ECE2112 PA2

# NORMALIZATION PROBLEM
- create a random 5 x 5 ndarray and store it to variable X. Normalize X. Save your normalized ndarray as X_normalized.npy

**Purpose**
Standardize the dataset so that all values are on the same scale.

**Example**
```python
X = np.random.rand(5, 5)
X_normalized = (X - X.mean()) / X.std()
np.save("X_normalized.npy", X_normalized)
print(X_normalized)
```

# DIVISIBLE BY 3 PROBLEM
- create a 10x10 ndarray with the squares of the first 100 integers and then print the numbers that are divisible by 3

**Purpose**

Build a 10×10 matrix from the squares of integers.
Apply a logical condition (divisibility by 3).
Extract or filter out values that meet this condition.
Save the results for later use.

**Example**

```python
A = (np.arange(1, 101) ** 2).reshape(10, 10)
div_by_3 = A[A % 3 == 0]
np.save("div_by_3.npy", div_by_3)
print(div_by_3)
```
