# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np
N=np.array(eval(input()))
print("Given array\n",N)
arr=np.sort(N,axis=0)
print(f"\n{arr}")
```
## Output

![image](https://github.com/user-attachments/assets/5ece9fcc-9f22-419a-84ff-6148fa8e2c4b)

## Result

The program successfully sorts the columns of the 2D NumPy array in ascending order.
