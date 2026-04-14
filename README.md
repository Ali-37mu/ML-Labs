# ML-Labs

Here all Machine Learning Labs

# ARTI308 - Lab 6: Linear Regression
 
This is my submission for Lab 6 in ARTI308. The task was to apply Linear Regression on a new dataset (Ecommerce Customers) using the same steps we did in the lab with the USA Housing dataset.
 
---
 
## Dataset
 
The dataset is called **Ecommerce Customers** and it contains info about customers of an online store. It has 500 rows and 8 columns.
 
The goal is to predict **Yearly Amount Spent** based on customer behavior features.
 
Features used:
- Avg. Session Length
- Time on App
- Time on Website
- Length of Membership
 
Columns like Email, Address, and Avatar were dropped since they're not useful for the model.
 
---
 
## What I Did
 
1. Loaded the dataset into a pandas DataFrame
2. Explored the data using head(), info(), and describe()
3. Checked for null values (there were none)
4. Dropped non-numeric columns
5. Looked at correlations to understand which features matter
6. Split the data into training and testing sets (70/30)
7. Trained a Linear Regression model
8. Evaluated using MAE, MSE, RMSE, and R²
 
---
 
## Results

The model performed really well with an R² of about 0.98 which means it explains 98% of the variance in the target variable.
 
The most important feature was **Length of Membership** followed by **Time on App**. Interestingly, Time on Website had almost no effect on how much customers spend.
 
---
 
## Files
 
- `ARTI308_Lab6_EcommerceCustomers.ipynb` - the main notebook
- `Ecommerce_Customers` - the dataset used
- `USA_Housing.csv` - original lab dataset (for reference)
 
---
 
## How to Run
 
1. Clone the repo
2. Make sure you have pandas, numpy, scikit-learn, matplotlib, and seaborn installed
3. Open the notebook and run all cells
 
 
---
 
## Notes
 
This was done as part of the ARTI308 course. The model and general approach follow what was covered in the lab, just applied to a different dataset.
