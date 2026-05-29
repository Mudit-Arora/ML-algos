# Data Preprocessing

The first step in any ML pipeline: turning raw data into a clean, numeric, scaled form
that algorithms can consume.

## Notebook

| File | What it does |
| --- | --- |
| `data_preprocessing.ipynb` | Loads `Data.csv`, fills missing values with `SimpleImputer`, one-hot encodes the categorical country column, label-encodes the target, splits into train/test sets, and applies feature scaling with `StandardScaler`. |

## Dataset

- `Data.csv` — small sample with a categorical feature (Country), two numeric features
  (Age, Salary, including missing values), and a yes/no target (Purchased).

## Requirements

```bash
pip install jupyter numpy pandas matplotlib scikit-learn
```

## How to run

```bash
jupyter notebook data_preprocessing.ipynb
```

Run the cells top to bottom. The notebook reads `Data.csv` from this folder, so launch
Jupyter from here (or keep the CSV alongside the notebook).
