# 🛒 Predicting Customer Purchase Value

## 📌 Project Overview

This project was developed as part of the **Engage 2: Value from Clicks to Conversions** competition on Kaggle.
The goal is to **predict a customer’s purchase value** based on their **multi-session digital behavior** across web and app touchpoints.

The dataset contains anonymized user interactions such as:

* Browser and device information
* Traffic sources (organic, referral, direct, ads)
* Geographical details
* Multi-session activity patterns

By modeling these signals, we estimate each user’s **purchase potential**, helping optimize **marketing campaigns** and **customer engagement strategies**.

---

## ⚙️ Approach

1. **Exploratory Data Analysis (EDA):**

   * Studied distribution of purchase values and user behaviors
   * Analyzed categorical features like traffic source, browser, device type
   * Detected missing values and anomalies

2. **Feature Engineering:**

   * Encoded categorical features (One-Hot / Label Encoding)
   * Created aggregated session-level features (counts, means, ratios)
   * Derived interaction features to capture user behavior patterns

3. **Modeling:**

   * Trained multiple regression models:

     * **Linear Regression** (baseline)
     * **Random Forest Regressor**
     * **XGBoost Regressor**
     * **LightGBM Regressor**
   * Performed hyperparameter tuning using cross-validation
   * Compared results using **R² score** and **RMSE**

4. **Evaluation Metric:**

   * The main evaluation metric is **R² score** (higher is better)
   * Aim: Achieve **R² > 0.75** for strong predictive performance

---

## 📊 Results

* Baseline Linear Regression: \~0.30 R²
* Random Forest: Improved stability and feature importance insights
* XGBoost & LightGBM: Achieved the best scores (\~0.68 R² on Kaggle public leaderboard)

---

## 🛠️ Tech Stack

* **Language:** Python
* **Libraries:**

  * Data Processing → `pandas`, `numpy`
  * Modeling → `scikit-learn`, `xgboost`, `lightgbm`
  * Visualization → `matplotlib`


