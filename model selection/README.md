# Model Selection

Techniques for evaluating a model more reliably and tuning its hyperparameters. Both
notebooks train a kernel SVM on `Social_Network_Ads.csv` and add a model-selection step.

## Notebooks

| File | Technique | What it adds |
| --- | --- | --- |
| `k_fold_cross_validation.ipynb` | k-Fold Cross Validation | Estimates accuracy across 10 folds (mean and standard deviation) instead of a single split |
| `grid_search.ipynb` | Grid Search | Searches SVM hyperparameters (`C`, `kernel`, `gamma`) with `GridSearchCV` to find the best combination |

## Datasets

- `Social_Network_Ads.csv` — age and estimated salary with a 0/1 purchase label.
- `Data.csv` — included as an additional sample dataset.

## Requirements

```bash
pip install jupyter numpy pandas matplotlib scikit-learn
```

## How to run

```bash
jupyter notebook        # then open either notebook
```

Launch Jupyter from this folder so the notebooks can read their CSV. Run the cells top to
bottom to train the model and apply cross-validation / grid search.
