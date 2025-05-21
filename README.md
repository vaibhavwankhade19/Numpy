📘 NumPy Theory Notes

1️⃣ Basics of NumPy

NumPy (Numerical Python) is a powerful Python library for numerical and scientific computing.

It provides:

High-performance n-dimensional array object (ndarray)
Tools for integrating C/C++ code
Functions for mathematical, logical, and statistical operations
NumPy arrays are faster and more memory efficient than Python lists.


2️⃣ Array Creation

Methods to create arrays:
import numpy as np
| Method                          | Description                      |
| ------------------------------- | -------------------------------- |
| `np.array()`                    | Converts a list/tuple to ndarray |
| `np.zeros((r,c))`               | Creates array filled with 0s     |
| `np.ones((r,c))`                | Filled with 1s                   |
| `np.eye(n)`                     | Identity matrix                  |
| `np.arange(start, stop, step)`  | Range array                      |
| `np.linspace(start, stop, num)` | Evenly spaced numbers            |
| `np.reshape()`                  | Reshape array dimensions         |


3️⃣ Common NumPy Functions
| Function                       | Description            |
| ------------------------------ | ---------------------- |
| `np.sum(arr)`                  | Sum of all elements    |
| `np.mean(arr)`                 | Mean (average)         |
| `np.std(arr)`                  | Standard deviation     |
| `np.min(arr)` / `np.max(arr)`  | Min/Max values         |
| `np.cumsum()` / `np.cumprod()` | Cumulative sum/product |
| `np.sort()`                    | Sort elements          |
| `np.unique()`                  | Unique values          |


4️⃣ Mathematical & Logical Operations
Element-wise operations:
a + b, a - b, a * b, a / b, a ** 2

Logical comparison:
a > 5, a == b

Matrix operations:
np.dot(a, b), np.transpose(a), np.linalg.inv(a)


5️⃣ Slicing and Indexing
1D Slicing: a[1:4], a[::-1], a[::2]

2D Slicing:

a[i, j]         # Single element
a[i, :]         # Row
a[:, j]         # Column
a[1:3, 1:3]     # Sub-matrix

6️⃣ Concatenation and Splitting
Concatenation:
np.concatenate((a, b), axis=0)  # Row-wise
np.concatenate((a, b), axis=1)  # Column-wise
np.vstack((a, b)), np.hstack((a, b))


Splitting:
np.split(arr, 3)
np.vsplit(arr, 2)
np.hsplit(arr, 2)


7️⃣ Trigonometric Functions

np.sin(), np.cos(), np.tan()	Trigonometric values (input in radians)
np.arcsin(), np.arccos(), np.arctan()	Inverse trigonometric
np.radians(), np.degrees()	Convert degrees ↔ radians

8️⃣ Random Sampling
Use numpy.random for generating random numbers:

np.random.rand(n)         # Uniform dist [0, 1)
np.random.randn(n)        # Standard normal dist
np.random.randint(low, high, size)  # Random integers
np.random.choice(arr)     # Random pick
np.random.shuffle(arr)    # Shuffle array


9️⃣ String Operations, Comparisons & Info
🔤 String Operations (np.char)

np.char.add(a, b)          # Concatenate strings
np.char.upper(a), np.char.lower(a)
np.char.split(a), np.char.replace(a, 'old', 'new')

✅ Comparison Operations
a == b, a > b, a != b
np.array_equal(a, b)

ℹ️ Information About Arrays

a.shape         # Shape (rows, columns)
a.ndim          # Dimensions
a.size          # Total number of elements
a.dtype         # Data type
a.itemsize      # Byte size of each element

