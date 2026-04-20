# 🏠 House Price Prediction using Machine Learning

## 📌 Overview

This project aims to predict house prices using machine learning techniques. The goal was to analyze housing data, identify key features influencing prices, and build a robust predictive model.

---

## ⚙️ Approach

### 🔹 Data Processing

* Loaded dataset using Pandas
* Handled missing values
* Converted categorical data where required

### 🔹 Feature Engineering

* Created new features to improve model performance:

  * `TotalSF` = Total square footage of house
  * `LuxuryScore` = Overall quality × living area

### 🔹 Models Used

* Linear Regression
* Random Forest Regressor
* XGBoost Regressor

### 🔹 Model Optimization

* Hyperparameter tuning (depth, estimators, learning rate)
* Regularization to reduce overfitting
* Subsampling for better generalization

---

## 📊 Results

| Model             | R² Score       | MAE      |
| ----------------- | -------------- | -------- |
| Linear Regression | ~0.38          | High     |
| Random Forest     | ~0.88          | ~17k     |
| XGBoost           | **~0.91–0.92** | **~15k** |

---

## 🔍 Key Insights

* `OverallQual` and `GrLivArea` are the most influential features
* Tree-based models significantly outperform linear models
* Feature interactions improve prediction accuracy
* The model underpredicts extremely high-priced houses (>600k)

---

## ⚠️ Limitations

The dataset contains very few high-value houses (>600k), which limits the model’s ability to learn patterns in this range.
As a result, predictions for extreme values tend to regress toward the mean.

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* XGBoost
* Matplotlib, Seaborn

---

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/ShaunakG18/house-price-prediction.git
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the notebook:

```bash
jupyter notebook
```

---

## 📈 Future Improvements

* Collect more high-value house data
* Try advanced ensemble techniques
* Deploy model using FastAPI
* Build interactive frontend dashboard

---

## 👤 Author

Shaunak G
Computer Science & Engineering Student

---

## ⭐ Acknowledgment

Dataset inspired by the Ames Housing dataset (commonly used in Kaggle competitions).
