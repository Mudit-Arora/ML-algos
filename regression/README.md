# Regression

Supervised learning models that predict a **continuous** value (e.g. salary, profit).
Each notebook trains a model, makes predictions, and (where applicable) visualizes the fit.

## Notebooks

| File | Model | Dataset |
| --- | --- | --- |
| `simple_linear_regression.ipynb` | Linear regression with one feature | `Salary_Data.csv` (years of experience → salary) |
| `multiple_linear_regression.ipynb` | Linear regression with several features | `50_Startups.csv` (startup spend → profit) |
| `polynomial_regression.ipynb` | Polynomial regression | `Position_Salaries.csv` (job level → salary) |
| `support_vector_machine.ipynb` | Support Vector Regression (SVR) | `Position_Salaries.csv` |
| `decision_tree_regression.ipynb` | Decision tree regressor | `Position_Salaries.csv` |

## Requirements

```bash
pip install jupyter numpy pandas matplotlib scikit-learn
```

## How to run

```bash
jupyter notebook        # then open any notebook above
```

Launch Jupyter from this folder so each notebook can find its CSV. Run the cells top to
bottom to train the model and view the resulting plots/predictions.
