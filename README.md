# Experiment 9: Study of the NumPy Library

**Author:** Ronit Mehta  
**PRN:** 25070123094  


---

## AIM
To study and implement the **NumPy** (Numerical Python) library, understand its core functionalities, and perform various array creations, inspections, and numerical operations.

---

## Theory & Command Reference

### Why NumPy?
NumPy is a fundamental package for scientific computing in Python. It is widely used because:
* **Speed:** It is significantly faster than standard Python lists due to C-level optimization.
* **Utility:** It is strictly designed for high-performance numerical operations.
* **Foundation:** It serves as the base data structure for other essential data science libraries, such as Pandas.

### 1. Array Creation
NumPy's core object is the highly optimized multi-dimensional array, `ndarray`.
* `import numpy as np`: Standard convention to import the NumPy library.
* `np.array([list])`: Converts a standard Python list (or nested lists) into a 1D, 2D, or n-dimensional NumPy array.
* `np.zeros(shape)`: Creates a new array of specified dimensions filled entirely with zeros (e.g., `np.zeros((2,3))`).
* `np.ones(shape)`: Creates a new array of specified dimensions filled entirely with ones.
* `np.eye(N)`: Creates an `N x N` 2D identity matrix with ones on the main diagonal and zeros elsewhere.

### 2. Array Inspection & Attributes
These commands allow you to check the structural properties of an existing NumPy array.
* `.ndim`: Returns the number of dimensions (axes) of the array (e.g., 1 for a vector, 2 for a matrix).
* `.shape`: Returns a tuple indicating the size of the array in each dimension (e.g., `(rows, columns)`).
* `.dtype`: Returns the specific data type of the elements stored within the array (e.g., `int64`, `float64`).

### 3. Array Generation Functions
Functions used to generate arrays with specific sequences of numbers.
* `np.arange(start, stop, step)`: Returns an array containing evenly spaced values within a given interval. Similar to Python's built-in `range()`.
* `np.linspace(start, stop, num)`: Returns an array of `num` evenly spaced numbers over a specified interval (from `start` to `stop`). Very useful for plotting mathematical functions.

### 4. Mathematical Operations
NumPy allows for **vectorized operations**, meaning you can apply an operation to an entire array at once without writing explicit loops.
* **Scalar Operations:** Adding (`array + 5`) or multiplying (`array * 2`) a single number to an array applies that operation element-wise to every item in the matrix.

### 5. Statistical & Aggregate Functions
NumPy provides built-in methods to easily extract statistical information from arrays.
* `np.max(array)`: Finds the maximum value within the array.
* `np.min(array)`: Finds the minimum value within the array.
* `np.sum(array)`: Calculates the sum of all elements in the array.
* `np.mean(array)`: Computes the arithmetic mean (average) of the array's elements.
* `np.median(array)`: Computes the median (middle) value of the array's elements.

---

## Conclusion
In this experiment, the fundamentals of the NumPy library were successfully explored. We established that NumPy provides a highly efficient way to handle multidimensional arrays compared to standard Python lists. By utilizing built-in functions for array creation, inspection, and manipulation, we can easily perform complex mathematical and statistical operations at scale. This forms a crucial foundation for data analysis and scientific computing in Python.
