# Association Rule Learning

Unsupervised techniques that discover relationships between items — the classic
"customers who bought X also bought Y" market-basket analysis.

## Notebooks

| File | Method | Notes |
| --- | --- | --- |
| `apriori.ipynb` | Apriori | Learns rules with support/confidence/lift and ranks them by lift |
| `eclat.ipynb` | Eclat | Simplified version that ranks item sets by support |

## Dataset

- `Market_Basket_Optimisation.csv` — 7,500 store transactions, one basket per row.

## Requirements

```bash
pip install jupyter numpy pandas matplotlib apyori
```

> The `apyori` package provides the `apriori` implementation imported in the notebooks
> and is **not** part of scikit-learn, so it must be installed separately.

## How to run

```bash
jupyter notebook        # then open apriori.ipynb or eclat.ipynb
```

Launch Jupyter from this folder so the notebooks can read
`Market_Basket_Optimisation.csv`. Run the cells top to bottom to mine and display the
strongest rules.
