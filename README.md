# Football-Player-Analysis
# ⚽ Football Players Dataset Analysis

## 📌 Project Overview

This project analyzes a football players dataset created by merging two separate datasets, each containing approximately 4,000 player records. After merging, the final dataset consists of approximately 8,000 records and 11 attributes related to football players.

The project demonstrates the use of Python for data cleaning, exploratory data analysis (EDA), and data visualization to uncover insights about player characteristics such as age, height, weight, wages, preferred foot, and playing positions.

---

##  Dataset Information

### Source Files

* `players1.csv`
* `players2.csv`

### Final Merged Dataset

* `players data md.csv`

### Dataset Size

* Approximately 8,000 records
* 11 columns

---

## 🛠 Technologies & Libraries Used

* Python
* Pandas
* Matplotlib
* Seaborn

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

---

##  Data Preparation

### Data Merging

The two datasets were merged using an inner join based on the `short_name` column.

```python
merge = pd.merge(data1, data2, how='inner', on='short_name')
```

### Data Cleaning

The following cleaning steps were performed:

* Removed missing values using `dropna()`
* Removed duplicate records using `drop_duplicates()`

```python
cl.dropna(inplace=True)
cl.drop_duplicates(inplace=True)
```

---

##  Exploratory Data Analysis (EDA)

The following exploratory analysis methods were applied:

* Dataset inspection (`head()`, `tail()`, `sample()`)
* Missing value analysis
* Statistical summary using `describe()`
* Data type inspection using `info()`

---

#  Analysis Questions & Visualizations

## 1. Correlation Between Weight, Height, and Age

A correlation heatmap was created to examine relationships between:

* Weight (kg)
* Height (cm)
* Age

### Visualization

* Heatmap

### Objective

Identify whether age, weight, and height are positively or negatively correlated.

---

## 2. What Is the Average Age of Football Players?

A box plot was used to visualize the distribution of player ages.

### Visualization

* Box Plot

### Objective

* Examine age distribution
* Identify median age
* Detect outliers

---

## 3. How Does Age Affect Player Wage?

A scatter plot was generated to explore the relationship between player age and wage.

### Visualization

* Scatter Plot

### Objective

Determine whether player earnings tend to increase or decrease with age.

---

## 4. Players Height Distribution

A histogram was created to analyze player height distribution.

### Visualization

* Histogram

### Objective

Identify the most common height ranges among football players.

---

## 5. Preferred Foot Analysis

A pie chart was used to show the proportion of left-footed and right-footed players.

### Visualization

* Pie Chart

### Objective

Compare the distribution of preferred foot usage among players.

---

## 6. Most Preferred Playing Positions

A count plot was created to display the frequency of each playing position.

### Visualization

* Count Plot

### Objective

Determine the most common positions occupied by football players.

---

## 📷 Visualizations Included

* Correlation Heatmap
* Age Distribution Box Plot
* Age vs Wage Scatter Plot
* Height Distribution Histogram
* Preferred Foot Pie Chart
* Position Count Plot

---

## 🎯 Key Learning Outcomes

Through this project, the following data analysis skills were practiced:

* Data merging and integration
* Data cleaning and preprocessing
* Exploratory data analysis (EDA)
* Statistical correlation analysis
* Data visualization with Matplotlib and Seaborn
* Insight generation from sports datasets

---

##  Future Improvements

Possible enhancements for future versions:

* Analyze player nationality distributions
* Investigate wage differences by position
* Explore player performance metrics
* Build predictive models for player wages
* Create interactive dashboards using Plotly or Tableau

---

##  Author

Football Players Dataset Analysis Project

Created using Python, Pandas, Matplotlib, and Seaborn for exploratory data analysis and visualization.
