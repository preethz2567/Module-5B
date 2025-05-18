# PYTHON PROGRAMMING MODULE V-B
## NAME : PREETHI D
## REGISTER NUMBER : 212224040250

# EXP 01 -  NumPy Program: Column-wise Sorting of a 2D Array

##  Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

##  Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## Program
```
import numpy as np
array_2d = np.array([
    [12, 25, 17],
    [5,  10, 8],
    [20, 15, 2]
])

sorted_columns = np.sort(array_2d, axis=0)
print("Original 2D Array:\n", array_2d)
print("\nColumn-wise Sorted Array:\n", sorted_columns)
```

## Output
![image](https://github.com/user-attachments/assets/d900ffcf-3a08-4ad2-9456-9cc5f13e8121)

## Result
Therfore the given Python program has been executed successfully and the ouput has been verified.

# EXP 02-  NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

##  Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## Program
```
import numpy as np
x = np.array([5, 8, 10, 3, 6])
y = np.array([3, 8, 7, 4, 5])

condition = x >= y

indices = np.where(condition)

print("Array x:", x)
print("Array y:", y)
print("Indices where x >= y:", indices[0])


```

## Output
![image](https://github.com/user-attachments/assets/c28b0239-8493-4771-b5e0-d01db963c7eb)

## Result
Therefore the given Python program has been executed successfully and the output has been verified.

# EX 03 - NumPy Program: Replace the Second Column in a 2D Array

##  Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

##  Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## Program
```
import numpy as np
arr = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
])

new_column = np.array([10, 11, 12])
arr_deleted = np.delete(arr, 1, axis=1)
updated_arr = np.insert(arr_deleted, 1, new_column, axis=1)

print("Original array:\n", arr)
print("Updated array:\n", updated_arr)

```

## Output
![image](https://github.com/user-attachments/assets/6e63ba74-23de-4a99-8cea-61d8193c9285)

## Result
Therefore the given Python program has been executed succeesfully and the output has been verified.

#  EX 04-Pandas Program: Create and Display a DataFrame with Custom Index Labels

##  Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

##  Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

##  Program
```
import pandas as pd
import numpy as np
exam_data = {
    'name': ['Ananya', 'Joseph', 'Preethi', 'Ravi', 'Nila', 'Arjun', 'Deepa', 'Tom'],
    'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan],
    'attempts': [1, 3, 2, 3, 2, 3, 1, 1],
    'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no']
}

labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h']

df = pd.DataFrame(exam_data, index=labels)
print("Exam Results DataFrame:\n")
print(df)


```

## Output
![image](https://github.com/user-attachments/assets/e3590e12-afdd-47b8-b3c8-ddd7e45b0502)

## Result
Therefore the given Python program has been executed successfully and the output has been verified.
# EX 05- Pandas Program: Join Two DataFrames Along Rows

##  AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

##  ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

##  Program
```
import pandas as pd
student_data1 = {
    'name': ['Alice', 'Bob', 'Charlie'],
    'score': [85, 90, 95]
}
df1 = pd.DataFrame(student_data1)

student_data2 = {
    'name': ['David', 'Eve', 'Frank'],
    'score': [88, 92, 87]
}
df2 = pd.DataFrame(student_data2)

combined_df = pd.concat([df1, df2], axis=0)
print("Combined Student DataFrame (Row-wise Join):\n")
print(combined_df)

```

## Output
![image](https://github.com/user-attachments/assets/2cf04b0f-69e7-41e6-a3b1-71bc902d5367)


## Result
Therefore the given Python program has been executed successfully and the output has been verified.
