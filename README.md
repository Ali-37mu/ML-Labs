# ML-Labs

Here all Machine Learning Labs

# SVM Assignment - Iris Dataset

Assignment from the SVM section of the machine learning course. We use Support Vector Machines to classify Iris flower species based on their measurements.

## Dataset

The classic Iris dataset: 150 samples across 3 species (setosa, versicolor, virginica), with 4 features each: sepal length, sepal width, petal length, and petal width (all in cm). Loaded straight from seaborn with `sns.load_dataset('iris')`.

## What I did

**EDA**: Made a pairplot to see how the features separate the species visually. Setosa is clearly the most separable one. Also made a KDE plot of sepal length vs sepal width just for the setosa species.

**Training**: Dropped the species column to get X, split 70/30 with `random_state=101`, then trained a default `SVC()` on the training set.

**Evaluation**: Used confusion matrix and classification report. Got 98% overall accuracy. Only 1 misclassification  a versicolor sample predicted as virginica, which makes sense since those two overlap the most in feature space.

**GridSearchCV**: Tried different values of C (`0.1, 1, 10, 100`) and gamma (`1, 0.1, 0.01, 0.001`) with an RBF kernel using 3-fold cross validation. The results came out the same as the baseline, which just shows how clean this dataset is.

## Notes

The model performs really well with basically no effort, which makes sense given how small and clean the Iris dataset is. In a real project with messier data, the GridSearch step would matter a lot more. The main takeaway is that SVMs with an RBF kernel work great for this kind of multi-class classification problem.
