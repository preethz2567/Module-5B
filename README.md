# PYHON PROGRAMMING MODULE V-B
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
