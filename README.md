# ML-Labs

Here all Machine Learning Labs

# Credit Card Customer Segmentation - K-Means Clustering

Machine learning assignment focused on customer segmentation using K-Means clustering.  
The goal of this project is to group credit card customers based on their financial behavior and spending patterns.

---

# Dataset

The project uses the `CC_GENERAL.csv` dataset, which contains customer information such as:

- Balance
- Purchases
- Cash advances
- Credit limit
- Payments
- Purchase frequency
- Tenure

---

# What I Did

- Cleaned the dataset and handled missing values
- Removed the `CUST_ID` column
- Performed Exploratory Data Analysis (EDA)
- Applied feature scaling using `StandardScaler`
- Used the Elbow Method and Silhouette Score to choose the best number of clusters
- Trained a K-Means model with `K = 4`
- Analyzed customer segments using cluster averages
- Used PCA to visualize clusters in 2D

---

# Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---

# Notes

This project demonstrates how unsupervised learning can identify hidden patterns in customer behavior without labeled data. The results help separate customers into meaningful groups based on spending and financial activity.
