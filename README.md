# ML-Labs

Here all Machine Learning Labs

# Premier League Data Quality Assessment & Preprocessing

This lab focuses on the fundamental steps of Data Preprocessing and Exploratory Data Analysis (EDA) using a real-world dataset of English Premier League matches. The goal is to clean, normalize, and reduce the dimensionality of the data to make it ready for Machine Learning models.

## Project Overview
In this branch, I applied various data science techniques to assess the quality of football match statistics, handling everything from missing attendance figures to analyzing performance using PCA.

## Features & Tasks

### 1. Data Cleaning & Quality Assessment
* Converted `attendance` figures from string format (with commas) to numeric for analysis.
* Identified data types and ensured consistency across the dataset.

### 2. Handling Missing Values
* Analyzed columns for null values.
* **Strategy:** Applied **Median Imputation** for missing numerical values. 
* *Why Median?* In football statistics, extreme scorelines (e.g., a 9-0 win) can skew the mean. The median provides a more robust central tendency.

### 3. Outlier Detection
* Used the **Interquartile Range (IQR)** method to detect anomalies in match stats like `home_shots`.
* Visualized distributions using **Boxplots** to identify extreme performance cases.


### 4. Feature Scaling (Normalization)
To prepare the data for PCA, I implemented two scaling techniques:
* **Min-Max Scaling:** Squashing data into a [0, 1] range.
* **Z-score Standardization:** Scaling data to have a Mean of 0 and Standard Deviation of 1.

### 5. Dimensionality Reduction (PCA)
* Applied **Principal Component Analysis (PCA)** to reduce 5+ features into 2 Principal Components.
* Visualized the variance to understand how match intensity and team performance are distributed.



## Technologies Used
* **Pandas & NumPy** (Data Manipulation)
* **Matplotlib & Seaborn** (Data Visualization)
* **Scikit-Learn** (Preprocessing & PCA)

## Results
The PCA visualization clearly shows clusters of matches, helping to distinguish between high-intensity games (many shots/high possession) and more defensive encounters.
