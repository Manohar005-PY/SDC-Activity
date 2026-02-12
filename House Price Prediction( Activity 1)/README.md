🏠 House Price Prediction Using Regression

## 📌 Project Overview

This project aims to predict residential house sale prices using machine learning regression techniques. 
The objective is to estimate the sale price of a house based on selected structural and property-related features.

The project demonstrates a complete machine learning workflow including dataset exploration, preprocessing, model training, and performance evaluation.

## 🎯 Problem Definition

Accurate house price prediction is important for buyers, sellers, and real estate professionals to make informed financial decisions.

This problem is formulated as:

* **Type:** Supervised Learning
* **Task:** Regression
* **Input:** Selected numerical house features
* **Output:** SalePrice (continuous value)

---

## 📊 Dataset Information

* **Source:** Kaggle – House Prices: Advanced Regression Techniques
* **Total Records:** 1460
* **Total Features:** 80+
* **Target Variable:** SalePrice

### Features Used in This Project

* OverallQual
* GrLivArea
* GarageCars
* TotalBsmtSF
* FullBath
* YearBuilt
* LotArea

Only selected numerical features were used to simplify preprocessing and maintain clarity.

---

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

* Selected relevant numerical features
* Handled missing values using median imputation
* Split dataset into 80% training and 20% testing sets
* Used `random_state=42` to ensure reproducibility

---

## 🧠 Models Implemented

Two regression models were implemented:

1. **Linear Regression** – Baseline model
2. **Random Forest Regressor** – Non-linear ensemble model

Linear Regression provides a simple baseline, while Random Forest captures complex non-linear relationships between features and house prices.

---

## 📈 Evaluation Metrics

Since this is a regression task, classification metrics such as accuracy and confusion matrix are not applicable.

The models were evaluated using:

* **Mean Absolute Error (MAE)**
* **Root Mean Squared Error (RMSE)**
* **R² Score**

---

## 📊 Results

| Model             | MAE    | RMSE   | R² Score |
| ----------------- | ------ | ------ | -------- |
| Linear Regression | 24,788 | 39,583 | 0.796    |
| Random Forest     | 18,525 | 28,659 | 0.893    |

### Interpretation

Random Forest outperformed Linear Regression across all evaluation metrics. 
The higher R² score (0.89) indicates that the model explains approximately 
89% of the variance in house prices, suggesting that non-linear relationships exist 
between property features and sale price.

---

## ▶️ How to Run the Project

1. Clone the repository:

```
git clone <your-repository-link>
```

2. Install required libraries:

```
pip install -r requirements.txt
```

3. Open Jupyter Notebook:

```
jupyter notebook
```

4. Run all cells sequentially.

---

## 📌 Conclusion

This project demonstrates how regression models can be applied to real-world price
prediction problems. Among the implemented models, Random Forest achieved superior 
performance, making it more suitable for this dataset.
