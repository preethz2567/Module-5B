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
