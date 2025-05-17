# 🚗 Predicting MPG of Cars

This project analyzes and models automobile data to predict **miles per gallon (MPG)** using machine learning techniques. By exploring feature relationships and building regression models, we aim to understand the key factors influencing fuel efficiency.

## 📊 Dataset Overview

- Source: [`auto-mpg.csv`](https://raw.githubusercontent.com/cheribeda/datamining/main/auto-mpg.csv)
- Features include:
  - `mpg`: Target variable (fuel efficiency)
  - `cylinders`, `displacement`, `horsepower`, `weight`, `acceleration`
  - `model year`, `origin`, and `car name`

## 🛠 Data Preparation

- Dropped non-numeric `car name` column
- Converted `horsepower` to numeric and filled missing values with the column mean
- Created dummy variables for the `origin` column

## 🔍 Exploratory Analysis

- **Correlation Heatmap** revealed strong negative correlations between MPG and:
  - `weight` (-0.83), `displacement` (-0.80), `horsepower` (-0.77), `cylinders` (-0.78)
- **Positive Correlations** with:
  - `model year` (+0.58), `acceleration` (+0.42)
- **Scatter Plot** showed clear negative trend between vehicle weight and MPG

## 📈 Modeling

### 1. **Linear Regression**
- `R² (train/test)`: 0.819 / 0.845
- `RMSE (train/test)`: 3.37 / 2.89
- `MAE (train/test)`: 2.61 / 2.29

### 2. **Random Forest Regressor**
- `R² (train/test)`: 0.981 / 0.915
- `RMSE (train/test)`: 1.10 / 2.14
- `MAE (train/test)`: 0.75 / 1.60

## ✅ Key Takeaways

- Vehicle **weight** and **engine displacement** are strong predictors of MPG.
- Random Forest Regression significantly outperformed Linear Regression in both accuracy and error metrics.
- Newer car models (by year) tend to be more fuel-efficient.



