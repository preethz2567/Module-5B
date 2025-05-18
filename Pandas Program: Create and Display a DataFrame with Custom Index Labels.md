# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
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
