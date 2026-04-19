# ML-Labs

Here all Machine Learning Labs

# K Nearest Neighbors - Classification Project

This is one of my machine learning assignments where I applied the K Nearest Neighbors algorithm to classify data into two target classes.

## About the Project

The dataset (`KNN_Project_Data`) contains 1000 rows and 10 anonymized features (WTT, PTI, EQW, etc.) along with a TARGET CLASS column (0 or 1). The goal is to build a KNN model that can correctly predict which class a data point belongs to.

## What I Did

- Explored the data using a pairplot to visualize how the features separate the two classes
- Standardized the features using `StandardScaler` since KNN is distance-based and sensitive to scale
- Split the data 70/30 into training and testing sets
- Trained an initial KNN model with K=1 and evaluated it
- Used the **Elbow Method** to find the optimal K value by plotting error rate vs. K
- Retrained the model with the best K and compared results

## Results

| K Value | Accuracy |
|---------|----------|
| K = 1   | 83%      |
| K = 5   | 89%      |

Using K=5 gave noticeably better results than K=1. K=1 tends to overfit because it just memorizes the nearest training point.

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
