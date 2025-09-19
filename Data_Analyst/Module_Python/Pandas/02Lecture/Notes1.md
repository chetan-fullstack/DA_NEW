#  Lecture 2 – DataFrame Operations & Data Cleaning in Pandas

##  Learning Objectives
By the end of this lecture, you will be able to:  
- Select rows and columns in different ways.  
- Filter and sort data.  
- Add or remove columns.  
- Handle missing values (NaN).  
- Remove duplicates.  
- Perform basic data cleaning operations.  

---

## Theory (Explanation)

### 1. Selecting Rows & Columns
- `df['column']` → Select a column  
- `df[['col1','col2']]` → Select multiple columns  
- `df.loc[0]` → Select row by label/index  
- `df.iloc[0]` → Select row by position  
- `df.loc[0:5, ['col1','col2']]` → Slice rows & columns  

### 2. Filtering Data
```python
df[df['salary'] > 50000]
df[(df['age'] > 25) & (df['city'] == 'Delhi')]
```

### 3. Sorting Data
```python
df.sort_values('salary', ascending=False)
```

### 4. Adding & Removing Columns
```python
df['bonus'] = df['salary'] * 0.10
df.drop('bonus', axis=1, inplace=True)
```

### 5. Handling Missing Values
```python
df.isnull().sum()
df['salary'].fillna(df['salary'].mean(), inplace=True)
df.dropna(inplace=True)
```

### 6. Removing Duplicates
```python
df.drop_duplicates(inplace=True)
```

---

##  Code Example
```python
import pandas as pd

# Sample DataFrame
data = {
    'Name': ['Amit', 'Priya', 'Rahul', 'Sneha', 'Amit'],
    'Age': [25, 30, None, 28, 25],
    'City': ['Delhi', 'Mumbai', 'Delhi', None, 'Delhi'],
    'Salary': [50000, 60000, 55000, None, 50000]
}

df = pd.DataFrame(data)

print("Original DataFrame:\n", df)

# Select columns
print(df[['Name', 'Salary']])

# Filter data
print(df[df['Salary'] > 52000])

# Handle missing values
df['Salary'].fillna(df['Salary'].mean(), inplace=True)

# Remove duplicates
df.drop_duplicates(inplace=True)

print("Cleaned DataFrame:\n", df)
```

---

##  Practical Tasks (Assignments)
1. Select only the `Name` and `City` columns.  
2. Filter employees with `Salary > 55000`.  
3. Sort the DataFrame by `Age` in descending order.  
4. Fill missing `Age` with the average age.  
5. Remove duplicate rows from the dataset.  
