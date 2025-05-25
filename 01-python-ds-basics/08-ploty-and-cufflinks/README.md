# Plotly and Cufflinks Visualization (Section 07)

## 🔍 Overview

In this section, I explored interactive dashboard-style visualizations using **Plotly** in combination with **Cufflinks**.  
Cufflinks allows easy integration of Plotly with Pandas DataFrames using `.iplot()` for inline, interactive plotting.

---

## 🛠️ Setup Issues

While working with `.iplot()`, I encountered a `ValueError` related to a NumPy compatibility issue.  
This was resolved by downgrading the libraries to the following versions:

- `numpy==1.26.4`  
- `plotly==5.24.1`

After this adjustment, `iplot()` worked without any errors.

---

## 📌 Key Plot Types Used

- `iplot(kind='line')` – Basic line plot  
- `iplot(kind='bar')` – Bar chart  
- `iplot(kind='scatter')` – Scatterplot  
- `iplot(kind='box')` – Box-and-whisker plot  
- `iplot(kind='surface')` – 3D surface plot (interactive rotation)  
- `iplot(kind='hist')` – Histogram  
- `iplot(kind='bubble')` – Bubble chart

The syntax is straightforward:  
```python
df.iplot(kind='bar')
```

---

## 💬 Reflection

Plotly with Cufflinks was surprisingly simple to use, especially for building interactive plots right from Pandas DataFrames.  
The `.iplot()` method worked similarly to other plotting libraries, but with built-in support for interactive, zoomable, and hoverable charts.  
The 3D `surface` plot was the most unique and visually engaging — being able to rotate the plot made it feel like a true dashboard-level visualization.  
The only challenge was solving the version conflict with NumPy and Plotly, but once that was fixed, the experience was smooth.

---

## 📂 Files

| File | Description |
|------|-------------|
| `01-plotly and cufflinks.ipynb` | Interactive plotting using Plotly with Cufflinks |

---
