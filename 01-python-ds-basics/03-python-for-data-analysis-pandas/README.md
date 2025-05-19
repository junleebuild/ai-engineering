# Pandas Basics (Section 03)

## 🔍 Overview

In this section, I studied the **Pandas** library, which is one of the most essential tools in Python for real-world data analysis.  
It expands on NumPy’s capabilities and offers powerful structures for handling, analyzing, and transforming tabular data.

---

## ✅ Topics Covered

### 🔹 Series
- `Series` is a one-dimensional labeled array, similar to a NumPy array.
- Created using `pd.Series(data)` with optional `index` argument.
- Supports arithmetic operations when indices match.
- Output format is clean and well-structured for readability.

### 🔹 DataFrames
- Created via `pd.DataFrame(data, index, columns)`
- Columns accessed with `df['W']`, returns a Series
- Rows accessed via `df.loc['row_label']` or `df.iloc[row_index]`
- Can use conditional filtering like `df[df > 0]`
- Combine conditions with `&`, `|`, enclosed in parentheses

### 🔹 MultiIndex
- Built with `pd.MultiIndex.from_tuples(list(zip(...)))`
- Enables hierarchical indexing
- Extract sub-levels with `df.xs('label', level=...)`

### 🔹 Handling Missing Data
- Use `df.fillna(value)` to fill in missing values
- Replace NaNs with statistical values (e.g. mean, median)
- Remove missing rows/columns using `df.dropna()`

### 🔹 Grouping & Aggregation
- `df.groupby('column')` groups rows by column values
- Aggregate methods like `.sum()`, `.mean()`, `.max()` provide summary statistics
- Can group multiple levels and sort results

### 🔹 Merging, Joining, Concatenating
- `pd.concat([df1, df2], axis=...)` joins data vertically or horizontally
- `pd.merge(df1, df2, on='column')` merges on common keys
- `df1.join(df2)` joins by index; unmatched rows show `NaN` by default

### 🔹 Data Operations & Transformation
- Use `df.apply(func)` to apply a function across rows or columns
- Example: `df['col'].apply(len)`, `df['col'].apply(lambda x: x**2)`
- Sort rows by column: `df.sort_values(by='col')`

### 🔹 Data Input and Output
- Reading:
  - `pd.read_csv('file.csv')`
  - `pd.read_excel('file.xlsx')`
  - `pd.read_html('url')`
  - `pd.read_sql()`
- Writing:
  - `df.to_csv()`, `df.to_excel()`, `df.to_html()`, `df.to_sql()`

---

## 💬 Personal Reflection

Pandas initially felt more complex than NumPy due to its labeled structure and indexing mechanisms.  
However, as I worked through Series and DataFrame basics, I began to appreciate its flexibility and expressive power.

This module gave me a solid foundation in handling and analyzing structured data.  
I found the `fillna()` and `groupby()` features especially useful in real-life datasets, where missing data and aggregation are common.  
Learning the differences between `concat`, `merge`, and `join` also clarified how to combine datasets based on keys or indexes.  
Applying functions with `.apply()` opened the door to more flexible row/column operations.  
Finally, practicing importing and exporting CSV, Excel, and HTML files using Pandas made me realize how close data analysis is to actual automation.

---

## 🗂️ Self-Written Notebooks

- `01-my series.ipynb`
- `02-my dataframes.ipynb`
- `03-my missing data.ipynb`
- `04-my groupby.ipynb`
- `05-my merging-joining-concat.ipynb`
- `06-my operations.ipynb`
- `07-my data input output.ipynb`

## 📘 Instructor Reference Notebooks

- `01-ref series.ipynb`
- `02-ref dataframes.ipynb`
- `03-ref missing data.ipynb`
- `04-ref groupby.ipynb`
- `05-ref merging joining concat.ipynb`
- `06-ref operations.ipynb`
- `07-ref data input output.ipynb`

---

## 🚧 Next

The **Pandas Capstone Project** follows this section. I will complete it and commit a final version of the Pandas section tomorrow.