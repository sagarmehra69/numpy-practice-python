# NumPy Assignment

This repository contains a Jupyter Notebook demonstrating fundamental **NumPy operations** used in data analysis and scientific computing. The notebook explores how NumPy arrays work and compares their performance with Python lists while showcasing common operations such as indexing, slicing, reshaping, stacking, and concatenation.

---

## 📌 Overview

NumPy is a powerful Python library for numerical computing. It provides high-performance multidimensional arrays and tools to manipulate them efficiently.

This notebook demonstrates:

* Creating NumPy arrays
* Understanding dimensions and shapes
* Data types and array properties
* Indexing and slicing
* Reshaping arrays
* Flattening arrays
* Copy vs View (memory behavior)
* Stacking and concatenation
* Append, insert, and delete operations
* Performance comparison between Python lists and NumPy arrays

---

## 📦 Technologies Used

* Python
* NumPy
* Jupyter Notebook

---

## 🧮 Array Creation

```python
import numpy as np

arr = np.array([1, 2, 3])
print(arr)
```

Create arrays of different dimensions:

```python
a = np.array(10)
b = np.array([1,2,3])
c = np.array([[1,2,3],[4,5,6]])
d = np.array([[[1,2,3],[4,5,6]],[[7,8,9],[10,11,12]]])
```

---

## 📊 Array Properties

```python
print(a.ndim)
print(b.ndim)
print(c.shape)
print(c.dtype)
print(type(c))
```

These operations help understand the **structure and data type of arrays**.

---

## ⚡ NumPy vs Python Lists

NumPy operations are faster than traditional Python loops.

```python
l1 = [10,20,30]
l2 = [40,50,60]

[i*j for i,j in zip(l1,l2)]
```

Using NumPy:

```python
arr1 = np.array(l1)
arr2 = np.array(l2)

arr1 * arr2
```

---

## 🔢 Creating Arrays with `arange`

```python
np.arange(1,11)
np.arange(1,11,2)
```

Create identity matrix:

```python
np.eye(3)
```

---

## 🔄 Reshaping Arrays

```python
x = np.arange(1,17)
x.reshape(4,4)
```

Convert to 3D array:

```python
x.reshape(2,4,2)
```

---

## 📉 Flattening Arrays

```python
y.flatten()
```

Flatten converts multi-dimensional arrays into **1D arrays**.

---

## 🔍 Indexing Arrays

```python
a = np.array([2,4,6,8,10])

print(a[2])
print(a[[1,3]])
```

---

## ✂️ Slicing Arrays

```python
arr = np.array([1,2,3,4,5,6,7,8])

print(arr[1:5])
print(arr[:4])
print(arr[::2])
```

---

## 🧱 2D Array Indexing

```python
a = np.array([
    [1,2,3],
    [4,5,6],
    [7,8,9]
])

print(a[2,2])
```

---

## 🧠 Copy vs View

### View (shares memory)

```python
x = np.array([1,2,3])
y = x.view()
```

### Copy (independent memory)

```python
z = x.copy()
```

---

## 📚 Stacking Arrays

Horizontal stack:

```python
np.hstack((x,y))
```

Vertical stack:

```python
np.vstack((x,y))
```

---

## 🔗 Concatenation

```python
np.concatenate((arr1, arr2))
```

---

## ➕ Append, Insert, Delete

Append elements:

```python
np.append(arr1, arr2)
```

Insert element:

```python
np.insert(arr1, 2, 100)
```

Delete element:

```python
np.delete(arr1, 2)
```

---

## 🎯 Learning Outcomes

After completing this assignment you will understand:

* Core NumPy array operations
* Working with multi-dimensional arrays
* Efficient data manipulation
* Memory management with view and copy
* Performance benefits of NumPy

---

## 👨‍💻 Author

Sagar
