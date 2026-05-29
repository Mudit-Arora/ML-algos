# Clustering

Unsupervised learning that groups **unlabelled** data into clusters. Both notebooks
segment mall customers by annual income and spending score, then visualize the clusters.

## Notebooks

| File | Method | Notes |
| --- | --- | --- |
| `k_means_clustering.ipynb` | K-Means | Uses the elbow method (WCSS) to choose the number of clusters |
| `hierarchical_clustering.ipynb` | Agglomerative hierarchical clustering | Uses a `scipy` dendrogram to choose the number of clusters |

## Dataset

- `Mall_Customers.csv` — customer ID, gender, age, annual income, and spending score.

## Requirements

```bash
pip install jupyter numpy pandas matplotlib scikit-learn scipy
```

(`scipy` is needed for the dendrogram in the hierarchical notebook.)

## How to run

```bash
jupyter notebook        # then open either notebook
```

Launch Jupyter from this folder so the notebooks can read `Mall_Customers.csv`. Run the
cells top to bottom to build the clusters and view the plots.
