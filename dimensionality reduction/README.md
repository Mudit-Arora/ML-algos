# Dimensionality Reduction

Techniques that compress many features into a few while preserving the information that
matters — useful for visualization and for speeding up models. Both notebooks reduce a
wine dataset's features to 2 components, then train a logistic regression classifier and
plot the decision regions.

## Notebooks

| File | Method |
| --- | --- |
| `principal_component_analysis.ipynb` | Principal Component Analysis (PCA) — linear |
| `kernel_pca.ipynb` | Kernel PCA — non-linear (RBF kernel) |

## Dataset

These notebooks use the Wine dataset (typically `Wine.csv`). If a CSV is referenced in
the first cell but missing from this folder, download the standard Wine dataset and place
it alongside the notebook before running.

## Requirements

```bash
pip install jupyter numpy pandas matplotlib scikit-learn
```

## How to run

```bash
jupyter notebook        # then open either notebook
```

Launch Jupyter from this folder. Run the cells top to bottom to reduce dimensions, train
the classifier, and view the decision-boundary plots.
