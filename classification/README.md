# Classification

Supervised learning models that predict a **discrete class label**. Every notebook here
trains on `Social_Network_Ads.csv` to predict whether a user purchased a product, then
reports a confusion matrix and accuracy and plots the decision boundary.

## Notebooks

| File | Model |
| --- | --- |
| `logistic_regression.ipynb` | Logistic regression |
| `k_nearest_neighbors.ipynb` | K-Nearest Neighbors (KNN) |
| `support_vector_machine.ipynb` | Support Vector Machine (linear kernel) |
| `kernel_svm.ipynb` | Support Vector Machine (RBF/kernel) |
| `naive_bayes.ipynb` | Gaussian Naive Bayes |
| `decision_tree_classification.ipynb` | Decision tree classifier |
| `random_forest_classification.ipynb` | Random forest classifier |

## Dataset

- `Social_Network_Ads.csv` — age and estimated salary of users with a 0/1 label for
  whether they purchased.

## Requirements

```bash
pip install jupyter numpy pandas matplotlib scikit-learn
```

## How to run

```bash
jupyter notebook        # then open any notebook above
```

Launch Jupyter from this folder so each notebook can load `Social_Network_Ads.csv`. Run
the cells top to bottom to train, evaluate, and visualize the classifier.
