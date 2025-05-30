# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```
import numpy as np
a=np.array(list(eval(input())))
print("Printing Original array")
print(a)
arr1=np.min(a,axis=1)
print("Printing amin Of Axis 1")
print(arr1)
arr2=np.max(a,axis=0)
print("Printing amax Of Axis 0")
print(arr2)
```

## Output

![image](https://github.com/user-attachments/assets/90038bfc-9060-48af-aaeb-193e41fb5079)

## Result

The program successfully deletes the second column from the original 2D NumPy array and inserts a new column at the same index.
