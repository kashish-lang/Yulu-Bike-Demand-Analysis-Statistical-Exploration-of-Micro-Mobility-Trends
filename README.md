# Yulu-Bike-Demand-Analysis-Statistical-Exploration-of-Micro-Mobility-Trends
This project analyzes the factors influencing the demand for Yulu’s shared electric bikes in India. Using statistical techniques like t-tests, ANOVA, and Chi-square tests, the study explores how variables such as season, weather, working days, and temperature affect bike rentals.
# 🚲 Yulu Bike Demand Analysis

Yulu is India’s leading micro-mobility service provider, offering shared electric bikes for daily commutes. This project analyzes the **factors affecting the demand** for Yulu's shared electric cycles using **statistical tests** and **exploratory data analysis (EDA)**.

---

## 📌 Problem Statement

Yulu has observed a drop in revenue and wants to understand the key variables that influence demand. The goal is to:

- Identify which factors significantly impact bike rental demand.
- Quantify how well those variables explain the variation in demand.

---

## 🧪 Techniques Used

- **Exploratory Data Analysis (EDA)**  
- **2-Sample T-Test**  
- **ANOVA (Analysis of Variance)**  
- **Chi-Square Test**  
- **Hypothesis Testing Framework**  
- **Visual Analysis and Assumption Checks**

---

## 🗃️ Dataset

The dataset `yulu_data.csv` includes the following variables:

| Column       | Description |
|--------------|-------------|
| `datetime`   | Timestamp of rental |
| `season`     | Season (1: Spring, 2: Summer, 3: Fall, 4: Winter) |
| `holiday`    | Whether the day is a holiday (0/1) |
| `workingday` | Whether it is a working day (0/1) |
| `weather`    | Weather condition (1 to 4 scale) |
| `temp`       | Temperature in Celsius |
| `atemp`      | Feels-like temperature in Celsius |
| `humidity`   | Humidity percentage |
| `windspeed`  | Wind speed |
| `casual`     | Count of casual users |
| `registered` | Count of registered users |
| `count`      | Total rental bikes (casual + registered) |

---

## 🔍 Analysis Overview

### 1. 📊 Exploratory Data Analysis (EDA)
- Univariate and bivariate visualizations
- Detection of outliers and missing values
- Summary statistics and data type conversions

### 2. 🧠 Hypothesis Testing

| Hypothesis | Test Used | Purpose |
|------------|-----------|---------|
| Does working day affect demand? | 2-Sample T-Test | Compare mean rentals on working vs non-working days |
| Is rental count different across seasons? | One-way ANOVA | Compare mean rentals across seasons |
| Is rental count different across weather conditions? | One-way ANOVA | Compare mean rentals across weather types |
| Are weather and season dependent? | Chi-Square Test | Test association between two categorical variables |

- Assumptions checked using:
  - Histograms
  - Q-Q Plots
  - Levene’s Test (for equal variances)
  - Shapiro-Wilk Test (for normality)

---

## 📈 Key Insights

- Demand is significantly higher on working days.
- Seasonal and weather changes have a notable effect on rentals.
- There is a dependency between season and weather conditions.

---

## 🛠 Tools & Libraries

- **Python**
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scipy.stats`, `statsmodels`

---

## ✅ Conclusion

This analysis provides data-driven insights into user behavior and helps Yulu optimize operations and zone placements based on demand patterns.

---

## 📂 Repository Structure

