# Seaborn Basics (Section 05)

## 🔍 Overview

In this section, I studied the **Seaborn** library for statistical data visualization.  
Seaborn builds on top of Matplotlib and provides higher-level, more aesthetically pleasing visualizations.  
Compared to Matplotlib, Seaborn offers many more built-in plot types and handles DataFrame objects more naturally.

---

## 📌 Topics Covered

### 🔹 01 – Distribution Plots

- `sns.histplot()` – Histogram for univariate distribution  
- `sns.kdeplot()` – Kernel density estimation  
- `sns.displot()` – Combines histogram and KDE with facet support  
- `sns.jointplot()` – Combines scatterplot and univariate distributions  
- `sns.pairplot()` – Plots all pairwise relationships in a dataset

### 🔹 02 – Categorical Plots

- `sns.barplot()` – Bar chart with aggregation (mean by default)  
- `sns.countplot()` – Count frequencies of categorical values  
- `sns.boxplot()` – Box-and-whisker plot  
- `sns.violinplot()` – Combines boxplot with KDE  
- `sns.stripplot()` – Raw data points with jitter  
- `sns.swarmplot()` – Spread-out version of stripplot (no overlap)

### 🔹 03 – Matrix Plots

- `sns.heatmap()` – Color-coded matrix  
- `sns.clustermap()` – Heatmap with hierarchical clustering

### 🔹 04 – Grids

- `sns.FacetGrid()` – Grid of plots based on row/column facets  
- `sns.PairGrid()` – Custom pairwise plotting  
- `sns.pairplot()` – Quick, automatic pairwise plot

### 🔹 05 – Regression Plots

- `sns.regplot()` – Scatterplot with regression line  
- `sns.lmplot()` – More flexible regression plot with faceting  
- Supports `hue`, `col`, and `row` arguments for segmentation

### 🔹 06 – Style and Color

- `sns.set_style()` – Set overall style: `"white"`, `"whitegrid"`, `"dark"`, etc.  
- `sns.set_palette()` – Set color themes: `"pastel"`, `"deep"`, etc.  
- `sns.despine()` – Remove axes spines for a cleaner look

---

## 💬 Reflection

Seaborn provides many more built-in chart types than Matplotlib, but the number of options made it feel overwhelming at first.  
It became clear that memorizing the main plot functions is important, especially when switching between types like categorical or distribution plots.  
`jointplot()` and `pairplot()` were especially useful once I understood they combine both scatter and distribution views.  
The hardest part wasn't the syntax but recognizing when to use which kind of plot.  
I plan to practice more with real datasets to become comfortable choosing the right plot for the right context.

---

## 📂 Files

| File | Description |
|------|-------------|
| `01-distribution plots.ipynb` | Histograms, KDE, displot, jointplot, pairplot |
| `02-categorical plots.ipynb` | Categorical visualizations: bar, count, box, etc. |
| `03-matrix plots.ipynb` | Heatmaps and clustermaps |
| `04-grids.ipynb` | FacetGrid, PairGrid, pairplot |
| `05-regression plots.ipynb` | Regression plots with hue and faceting |
| `06-style and color.ipynb` | Themes, palettes, and visual cleanup |
| `07-my seaborn exercises.ipynb` | My solutions to seaborn exercises |
| `08-seaborn exercises - solutions.ipynb` | Instructor reference answers |

---
