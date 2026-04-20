# 🏠 House Price Prediction (Advanced Regression + XGBoost)

## 📌 Project Overview

This project focuses on predicting house prices using machine learning techniques on structured housing data.
It explores multiple regression models, applies feature engineering, and performs model optimization to achieve high predictive accuracy.

---

## 🎯 Objective

* Predict house sale prices based on property features
* Identify key factors influencing house valuation
* Improve model performance using tuning and feature engineering

---

## ⚙️ Workflow

### 🔹 1. Data Analysis

* Explored dataset structure (1460 houses, ~80 features)
* Identified missing values and feature distributions
* Analyzed correlations with target variable (`SalePrice`)

---

### 🔹 2. Data Preprocessing

* Handled missing values using appropriate strategies
* Selected relevant features
* Converted categorical variables for modeling

---

### 🔹 3. Feature Engineering

Created new features to improve model understanding:

* `TotalSF` → total living area
* `LuxuryScore` → OverallQual × GrLivArea

These features helped capture patterns in high-value houses.

---

### 🔹 4. Models Implemented

* Linear Regression
* Random Forest Regressor
* XGBoost Regressor

---

### 🔹 5. Model Optimization

* Hyperparameter tuning (depth, estimators, learning rate)
* Regularization (`reg_alpha`, `reg_lambda`)
* Subsampling to prevent overfitting

---

## 📊 Results

| Model                 | R² Score       | MAE      |
| --------------------- | -------------- | -------- |
| Linear Regression     | ~0.38          | Poor     |
| Random Forest         | ~0.88          | ~17k     |
| XGBoost (Final Model) | **~0.91–0.92** | **~15k** |

---

## 🔍 Key Insights

* `OverallQual` and `GrLivArea` are the most influential features
* Tree-based models outperform linear models due to non-linear relationships
* Feature interactions significantly improve performance
* The model performs best in mid-range price segments

---

## ⚠️ Limitations

* Only **4 houses above 600k** exist in the dataset
* This leads to:

  * underprediction of extreme values
  * regression toward the mean

👉 This highlights a key ML concept:

> Model performance is limited by data distribution

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* XGBoost
* Matplotlib, Seaborn

---

## 🚀 How to Run

```bash
git clone https://github.com/ShaunakG18/house-price-prediction.git
cd house-price-prediction
pip install -r requirements.txt
jupyter notebook
```

---

## 📈 Future Improvements

* Collect more high-value housing data
* Use ensemble/stacking methods
* Deploy model using FastAPI
* Build a frontend dashboard

---

## 👨‍💻 Author

Shaunak G
BTech CSE Student

---

## ⭐ Key Learning

This project demonstrates that:

* Model tuning improves performance
* Feature engineering is critical
* **Data imbalance strongly affects predictions**

---

## 📎 Dataset

Ames Housing Dataset (Kaggle - Advanced Regression Techniques)
