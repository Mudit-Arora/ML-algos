# Reinforcement Learning

Online decision-making algorithms that learn which action pays off best by balancing
**exploration** and **exploitation**. Both notebooks solve the same multi-armed bandit
problem: picking which of 10 ads to show to maximize click-through.

## Notebooks

| File | Algorithm |
| --- | --- |
| `upper_confidence_bound.ipynb` | Upper Confidence Bound (UCB) |
| `thompson_sampling.ipynb` | Thompson Sampling |

Each notebook runs the strategy over the dataset and plots a histogram of how often each
ad was selected.

## Dataset

- `Ads_CTR_Optimisation.csv` — 10,000 rounds × 10 ads, with a 1/0 indicating whether the
  ad was clicked. (Used to simulate live rewards.)

## Requirements

```bash
pip install jupyter numpy pandas matplotlib
```

These notebooks rely only on NumPy, pandas, matplotlib, and the standard-library `math`
module — no scikit-learn needed.

## How to run

```bash
jupyter notebook        # then open either notebook
```

Launch Jupyter from this folder so the notebooks can read `Ads_CTR_Optimisation.csv`. Run
the cells top to bottom to simulate the strategy and view the selection histogram.
