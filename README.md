# ML-Labs

Here all Machine Learning Labs

# Logistic Regression - Ad Click Prediction

## About

This project is part of the Machine Learning course. The goal is to build a logistic regression model that predicts whether a user will click on an advertisement based on their behavior and demographic data.

The dataset used is a fake advertising dataset with 1000 entries.

---

## Dataset

The file `advertising.csv` contains the following columns:


'Daily Time Spent on Site': consumer time on site in minutes
'Age': cutomer age in years
'Area Income': Avg. Income of geographical area of consumer
'Daily Internet Usage': Avg. minutes a day consumer is on the internet
'Ad Topic Line': Headline of the advertisement
'City': City of consumer
'Male': Whether or not consumer was male
'Country': Country of consumer
'Timestamp': Time at which consumer clicked on Ad or closed window
'Clicked on Ad': 0 or 1 indicated clicking on Ad

---

## What I Did

1. Loaded and explored the data using pandas
2. Made some visualizations with seaborn (histograms, jointplots, pairplot)
3. Split the data into training and testing sets (70/30 split)
4. Trained a Logistic Regression model using scikit-learn
5. Evaluated the model using a classification report

---

## Results

The model got about **93% accuracy** on the test set which I think is pretty good for a simple logistic regression.
