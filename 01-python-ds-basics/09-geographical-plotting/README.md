# Plotly Choropleth Maps (Section 08)

## 🌍 Overview

In this section, I learned how to build geographic visualizations using **Plotly choropleth maps** via the `chart_studio` and `plotly` modules.  
Unlike earlier visualizations, these plots are mapped directly onto global or national maps, providing powerful ways to represent geographic data.

---

## 🛠️ Core Concepts

The choropleth data was defined using a lower-case `data = dict(...)` pattern, including keys such as:

- `type='choropleth'` – Defines the map type  
- `locations` – Country or state codes  
- `locationmode` – `"USA-states"` or `"country names"`  
- `z` – Numeric values to map by color intensity  
- `text` – Optional hover information

The layout is passed as a separate dictionary and both are wrapped into a `go.Figure(data, layout)` object.

This figure is then passed to `iplot()` to render an interactive choropleth map.

---

## 💬 Reflection

This type of visualization was more complex than previous charts, especially due to the structure of Plotly’s `data` and `layout` dictionaries.  
However, I realized that this also makes the charts much more customizable.  
Being able to create interactive global and USA maps, complete with hover effects and zoom, makes it ideal for dashboards and data storytelling.

---

## 📂 Files

| File | Description |
|------|-------------|
| `01-my choropleth maps.ipynb` | My practical notebook for choropleth map creation |
| `02-choropleth maps exercise.ipynb` | Choropleth map practice assignment |
| `03-choropleth maps exercise-solutions.ipynb` | Instructor solution notebook |
| `01-ref choropleth maps.ipynb` | Provided reference notebook |
| `2011_US_AGRI_Exports` | Data for US agriculture map |
| `2012_Election_Data` | Data for US election map |
| `2014_World_GDP` | Data for global GDP map |
| `2014_World_Power_Consumption` | Data for global energy consumption map |

---
