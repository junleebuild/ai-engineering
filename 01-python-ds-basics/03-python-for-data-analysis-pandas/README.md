# Pandas Basics (Section 03)

## 🔍 Overview

In this section, I began learning the **Pandas** library, one of the most important tools for data analysis in Python.  
Pandas builds upon NumPy and adds labeled data structures that make handling, selecting, and filtering data much more intuitive and powerful.

## ✅ Topics Covered

### 🔹 Series
- Pandas `Series` is a one-dimensional labeled array, similar to a NumPy array.
- Can be created using `pd.Series(data)` and optionally customized with `index` (label) arguments.
- Arithmetic operations are supported between Series if their indices match.
- Visually more readable and informative than raw arrays.

### 🔹 DataFrames
- Created using `pd.DataFrame()` with custom `data`, `index`, and `columns`.
- Columns can be accessed using `df['W']`, which returns a `Series`.
- `drop()` method allows for column or row removal.
  - To update the original DataFrame: `inplace=True`
- Rows can be selected using `df.loc['C']` or `df.iloc[1]`.
- Conditional filtering:  
  - `df[df > 0]` returns only positive values.  
  - Multiple conditions: `df[(df['W'] > 0) & (df['Y'] > 1)]`
- MultiIndex: Created using `pd.MultiIndex.from_tuples()` and enables hierarchical row indexing.
- `xs()` method extracts data at specific levels of MultiIndex.

## 💬 Personal Reflection

Pandas initially felt more complex than NumPy, but it’s clearly designed for real-world data analysis.  
The labeled axes, flexible selection tools, and rich structure make it a must-have skill.  
Once I get more familiar with it, I expect it to become second nature in handling data.  
Learning about `dtype`, indexing methods, and logical filtering with `&` and `|` were particularly insightful.

---

📁 Self-written notebooks:
- `01-my-series.ipynb`
- `02-my-dataframes.ipynb`

📁 Instructor references:
- `01-ref-series.ipynb`
- `02-ref-dataframes.ipynb`