# Matplotlib Basics (Section 04)

## 🔍 Overview

In this section, I learned the fundamentals of data visualization using the **Matplotlib** library.  
Matplotlib allows for highly customizable plots and serves as the foundation for many other visualization libraries in Python.

---

## 📌 Topics Covered

### 🔹 Basic Setup
- Imported the library as `import matplotlib.pyplot as plt`
- Used `plt.figure()` to create a blank canvas
- Added visual space using `.add_axes()` to place subplots

### 🔹 Plotting Data
- Plotted lines with `ax.plot(x, y)` within specific axes
- Customized plot titles, labels, line color, linewidth, linestyle, and markers
- Used `plt.subplots()` to quickly create multiple plots in one figure
- Assigned individual axes to variables for more flexible control

### 🔹 Nested Axes (Inset Plots)
- Created multi-layered plots using:

```python
fig = plt.figure()
ax1 = fig.add_axes([0, 0, 1, 1])       # Main plot
ax2 = fig.add_axes([0.2, 0.5, .4, .4]) # Inset plot
```

- This allows embedding a plot inside another, often for zoomed-in detail or sub-highlighting.

---

## 💬 Reflection

Learning how to manually build a plot structure using `.figure()` and `.add_axes()` helped me understand how Matplotlib renders visual elements layer by layer.  
The `.subplots()` function, while faster for general use, offered less control than explicitly placing axes.  
Using customizable styles for plot appearance (line color, marker size, legends) made me appreciate how versatile this library is for both technical and presentation-ready charts.  
The inset plot technique was especially interesting and showed how professional-level visual storytelling can be achieved.

---

## 📂 Files

| File | Description |
|------|-------------|
| `01-my-matplotlib-concepts-lecture.ipynb` | My practical notebook from lecture concepts |
| `02-my-matplotlib-exercises.ipynb` | Exercise solutions written by me |
| `03-matplotlib-exercises-solutions.ipynb` | Instructor-provided answer notebook |
| `01-ref-matplotlib-concepts-lecture.ipynb` | Instructor reference notebook from lecture |

---
