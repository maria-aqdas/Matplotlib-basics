# 📊 Matplotlib Basics: Data Visualization Guide

A beginner-friendly, hands-on guide to **Data Visualization in Python using Matplotlib**.

This repository contains a practical Jupyter Notebook covering essential visualization techniques, including line plots, bar charts, histograms, pie charts, scatter plots, and subplots. It is designed to help beginners understand how to create, customize, and interpret different types of charts using Python.

## 📋 Table of Contents
              
- 📝 Project Overview
- 📊 Visualizations Covered
- 🛠️ Technologies & Libraries
- ⚙️ Prerequisites
- 🚀 Installation & Setup
- 💻 Practical Code Examples
- 📚 What I Learned
- 🤝 Contributing
- 📄 License

## 📝 Project Overview

Data visualization is an important skill in Data Science because it helps transform raw data into meaningful visual information.

In this notebook, I explored the fundamentals of Matplotlib using `matplotlib.pyplot`. The examples demonstrate how to create different charts, customize their appearance, compare multiple datasets, and display multiple visualizations in a single figure.

### 🎯 Learning Objectives

- Understand the basics of Matplotlib.
- Create different types of charts using Python.
- Customize chart colors, markers, and line styles.
- Add titles, axis labels, legends, and grids.
- Compare multiple datasets using line plots.
- Arrange multiple charts using subplots.

## 📊 Visualizations Covered

The notebook includes the following visualization techniques:

| Visualization | Key Functions | Description |
|---|---|---|
| 📈 Basic Line Plot | `plt.plot()` | Creates a simple line graph to display data trends. |
| 🎨 Customized Line Plot | `plt.figure()`, `color`, `marker`, `linestyle` | Customizes chart appearance, markers, and figure size. |
| 📉 Multi-line Comparison | `plt.plot()`, `plt.legend()` | Compares multiple datasets, such as sales across different years. |
| 📊 Bar Chart | `plt.bar()` | Compares values across different categories. |
| 📦 Histogram | `plt.hist()` | Displays the frequency distribution of numerical data. |
| 🥧 Pie Chart | `plt.pie()` | Represents proportions and percentage distributions. |
| 🔵 Scatter Plot | `plt.scatter()` | Visualizes relationships between two numerical variables. |
| 🧩 Subplots | `plt.subplot()` | Displays multiple charts within a single figure. |

## 🛠️ Technologies & Libraries

- **Programming Language:** Python
- **Data Visualization:** Matplotlib
- **Development Environment:** Jupyter Notebook

## ⚙️ Prerequisites

Before running this notebook, make sure you have:

- Python 3.8 or above
- Jupyter Notebook or JupyterLab
- Basic knowledge of Python

You can also use VS Code with the Jupyter extension.

## 🚀 Installation & Setup

Follow these steps to run the notebook on your local machine.

### 1. Clone the Repository

```bash
git clone https://github.com/maria-aqdas/Matplotlib-basics.git
```

### 2. Navigate to the Project Directory

```bash
cd Matplotlib-basics
```

### 3. Install Required Libraries

```bash
pip install matplotlib jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `Matplotlib.ipynb` and run the notebook cells to explore the examples.

## 💻 Practical Code Examples

### 1. 🎨 Customized Line Chart

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [10, 45, 76, 84, 34]

plt.figure(figsize=(6, 4))

plt.plot(
    x, y,
    color="green",
    marker="o",
    linestyle="dashed",
    linewidth=2,
    markersize=10
)

plt.title("My First Matplotlib Chart")
plt.xlabel("X-Axis")
plt.ylabel("Y-Axis")
plt.grid(True)

plt.show()
```

### 2. 📈 Multi-line Sales Comparison

```python
import matplotlib.pyplot as plt

months = [1, 2, 3, 4, 5]

sales_2024 = [20, 30, 40, 50, 80]
sales_2025 = [40, 60, 90, 85, 70]

plt.plot(months, sales_2024, label="Sales of 2024")
plt.plot(months, sales_2025, label="Sales of 2025")

plt.title("Year-on-Year Sales Comparison")
plt.xlabel("Months")
plt.ylabel("Sales")

plt.legend()
plt.show()
```

### 3. 🧩 Creating Side-by-Side Subplots

```python
import matplotlib.pyplot as plt

category = ["A", "B", "C", "D", "E"]
sales = [76, 56, 48, 98, 76]

a = [3, 6, 7, 8, 4]
b = [34, 54, 32, 36, 76]

plt.figure(figsize=(10, 4))

# Bar Chart
plt.subplot(1, 2, 1)
plt.bar(category, sales, color="skyblue")
plt.title("Bar Chart")
plt.xlabel("Category")
plt.ylabel("Sales")

# Scatter Chart
plt.subplot(1, 2, 2)
plt.scatter(a, b, color="coral")
plt.title("Scatter Chart")
plt.xlabel("A Values")
plt.ylabel("B Values")

plt.tight_layout()
plt.show()
```

## 📚 What I Learned

Through this hands-on practice, I developed a better understanding of:

- 📈 Creating different types of visualizations using Matplotlib.
- 🎨 Customizing charts with colors, markers, and line styles.
- 🏷️ Adding titles, labels, legends, and grid lines.
- 📊 Comparing multiple datasets through visualizations.
- 🔍 Understanding distributions and relationships using histograms and scatter plots.
- 🧩 Organizing multiple visualizations using subplots.

## 🤝 Contributing

Suggestions, improvements, and contributions are always welcome!

Feel free to:

- Open an issue to report a problem.
- Suggest new visualization examples.
- Submit a pull request with improvements.

## 📄 License

This project is licensed under the **MIT License**.

---

### 👩‍💻 Author
                  
**Maria Aqdas**

BS Data Science Student | Aspiring Data Scientist

🔗 [GitHub](https://github.com/maria-aqdas)
