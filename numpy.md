### **NumPy in Python**
**NumPy (Numerical Python)** is a powerful library in Python used for numerical computing. It provides efficient support for working with **arrays, matrices, mathematical operations, and scientific computing**.

---

## **🔹 Why Use NumPy?**
1. **Faster than Python lists** – NumPy arrays are stored in contiguous memory, making operations **faster and more efficient**.
2. **Uses less memory** – NumPy arrays require **less space** compared to Python lists.
3. **Supports vectorized operations** – Perform operations on entire arrays at once (avoids slow Python loops).
4. **Built-in mathematical functions** – Includes functions for **linear algebra, statistics, Fourier transforms, and more**.
5. **Works well with other libraries** – Used in **Pandas, SciPy, Scikit-Learn, TensorFlow, etc.**.

---

## **🔹 Installing NumPy**
If you haven’t installed NumPy yet, you can do so using:
```bash
pip install numpy
```

---

## **🔹 Creating a NumPy Array**
### **1️⃣ Creating a 1D Array**
```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])
print(arr)
```
📌 **Output:**  
```
[1 2 3 4 5]
```

### **2️⃣ Creating a 2D Array (Matrix)**
```python
matrix = np.array([[1, 2, 3], [4, 5, 6]])
print(matrix)
```
📌 **Output:**
```
[[1 2 3]
 [4 5 6]]
```

### **3️⃣ Checking Array Shape & Data Type**
```python
print(matrix.shape)   # (2, 3) -> 2 rows, 3 columns
print(matrix.dtype)   # int64 (depends on system)
```

---

## **🔹 NumPy Array Operations**
### **1️⃣ Basic Math Operations**
NumPy allows you to perform operations directly on arrays **without using loops**.

```python
arr = np.array([1, 2, 3, 4])
print(arr + 2)  # Adds 2 to each element
print(arr * 3)  # Multiplies each element by 3
print(arr ** 2) # Squares each element
```
📌 **Output:**
```
[3 4 5 6]
[ 3  6  9 12]
[ 1  4  9 16]
```

### **2️⃣ Matrix Operations**
```python
A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])

print(A + B)  # Matrix addition
print(A @ B)  # Matrix multiplication
print(np.dot(A, B))  # Alternative for matrix multiplication
```

---

## **🔹 Useful NumPy Functions**
### **1️⃣ Create Arrays with Zeros, Ones, and Random Numbers**
```python
print(np.zeros((2, 3)))   # 2x3 matrix filled with zeros
print(np.ones((3, 3)))    # 3x3 matrix filled with ones
print(np.random.rand(2, 2))  # 2x2 matrix with random values between 0 and 1
```

### **2️⃣ Generating Sequences (Like Python `range()`)**
```python
print(np.arange(1, 10, 2))  # [1 3 5 7 9]
print(np.linspace(0, 1, 5)) # [0.   0.25 0.5  0.75 1. ]
```

### **3️⃣ Reshaping Arrays**
```python
arr = np.array([1, 2, 3, 4, 5, 6])
print(arr.reshape(2, 3))  # Reshape into a 2x3 matrix
```

---

## **🔹 NumPy and Indexing**
### **1️⃣ Indexing and Slicing**
```python
arr = np.array([10, 20, 30, 40, 50])
print(arr[0])      # First element
print(arr[1:4])    # Elements from index 1 to 3
print(arr[::-1])   # Reverse the array
```

### **2️⃣ Indexing in 2D Arrays**
```python
matrix = np.array([[1, 2, 3], [4, 5, 6]])
print(matrix[0, 1])   # Row 0, Column 1 -> Output: 2
print(matrix[:, 0])   # First column of all rows -> Output: [1 4]
```

---

## **🔹 NumPy and Pandas**
NumPy is heavily used in **Pandas** for handling data efficiently.

```python
import pandas as pd

df = pd.DataFrame(np.random.rand(5, 3), columns=['A', 'B', 'C'])
print(df)
```

---

## **🔹 Summary**
| Feature         | NumPy |
|----------------|------------------|
| Data Type      | Uses `ndarray` for fast computations |
| Performance    | Faster than Python lists |
| Memory Usage   | More efficient than lists |
| Operations     | Supports vectorized operations |
| Libraries      | Used in Pandas, SciPy, TensorFlow, etc. |

🚀 **NumPy is the backbone of numerical computing in Python.**  
