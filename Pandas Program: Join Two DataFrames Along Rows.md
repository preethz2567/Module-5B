# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
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
