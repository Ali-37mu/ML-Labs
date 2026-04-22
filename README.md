# ML-Labs

Here all Machine Learning Labs
---
Random Forest Project

A machine learning project from my ML course. The goal is to predict whether a borrower will fully pay back their loan using Decision Trees and Random Forests.

---

## About the Dataset

The data covers loans issued between 2007 and 2010. Each row is one borrower, and the target column is `not.fully.paid` (1 = defaulted, 0 = paid back).

Features include things like FICO score, interest rate, debt-to-income ratio, loan purpose, and a few others. The dataset was already cleaned (no missing values).

---

## What I Did

1. **Explored the data** – plotted FICO distributions, loan counts by purpose, and the relationship between FICO score and interest rate using histograms, countplots, and seaborn jointplots.

2. **Prepared the data** – the `purpose` column was categorical so I converted it to dummy variables using `pd.get_dummies()`.

3. **Trained two models:**
   - Decision Tree (`DecisionTreeClassifier`)
   - Random Forest (`RandomForestClassifier` with 200 trees)

4. **Evaluated both** using classification reports and confusion matrices.

---

## Results

**Model Accuracy**:

Decision Tree: ~73%

Random Forest: ~85%

**Defaulter Recall**:

Decision Tree: Catches more defaulters (recall=0.23) but many false positives

Random Forest: Higher overall accuracy, but almost ignores class 1 (recall≈0.02)

The Random Forest had higher overall accuracy, but it basically ignored the defaulters almost entirely, the dataset is heavily imbalanced (about 84% of borrowers paid back), so the model just learned to predict "fully paid" for almost everyone and still got 85% accuracy

The Decision Tree was lower in accuracy but actually caught more real defaults, which honestly matters more in a lending context you don't want to invest in someone who won't pay you back.

---

## Libraries Used

- pandas, numpy
- matplotlib, seaborn
- scikit-learn (DecisionTreeClassifier, RandomForestClassifier, train_test_split)
