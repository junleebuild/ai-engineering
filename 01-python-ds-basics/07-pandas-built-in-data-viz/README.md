# Pandas Built-in Data Visualization (Section 06)

## 🔍 Overview

In this section, I learned how to visualize data directly using **Pandas' built-in plotting functions**.  
Unlike Seaborn or Matplotlib, these functions are accessible directly from a DataFrame object using `.plot()` methods, and are useful for quick exploratory visualizations.

The data used was loaded from CSV and pickled DataFrame files, and visualized with a variety of plot types using simple commands.

---

## 📌 Topics Covered

### 🔹 Basics

- Loaded CSV and `.pkl` data files using `pd.read_csv()` and `pd.read_pickle()`
- Used `df.plot()` and `df.hist()` to create fast default visualizations

### 🔹 Plot Types via `.plot(kind=...)`

- `line` – Default, simple line plot
- `area` – Stacked area chart
- `bar` – Vertical bar chart
- `barh` – Horizontal bar chart
- `hist` – Histogram (can also use `df.hist()`)
- `box` – Box-and-whisker plot
- `kde` / `density` – Kernel density estimate (smoothed curve)
- `scatter` – Scatterplot (requires `x` and `y` arguments)
- `hexbin` – 2D density heatmap (for large scatterplots)

---

## 💬 Reflection

This was the first time I used Pandas directly to create plots.  
It was much simpler than using Seaborn or Matplotlib because all I needed was `.plot(kind='...')` right on the DataFrame.  
While the customizability is more limited, it’s a great tool for quick data checks.  
I’ll probably use this for fast previews before switching to Seaborn for more polished graphs.

---

## 📂 Files

| File | Description |
|------|-------------|
| `01-pandas built-in data visualization.ipynb` | Main lecture notebook on Pandas plotting |
| `02-my pandas data visualization exercise.ipynb` | My self-written exercise notebook |
| `03-pandas data visualization exercise - solutions.ipynb` | Instructor-provided solution notebook |
| `df1`, `df2`, `df3` | Sample datasets used for plotting |

---