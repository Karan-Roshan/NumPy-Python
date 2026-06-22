# NumPy – Complete Learning Guide
> A comprehensive, hands-on study of **NumPy** — the fundamental package for numerical computing in Python. This repository covers everything from array creation to advanced universal functions (ufuncs), aggregate operations, broadcasting, and set operations.

## Why NumPy?
- Faster than Python lists due to C-level implementation
- Supports N-dimensional arrays and matrix operations
- Foundation for libraries like Pandas, TensorFlow, and Scikit-learn
- Efficient memory usage and vectorized computations

## Table of Contents
### 1. Introduction
- Why Use NumPy?
- Why is NumPy Faster Than Lists?
- Which Language is NumPy Written In?
- NumPy Arrays vs Python Lists

### 2. Getting Started
- Import NumPy
- Checking NumPy Version

### 3. NumPy Creating Arrays
- Create a NumPy ndarray
- **Dimensions in Arrays**
  - 0-D Arrays
  - 1-D Arrays
  - 2-D Arrays
  - 3-D Arrays
- Check Number of Dimensions
- Higher Dimensional Arrays

### 4. Creating NumPy Array (Methods)
- Creating an Array from a List
- Creating a Sequence of Numbers (`np.arange()`)
- Creating Evenly Spaced Values (`np.linspace()`)
- Creating Logarithmically Spaced Values (`np.logspace()`)
- Creating an Array of Zeros (`np.zeros()`)
- Creating an Array of Ones (`np.ones()`)
- Creating an Array with a Constant Value (`np.full()`)
- Creating an Empty Array (`np.empty()`)

### 5. Creating Random NumPy Arrays
- `np.random.rand()` — Uniform distribution [0, 1)
- `np.random.randn()` — Standard normal distribution
- `np.random.randint()` — Random integers
- `np.random.random()` — Random floats
- `np.random.choice()` — Random sampling

### 6. NumPy Array Indexing
- Access Array Elements
- Access 2-D Arrays
- Access 3-D Arrays
- Negative Indexing

### 7. NumPy Array Slicing
- Slicing Arrays
- Negative Slicing
- STEP in Slicing
- Slicing 2-D Arrays
- `np.take()`

### 8. NumPy Data Types
- Data Types in Python
- Data Types in NumPy
- Checking the Data Type (`.dtype`)
- Creating Arrays With a Specific Data Type

### 9. Type Casting
- Converting Data Type of Existing Arrays
- What if a Value Cannot Be Converted?

### 10. NumPy Array Attributes
- `ndim` — Number of Dimensions
- `shape` — Shape of the Array
- `size` — Total Number of Elements
- `dtype` — Data Type of Elements
- `itemsize` — Size of Each Element
- `nbytes` — Total Memory Consumed

### 11. Copy vs View
- Difference Between Copy and View
  - COPY — `.copy()`
  - VIEW — `.view()`
- Check if Array Owns its Data

### 12. Array Reshaping
- Reshaping Arrays
- Reshape From 1-D to 2-D
- Reshape From 1-D to 3-D
- Unknown Dimension (`-1`)
- Flattening the Arrays

### 13. Array Ravel & Flatten
- Array Ravel (`np.ravel()`)
- Flatten (`.flatten()`)
- `ravel()` vs `flatten()` in NumPy

### 14. ➗ Arithmetic Operations in NumPy
- Addition (`+`)
- Subtraction (`-`)
- Multiplication (`*`)
- Division (`/`)
- Floor Division (`//`)
- Modulus (`%`)
- Exponentiation (`**`)

### 15. Array Iterating
- Iterating Arrays
- Using `nditer()`
- Using `ndenumerate()` Function

### 16. Transpose of a Matrix
- Using `.T` Attribute
- Using `np.transpose()`
- `swapaxes()` Function

### 17. Joining Array
- Using `concatenate()` Function
- **Using Stack Functions**
  - Stacking Along Rows
  - Stacking Along Columns
  - Stacking Along Height (`np.dstack()`)

### 18. Splitting Array
- `np.split()`
- `np.array_split()`
- `np.hsplit()` — Horizontal Split
- `np.vsplit()` — Vertical Split

### 19. Repeating Arrays
- **`np.repeat()`**
  - Different Repetitions
  - Repeat with 2D Arrays
  - Repeat Along Rows (`axis=0`)
  - Repeat Along Columns (`axis=1`)
- `np.tile()`

### 20. Searching Arrays
- Searching Arrays (`np.where()`)
- Search Sorted (`np.searchsorted()`)
  - Search From the Right Side

### 21. Sorting Arrays
- Sorting Arrays (`np.sort()`)
- Sorting a 2-D Array

### 22. Filter Array
- Filtering Arrays
- Creating the Filter Array
- Creating Filter Directly from Array

### 23. Aggregate Functions
- Sum of Elements — `np.sum()`
- Mean (Average) — `np.mean()`
- Median — `np.median()`
- Maximum Value — `np.max()`
- Minimum Value — `np.min()`
- Standard Deviation — `np.std()`
- Variance — `np.var()`
- Percentiles — `np.percentile()`
- **Aggregate Functions on 2-D Arrays**
  - Sum of All Elements
  - Row-wise Sum (`axis=1`)
  - Column-wise Sum (`axis=0`)
- Cumulative Sum (`np.cumsum()`)
- Cumulative Product (`np.cumprod()`)

### 24. Advanced Logical Operations
- Logical AND — `np.logical_and()`
- Logical OR — `np.logical_or()`
- Logical NOT — `np.logical_not()`
- Logical XOR — `np.logical_xor()`

### 25. Broadcasting in NumPy
- Broadcasting Rules in NumPy
  - Rule 1: Dimensions are Compatible
  - Rule 2: One Dimension is 1
  - Rule 3: Dimensions are Different

### 26. Vectorization
- What is Vectorization?
- Vectorization vs Loops

### 27. Dealing with Missing Values
- Detect Missing Values

---

## NumPy ufuncs (Universal Functions)
> Universal functions (ufuncs) are NumPy functions that operate element-wise on arrays, enabling fast vectorized computations.

### 28. Introduction to ufuncs
- What are ufuncs?
- What is Vectorization?
- Create Your Own ufunc
  - How To Create Your Own ufunc
  - Check if a Function is a ufunc

### 29. Simple Arithmetic (ufuncs)
- Addition
- Subtraction
- Multiplication
- Division
- Power
- Remainder
- Quotient and Mod
- Absolute Values

### 30. Rounding Decimals (ufuncs)
- Truncation
- Rounding
- Floor
- Ceil

### 31. Logs (ufuncs)
- Log at Base 2 (`np.log2()`)
- Log at Base 10 (`np.log10()`)
- Natural Log / Log at Base e (`np.log()`)

### 32. Summations (ufuncs)
- Summation Over an Axis
- Cumulative Sum

### 33. Products (ufuncs)
- Product Over an Axis
- Cumulative Product

### 34. Differences (ufuncs)
- `np.diff()`

### 35. LCM — Lowest Common Multiple
- Finding LCM in Arrays (`np.lcm.reduce()`)

### 36. GCD — Greatest Common Divisor
- Finding GCD in Arrays (`np.gcd.reduce()`)

### 37. Trigonometric Functions (ufuncs)
- Convert Degrees Into Radians
- Convert Radians to Degrees
- Finding Angles (arcsin, arccos, arctan)
- Angles of Each Value in an Array
- Hypotenuse (`np.hypot()`)

### 38. Hyperbolic Functions (ufuncs)
- Finding Angles (sinh, cosh, tanh)
- Angles of Each Value in an Array

### 39. Set Operations (ufuncs)
- Create Sets in NumPy (`np.unique()`)
- Finding Union (`np.union1d()`)
- Finding Intersection (`np.intersect1d()`)
- Finding Difference (`np.setdiff1d()`)
- Finding Symmetric Difference (`np.setxor1d()`)

---

## Tech Stack
<table>
  <tr>
    <th>Tool</th>
    <th>Purpose</th>
  </tr>
  <tr>
    <td>Python 3.x</td>
    <td>Programming Language</td>
  </tr>
  <tr>
    <td>NumPy</td>
    <td>Numerical Computing</td>
  </tr>
  <tr>
    <td>Jupyter Notebook</td>
    <td>Interactive Development</td>
  </tr>
</table>
---

## Getting Started
```bash
# Clone the repository
git clone https://github.com/your-username/numpy-complete-guide.git

# Install NumPy
pip install numpy

# Launch Jupyter Notebook
jupyter notebook
```

---

## Who Is This For?
- Beginners learning NumPy from scratch
- Data Science / ML aspirants building foundations
- Interview preparation for data roles
- Anyone wanting a structured NumPy reference
