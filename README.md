#  Car Price Prediction

A machine learning project that predicts the market price of used cars based on their features such as manufacturer, model, mileage, engine specifications, fuel type, and more.

---

Test Folder has only been used to filter based on brand and model. We have dropped the models and brands the were rare on the dataset.

## 📌 Project Overview

This project builds a regression-based machine learning pipeline to estimate car prices using structured tabular data. It includes:

- Data cleaning and preprocessing
- Feature engineering
- Target encoding for high-cardinality features
- Polynomial feature expansion
- Regularized regression model (Ridge Regression)
- Model evaluation using cross-validation

---

## 📊 Dataset Features

The dataset includes the following features:

### Numerical Features
- Levy
- Prod. year
- Engine volume
- Mileage
- Cylinders
- Airbags
- Car Age

### Categorical Features
- Manufacturer
- Model
- Category
- Fuel type
- Gear box type
- Drive wheels
- Color
- Doors
- Wheel
- Leather interior

---

## ⚙️ Data Processing Steps

### 1. Data Cleaning
- Handled missing values
- Converted text-based numeric columns
- Standardized inconsistent formats

### 2. Feature Engineering
- Created `Car_Age`
- Extracted turbo information from engine volume
- Converted mileage to numeric format

### 3. Encoding
- One-Hot Encoding for low-cardinality categorical features
- K-Fold Target Encoding for high-cardinality features (Manufacturer, Model)

### 4. Scaling & Transformation
- StandardScaler applied to numerical features
- PolynomialFeatures (degree=2) added for interaction terms

---

## 🤖 Model Used

- Ridge Regression (RidgeCV)
- Cross-validation (5-fold)
---

## 📈 Evaluation Metrics

The model is evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Example Results:
- MAE: ~6114
- RMSE: ~8883
- R²: ~0.685

---

## 🔍 Key Insights

- Manufacturer and model significantly influence price
- Feature interactions improve model performance
---

## ⚠️ Limitations

- Some outliers may affect performance
- Linear model may not fully capture complex relationships
- Performance can be improved using advanced models (e.g., XGBoost, CatBoost)

---

## 🚀 Future Improvements

- Try tree-based models (XGBoost / LightGBM / CatBoost)
- Improve feature engineering (accident history)
- Hyperparameter tuning
- Deploy model

---

## 🛠️ Tech Stack

- Python 🐍
- Pandas / NumPy
- Scikit-learn
- Jupyter Notebook
- Machine Learning (Regression)

---
