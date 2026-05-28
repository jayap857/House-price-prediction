# House Price Prediction System

## Project Overview

This project is a Machine Learning-based House Price Prediction System that predicts house prices using various regression models.

The project includes:
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Model Training
- Model Evaluation
- Cross Validation
- Feature Importance Analysis

The goal of this project is to build an accurate predictive model for house prices using machine learning techniques.

---

## Dataset Information

The dataset contains house-related features such as:
- Number of bedrooms
- Number of bathrooms
- Square footage
- Floors
- House condition
- Year built
- Location-related information

Target Variable:
- `price`

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Joblib

---

## Machine Learning Models Used

The following regression models were implemented:

1. Linear Regression
2. Random Forest Regressor
3. Gradient Boosting Regressor
4. XGBoost Regressor

---

## Project Workflow

### 1. Data Preprocessing
- Handled missing values
- Removed duplicates
- Removed outliers using IQR method

### 2. Exploratory Data Analysis (EDA)
- Distribution plots
- Correlation analysis
- Heatmaps
- Feature relationships

### 3. Feature Engineering
Created new features such as:
- `house_age`
- `total_rooms`
- `total_sqft`

### 4. Model Training
Split data into:
- Training Set
- Testing Set

Trained multiple machine learning models.

### 5. Model Evaluation
Used evaluation metrics:
- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

### 6. Cross Validation
Performed cross-validation to check model stability and performance.

---

## Results

Among all models, the best performance was achieved using:

- Random Forest Regressor / XGBoost Regressor

Key Findings:
- Square footage strongly influences house price
- Feature engineering improved model performance
- Ensemble models performed better than linear models

---

## Feature Importance

Feature importance analysis was performed to identify the most influential variables affecting house prices.

---

## Model Saving

The trained model was saved using Joblib for future predictions.

```python
joblib.dump(model, 'house_price_model.pkl')
