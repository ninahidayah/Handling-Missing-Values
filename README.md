# 🧹 Handling Missing Values in Movie Dataset

This project demonstrates how to handle missing values in a dataset using Python. The dataset includes movie-related information such as **budget**, **gross**, and **rating**, which contain missing data. The goal is to clean the data using appropriate imputation techniques based on the type, distribution, and proportion of missing values.

---

## 📂 Dataset
The dataset used in this project was imported from Kaggle (`danielgrijalvas/movies`).  
It contains several numerical and categorical features related to movies.

---

## ⚙️ Libraries
- Python  
- Pandas   
- Matplotlib 
- Seaborn

---

## 📊 Missing Value Handling Strategy

| Column  | Type        | Missing % | Distribution   | Imputation Method       | Reasoning                                                                 |
|---------|-------------|------------|----------------|--------------------------|---------------------------------------------------------------------------|
| budget  | Numerical   | 5–30%      | Right-skewed    | Grouped Median (by genre) | Median is robust to outliers; grouped by genre because it affects budget |
| gross   | Numerical   | <5%        | Right-skewed    | Median                   | Low missing %, right-skewed → median is suitable                          |
| rating  | Categorical | <5%        | N/A             | Mode                     | Categorical data → most common value (mode)                               |


