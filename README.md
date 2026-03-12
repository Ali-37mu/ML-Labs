# ML-Labs

Here all Machine Learning Labs

---

# ARTI 308 – Lab 5: Feature Engineering (Classification)

## Order Status Prediction using a Talabat-style Dataset

### Project Overview

This project focuses on the critical stage of **Feature Engineering** within the machine learning pipeline. Using a dataset modeled after food delivery services (like Talabat), the goal is to build a classification model that predicts the `Order_Status` of a given transaction.

### Objectives

The primary objective is not just model accuracy, but understanding how different feature engineering choices—such as time-based features, price-based metrics, and category reduction—impact the performance and interpretability of the model.

Key goals include:

* Identifying and avoiding **Data Leakage**.
* Creating new predictors from raw timestamps and coordinates.
* Handling high-cardinality categorical data.
* Evaluating a **Random Forest Classifier** and interpreting feature importance.

### Key Technical Steps

1. **Data Inspection:** Loading the "clean" dataset and identifying target/predictor variables.
2. **Feature Engineering:**
* **Time-based:** Extracting hour, day of the week, and "is_peak_hour".
* **Price-based:** Calculating average item price and total costs.
* **Distance-based:** Estimating delivery distance using coordinates.


3. **Encoding:** Implementing `OneHotEncoder` and managing category reduction for items.
4. **Modeling:** Training a Random Forest model.
5. **Evaluation:** Using Confusion Matrices and Classification Reports to measure success.

### Lab Tasks Included

The notebook contains several hands-on tasks:

* **Task 1:** Creating a custom engineered feature with a written justification.
* **Task 2:** Experimenting with different rules for "Peak Hour" classification.
* **Task 3:** Tuning `top_k` for item name reduction to observe changes in accuracy.
* **Task 4:** Performing optional feature selection to optimize the model.

### Requirements

* Python 3.x
* Pandas & NumPy
* Scikit-Learn
* Matplotlib & Seaborn

### Conclusion

By the end of this lab, it is demonstrated that while the raw data was clean, the "intelligence" of the model is largely derived from how we transform that data into meaningful features that capture human behavior and logistical patterns.
