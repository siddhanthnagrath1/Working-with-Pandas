# 🐼 Working with Pandas - Learning and Practice

## 📘 About This Project

This repository contains a Jupyter Notebook titled `Working_with_Pandas.ipynb`, created as part of my school learning. The goal was to learn and practice core functionalities of the **Pandas** library in Python for data handling and analysis.

---

## 🏫 What I Studied in School

During my school lessons, I was introduced to the basics of data manipulation using Pandas. Here's what was covered:

- Introduction to Pandas and its use in data analysis
- Understanding Series and DataFrame objects
- Reading data from files
- Accessing, cleaning, and analyzing data
- Performing group operations and summarizing results

---

## 🧠 What I Practiced in This Notebook

### ✅ Creating Series and DataFrames

- Creating Pandas **Series** and **DataFrames** from:
  - Lists
  - Dictionaries
  - NumPy arrays

- Setting **custom index labels** for easy identification and referencing.

### ✅ Reading External Files

- Using `pd.read_csv()` to load datasets into DataFrames.

  ```python
  import pandas as pd
  df = pd.read_csv("data.csv")
  ```

### ✅ Exploring Data

- Viewing structure and summary of data using:
  - `.head()` – first few rows
  - `.tail()` – last few rows
  - `.info()` – data types and null counts
  - `.describe()` – statistical summary

  ```python
  df.head()
  df.info()
  df.describe()
  ```

### ✅ Accessing Rows and Columns

- Accessing data using:
  - `loc[]` – label-based indexing
  - `iloc[]` – position-based indexing

  ```python
  df.loc[0]       # First row by label
  df.iloc[0]      # First row by position
  df["Column"]    # Access column
  ```

- **Conditional filtering** using Boolean expressions.

  ```python
  df[df["Age"] > 25]
  ```

### ✅ Cleaning Data

- Handling missing data:
  - `.dropna()` – remove missing values
  - `.fillna()` – fill missing values with a default

  ```python
  df.dropna()
  df.fillna(0)
  ```

### ✅ Aggregating and Grouping

- Performing operations like:
  - `.groupby()` – group rows
  - `.sum()`, `.mean()` – aggregate values

  ```python
  df.groupby("Department")["Salary"].mean()
  ```

### ✅ Sorting and Renaming

- Sorting data using `.sort_values()`
- Renaming columns with `.rename()`

  ```python
  df.sort_values("Age")
  df.rename(columns={"Name": "Employee_Name"})
  ```

### ✅ (Optional) Visualization

- Basic data plotting using:
  - **Matplotlib**
  ```python
  import matplotlib.pyplot as plt
  df["Salary"].plot(kind="hist")
  plt.show()
  ```

---

## 📁 Files Included

```
├── Working_with_Pandas.ipynb
└── README.md
```

---

## ⚙️ Requirements

- Python 3.x
- pandas
- numpy
- Jupyter Notebook
- (Optional) matplotlib, seaborn

Install dependencies using:

```bash
pip install pandas numpy matplotlib seaborn
```

---

## 🎯 Learning Outcome

By completing this notebook, I was able to:

- Understand the structure and purpose of Pandas Series and DataFrames
- Load and explore datasets effectively
- Clean and prepare data for analysis
- Apply aggregation and grouping techniques
- Create basic visualizations (if applicable)

---

## 👨‍🎓 Author

**Siddhanth Nagrath**  
Student | Learning Python & Data Science  
This notebook is a part of my learning through school and self-practice.
