# 📈 Demand Forecasting using Machine Learning

## 📌 Project Overview

This project predicts product demand using Machine Learning by analyzing historical sales, inventory, pricing, promotions, seasonality, weather conditions, and other business-related factors.

A complete end-to-end Machine Learning workflow was implemented, including data preprocessing, exploratory data analysis, feature engineering, model comparison, hyperparameter tuning, and model evaluation.

---

## 🎯 Objectives

* Predict future product demand accurately.
* Analyze the factors that influence demand.
* Compare multiple regression algorithms.
* Select and optimize the best-performing model.
* Build a production-ready machine learning pipeline.

---

## 📂 Dataset Information

The dataset contains **76,000 records** with historical demand data collected across multiple stores and products.

### Features

* Date
* Store ID
* Product ID
* Category
* Region
* Inventory Level
* Units Sold
* Units Ordered
* Price
* Discount
* Weather Condition
* Promotion
* Competitor Pricing
* Seasonality
* Epidemic

### Target Variable

* **Demand**

---

# 🧹 Data Preprocessing

The following preprocessing steps were performed:

* Removed unnecessary features after analysis
* Converted Date into datetime format
* Created new time-based features:

  * Year
  * Month
  * Day
  * DayOfWeek
  * WeekOfYear
  * Quarter
  * IsWeekend
* One-Hot Encoding for categorical variables
* Converted Boolean values into numerical format
* Time-based Train-Test Split (80% Training / 20% Testing)

---

# 📊 Exploratory Data Analysis (EDA)

Performed detailed analysis including:

* Daily Demand Trend
* Category-wise Demand
* Regional Analysis
* Weather Analysis
* Seasonal Analysis
* Promotion Impact
* Correlation Analysis
* Feature Importance Analysis

---

# 🤖 Machine Learning Models

The following regression algorithms were trained and evaluated:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* Gradient Boosting Regressor
* K-Nearest Neighbors Regressor
* Support Vector Regressor (SVR)
* XGBoost Regressor

---

# 🏆 Model Performance

| Model                     | Performance       |
| ------------------------- | ----------------- |
| XGBoost Regressor (Tuned) | ⭐ Best Model      |
| Random Forest Regressor   | Excellent         |
| Decision Tree Regressor   | Good              |
| Gradient Boosting         | Moderate          |
| Linear Regression         | Baseline          |
| KNN                       | Lower Performance |
| SVR                       | Lower Performance |

---

# 📈 Final Model Performance (Tuned XGBoost)

| Metric   | Score      |
| -------- | ---------- |
| R² Score | **91.98%** |
| MAE      | **9.40**   |
| RMSE     | **12.48**  |

---

# 🔧 Hyperparameter Tuning

The best-performing model (XGBoost) was further optimized using hyperparameter tuning, improving:

* R² Score from **85% → 91.98%**
* Lower MAE
* Lower RMSE
* Better overall generalization

---

# 📌 Feature Importance

The most influential features identified by the model were:

1. Price
2. Discount
3. Epidemic
4. Inventory Level
5. Store ID
6. Category
7. Week of Year
8. Region
9. Weather Condition

---

# 📁 Project Structure

```
Demand-Forecasting/
│
├── data/
│   ├── Raw_Dataset.csv
│   └── Cleaned_Dataset.csv
│
├── models/
│   ├── xgboost_demand_forecasting.pkl
│   └── feature_names.pkl
│
├── notebook.ipynb
├── README.md
```

---

# 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* XGBoost
* Joblib

---

# 🚀 Future Improvements

* Deploy using Streamlit
* Real-time demand prediction
* Interactive dashboard
* REST API integration
* Automated model retraining

---

# 👨‍💻 Author

**Zeeshan Shaukat**

Aspiring Machine Learning Engineer

GitHub: https://github.com/zeeshan2007

---

## ⭐ If you found this project useful, consider giving it a star on GitHub.
