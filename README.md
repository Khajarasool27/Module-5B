NumPy Program: Column-wise Sorting of a 2D Array
🎯 Aim
To write a NumPy program that sorts the elements in each column of a given 2D array in ascending order.

🧠 Algorithm
Import NumPy: Start by importing the NumPy library.
Get Input: Accept a 2D NumPy array from the user.
Sort Column-wise: Use the np.sort() function with axis=0 to sort each column in ascending order.
Store Result: Store the sorted result in a new array.
Display Output: Print the original array and the column-wise sorted array.
🧾 Program
import numpy as np
N=np.array(eval(input()))
print("Given array\n",N)
arr=np.sort(N,axis=0)
print(f"\n{arr}")
Output
image

Result
The program successfully sorts the columns of the 2D NumPy array in ascending order.

# NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y
🎯 Aim
To write a Python program using NumPy that finds the indices where elements in array x are greater than or equal to their corresponding elements in array y.

🧠 Algorithm
Import NumPy: Import the NumPy library.
Define Arrays: Define two NumPy arrays, x and y, with the same shape (i.e., same number of elements).
Use Boolean Indexing:
x > y gives a boolean array where elements of x are greater than y.
x == y gives a boolean array where elements of x are equal to y.
Find Indices: Use np.where() to get the indices where the conditions x >= y are satisfied.
Print Indices: Print the indices where the condition holds true.
🧾 Program
import numpy as np
x=eval(input())
y=eval(input())
l1=np.array(x)
l2=np.array(y)

print(np.where(l1>l2))
print(np.where(l1==l2))
Output
image

Result
This program successfully identifies and prints the indices where the elements of x are greater than or equal to those in y

NumPy Program: Replace the Second Column in a 2D Array
🎯 Aim
To write a NumPy program that deletes the second column from a given 2D array and inserts a new column at the same position.

🧠 Algorithm
Import NumPy: Start by importing the NumPy library.
Get Input: Get a 2D NumPy array and a new column (as another array) from the user.
Delete Column: Use np.delete() to remove the second column (index 1) from the original array.
Insert Column: Use np.insert() to insert the new column at the second column's original position.
Display Result: Print the updated array with the replaced column.
🧾 Program
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
Output
image

Result
The program successfully deletes the second column from the original 2D NumPy array and inserts a new column at the same index.

Pandas Program: Create and Display a DataFrame with Custom Index Labels
🎯 Aim
To create and display a DataFrame using the Pandas library in Python from a given dictionary, and apply specific index labels to the rows.

🧠 Algorithm
Import Libraries: Import the required libraries – pandas and numpy.
Create Dictionary: Define a dictionary exam_data with keys: 'name', 'score', 'attempts', and 'qualify'.
Index Labels: Create a list of custom index labels called labels.
Create DataFrame: Use pd.DataFrame() to create the DataFrame by passing the dictionary and index labels.
Display Output: Display the DataFrame using print() or by simply calling the DataFrame variable.
💻 Program
import pandas as pd
import numpy as np
exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura',
'Kevin', 'Jonas'],
 'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
 'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
 'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']
df = pd.DataFrame(exam_data , index=labels)
print(df)
Output
image

Result
The program successfully creates and displays a Pandas DataFrame using the provided dictionary and applies the specified row index labels ('a' to 'e'). The score column demonstrates how NaN values are handled (for missing data like in James's case).

🧪 Pandas Program: Join Two DataFrames Along Rows
🎯 AIM
To write a Python program using Pandas to join two DataFrames along rows (row-wise concatenation) and assign all data to a new DataFrame.

🧠 ALGORITHM
Import Libraries: Import the pandas library.
Create First DataFrame: Use a dictionary to create student_data1.
Create Second DataFrame: Use another dictionary to create student_data2.
Concatenate DataFrames: Use pd.concat() with axis=0 to concatenate both DataFrames row-wise.
Display Result: Print the new combined DataFrame.
💻 Program
import pandas as pd
data1 = {'s_id': ['S1', 'S2', 'S3', 'S4', 'S5'],
         'name': ['Dan', 'Ryder', 'Bryce', 'Bernal', 'Kwame'],
         'marks': [200, 210, 190, 222, 199]}
df1 = pd.DataFrame(data1)
data2 = {'s_id': ['S4', 'S5', 'S6', 'S7', 'S8'],
         'name': ['Scart', 'Willy', 'Dani', 'Kaise', 'Madeeha'],
         'marks': [201, 200, 198, 219, 201]}
df2 = pd.DataFrame(data2)
print("Original DataFrames:")
print(df1)
print("-" * 37)
print(df2)
result = pd.concat([df1, df2], axis=1)
print("\nJoin the said two dataframes along columns:")
print(result)
Output
image

Result
The program successfully joins two DataFrames row-wise using pd.concat() and assigns the result to a new DataFrame.
