# 🏠 Housing Price Prediction

This repository contains a Jupyter Notebook that implements a machine learning pipeline to predict housing prices in Delhi using different regression models. The project walks through the complete workflow of data preprocessing, model training, evaluation, and deployment of a prediction function.

---

## 📁 Files

- `Housing Price Prediction.ipynb`: Main Jupyter notebook containing the data cleaning, visualization, model building (Linear Regression and Decision Tree), and price prediction logic.


## 🧠 Project Summary

### 🎯 Objective
To predict housing prices based on multiple features like:
- Area
- Number of Bedrooms (BHK)
- Amenities (e.g., Gymnasium)
- Location

---

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn (optional for EDA)

---

## 📊 Data Preprocessing

- Null values and outliers are handled.
- Dummy variable is created for location.
- Feature matrix `X` and target variable `y` are defined.

---

## 🔍 Models Implemented - Decision Tree Regressor had a higher R^2 than Linear Regression

### ✅ Linear Regression
- Fitted using `LinearRegression()` from Scikit-learn.
- Log transformation of Price (Y variable) since the variable was not normally distributed (Rightly Skewed).
- Implemented K-fold cross validation to check the validity of Linear Regression results.

### 🌲 Decision Tree Regressor
- Implemented using `DecisionTreeRegressor()`.
- A separate `predict_price()` function (same interface) was used with this model.
- Offers better capture of non-linear relationships.
- Visualized top 10 locations using the decision tree.

