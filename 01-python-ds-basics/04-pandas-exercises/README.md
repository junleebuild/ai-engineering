# Pandas Exercises – SF Salaries & Ecommerce Purchases

## 🔍 Overview

This folder includes two hands-on Pandas exercises that focus on reading real-world datasets, performing conditional queries, and analyzing structured data using Pandas' built-in methods.

---

## 📘 01 – SF Salaries Exercise

**Dataset**: `Salaries.csv`  
**Objective**: Practice loading CSV files using Pandas and performing various data inspection and aggregation operations.

### 🔹 Key Concepts Covered:
- Loading CSV data with `pd.read_csv()`
- Exploring structure with `df.head()` and `df.info()`
- Computing statistical summaries:
  - `.mean()`, `.max()`, `.min()` for specific columns
- Conditional filtering based on column values
- Counting and summarizing unique data:
  - `.unique()` → list of unique values  
  - `.nunique()` → number of unique values  
  - `.value_counts()` → frequency of each value  
  - `.count()` → total number of non-null entries

This exercise highlighted the importance of choosing the correct method when analyzing unique values vs counts.

---

## 📘 02 – Ecommerce Purchases Exercise

**Dataset**: `Ecommerce Purchases`  
**Objective**: Extract insights from a semi-structured ecommerce dataset using conditional filtering and value-based operations.

### 🔹 Key Concepts Covered:
- Reading CSV files with unusual filenames and verifying structure
- Filtering data based on string values (e.g., job titles, email providers)
- Counting results based on specific conditions
- Understanding how Pandas handles data types in queries

Despite the file not having a typical `.csv` extension, `pd.read_csv()` handled it seamlessly, showing Pandas' robustness.

---

## 💬 Reflection

These exercises helped reinforce practical techniques for loading, inspecting, and filtering data with Pandas.  
Learning to distinguish between `.unique()`, `.nunique()`, `.value_counts()`, and `.count()` was especially important for accurate data profiling.  
It also showed that Pandas is capable of handling even non-standard data formats effectively.  
Most importantly, this solidified my understanding of how to extract meaningful insights from structured datasets using intuitive, Pythonic syntax.

---

## 📂 Files

| File | Description |
|------|-------------|
| `01-my SF salaries exercise.ipynb` | My full solution to the SF Salaries dataset |
| `02-ref SF salaries exercise solutions.ipynb` | Instructor-provided reference solution |
| `03-my ecommerce purchases exercise.ipynb` | My completed Ecommerce Purchases exercise |
| `04-ref ecommerce purchases exercise solutions.ipynb` | Instructor reference for Ecommerce exercise |
| `Salaries.csv` | Source dataset for Exercise 1 |
| `Ecommerce Purchases` | Source dataset for Exercise 2 |