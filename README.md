# Experiment 8: Tools for Exploratory Data Analysis - NumPy

## Author
- **Name:** Pushpak J  
- **PRN:** 25070123148  
- **Branch:** F.Y. E&TC (2025-29)  
- **Batch:** A1  
- **Subject:** Exploratory Data Analysis With Python  

---

## Title
Tools for Exploratory Data Analysis - NumPy

---

## Aim
To study and implement the NumPy library in Python and perform various numerical, multidimensional, and statistical operations for Exploratory Data Analysis.

---

## Objectives
- Understand the architectural concept of N-dimensional arrays (ndarrays)  
- Explore memory management and contiguous storage in numerical computing  
- Perform advanced array creation and property inspection  
- Apply mathematical, vectorized, and broadcasting operations  
- Understand the difference between array views and deep copies  
- Apply statistical methods and linear algebra for data insights  

---

## Theory on NumPy
NumPy (Numerical Python) is the foundational package for scientific computing in Python. It provides a powerful N-dimensional array object, broadcasting functions, and tools for integration with C/C++ and Fortran. At its core is the **ndarray**, which encapsulates n-dimensional arrays of homogeneous data types.

### Architecture of ndarray
- Python lists store fragmented memory (pointers to objects).  
- NumPy arrays store data in **contiguous memory blocks**, enabling faster access via pointer arithmetic.  

### Characteristics of NumPy
- **Vectorization:** Replace explicit loops with array expressions for speed.  
- **Homogeneity:** All elements share the same data type.  
- **Striding:** Defines how NumPy moves through memory.  
- **Broadcasting:** Allows arithmetic between arrays of different shapes.  
- **Axis and Rank:** Dimensions are called axes; number of axes is the rank.  

---

## Core Operations

### 1. Memory Management: Views vs Copies
- Slicing creates a **view** (shares memory with original).  
- Use `.copy()` for independent arrays.  

### 2. Universal Functions (ufuncs)
Operate element-wise on arrays. Examples:  
```python
import numpy as np
arr = np.array([1, 2, 3])
print(np.add(arr, 5))   # [6 7 8]
print(np.sin(arr))      # [0.84 0.91 0.14]
3. Advanced Indexing
Fancy Indexing: Access multiple elements using index arrays.

Boolean Indexing: Filter data using conditions.

python
data = np.array([10, -5, 20, -2])
print(data[data > 0])   # [10 20]
NumPy in the Data Science Ecosystem
Pandas: DataFrames built on NumPy arrays

Scikit-learn: Uses NumPy arrays for ML models

Matplotlib: Requires NumPy arrays for plotting

SciPy: Extends NumPy with advanced algorithms

Applications of NumPy in EDA
Dimensionality Reduction: PCA, SVD

Noise Filtering: Fourier Transforms

Data Transformation: Normalization, scaling

Simulation: Random data generation for hypothesis testing

Conclusion
NumPy is the backbone of numerical computing in Python.

Provides efficient memory management through contiguous storage

Boosts performance via vectorization

Handles complex multidimensional structures with simple syntax
Its integration with other libraries makes it indispensable for Exploratory Data Analysis and scientific computing.
