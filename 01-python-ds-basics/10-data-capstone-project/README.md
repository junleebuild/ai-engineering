# 📊 Data Capstone Projects – 911 Calls & Finance Data

## 📁 Project Overview

This folder contains two capstone projects focused on real-world data analysis using Pandas, Seaborn, and Matplotlib.

---

## 🚨 911 Calls Capstone Project

### ✅ Description:
Analyzed emergency 911 call data from a CSV file containing features like:
- Latitude & Longitude
- Timestamps
- Title (reason for the call)

### 📌 Techniques & Insights:
- Extracted features like `Hour`, `Month`, `Day of Week` from timestamps using:
  ```python
  df['Hour'] = df['timeStamp'].apply(lambda time: time.hour)
  df['Month'] = df['timeStamp'].apply(lambda time: time.month)
  df['Day of Week'] = df['timeStamp'].apply(lambda time: time.dayofweek)
  ```
- Used `.groupby()` and `.count()` for monthly and daily aggregation.
- Visualized call frequencies by reason with `sns.countplot(hue=...)`.
- Applied `sns.lmplot()` and line plots to observe trends.

### 💬 Reflection:
This project helped develop flexibility in time-based feature extraction and visualization.  
Although the logic wasn't difficult, mastering hue-based slicing and timestamp parsing was great practice.

---

## 💼 Finance Capstone Project

### ✅ Description:
Worked with financial stock data (FAANG companies) to perform advanced data analysis and correlation studies.

### 📌 Techniques & Insights:
- Used pre-downloaded stock data due to discontinued API access.
- Leveraged `.xs()` for multi-index selection across tickers and dates.
- Visualized using:
  - `seaborn.heatmap()` for correlation visualization
  - `seaborn.clustermap()` for similarity clustering

### 💬 Reflection:
This part was notably more challenging.  
It introduced a higher number of parameters and complex data structures.  
Understanding how multi-indexing interacts with advanced visualization tools like `clustermap` is something I need to revisit and reinforce.

---

📁 Files included:
- `01-my 911 calls data capstone project.ipynb`
- `02-911 Calls Data Capstone Project - Solutions.ipynb`
- `03-my finance project.ipynb`
- `04-Finance Project - Solutions.ipynb`

📦 Datasets:
- `911.csv`
- `precipitation.html`
- `*.csv` files for finance data
