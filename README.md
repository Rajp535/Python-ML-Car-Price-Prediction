# 🚗 Car Price Prediction Using Autos Dataset (autos_dataset.xlsx)

## 📌 Objective
To predict the price of a car based on its various specifications using regression models. The goal is to help estimate vehicle prices more accurately for resale platforms and dealerships.

## 📊 Dataset
- **Source:** Local file – `autos_dataset.xlsx` (based on UCI Automobile dataset)
- **Features:** 
  - `symboling`, `normalized-losses`, `make`, `fuel-type`, `aspiration`, `num-of-doors`
  - `body-style`, `drive-wheels`, `engine-location`, `wheel-base`, `length`, `width`, `height`
  - `curb-weight`, `engine-type`, `num-of-cylinders`, `engine-size`, `fuel-system`
  - `bore`, `stroke`, `compression-ratio`, `horsepower`, `peak-rpm`, `city-mpg`, `highway-mpg`
- **Target:** 
  - `price`

## 🧠 Techniques Used
- Data Cleaning (handling missing values, correcting datatypes)
- Outlier Treatment (IQR method)
- Label Encoding for categorical variables
- Feature Scaling using MinMaxScaler
- Log Transformation for the skewed target variable (`price`)
- Train-test split (80% train, 20% test)
- Linear Regression Model
- Ridge Regression (L2 Regularization)
- Ensemble Learning with Gradient Boosting Regressor
- Hyperparameter Tuning using RandomizedSearchCV

## 📈 Model Performances
| Model | Train R² Score | Test R² Score |
|:------|:--------------:|:-------------:|
| Linear Regression | 89.57% | 87.16% |
| Ridge Regression | 89.05% | 88.03% |
| Gradient Boosting (Tuned) | 97.13% | 91.05% |

## 🔍 Key Insights
- `engine-size`, `horsepower`, and `curb-weight` had the highest positive impact on car prices.
- Gradient Boosting Regressor outperformed other models after hyperparameter optimization.
- Regularization techniques like Ridge Regression helped improve model generalization.

## 📁 Files
- `Car_Price_Prediction.ipynb` – Full notebook including data preprocessing, EDA, modeling, and evaluation
- `autos_dataset.xlsx` – Cleaned dataset used for model training and testing

## ✅ Outcome
Successfully developed a robust regression model capable of predicting car prices with high accuracy (91% R² score on test data), making it suitable for use cases like price estimation in the used car market.

---

