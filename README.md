# ML-algos

A hands-on collection of classic Machine Learning algorithms, each implemented as a
self-contained Jupyter notebook with a small example dataset. The repository is organized
by topic so you can jump straight to the technique you want to study.

## Topics

| Folder | What it covers |
| --- | --- |
| [`data-preprocessing/`](data-preprocessing) | Cleaning, encoding, and scaling raw data before modelling |
| [`regression/`](regression) | Predicting continuous values (linear, polynomial, SVR, decision tree) |
| [`classification/`](classification) | Predicting discrete classes (logistic regression, KNN, SVM, naive bayes, trees) |
| [`clustering/`](clustering) | Grouping unlabelled data (K-Means, hierarchical) |
| [`association rule learning/`](association%20rule%20learning) | Finding item relationships (Apriori, Eclat) |
| [`reinforcement learning/`](reinforcement%20learning) | Online decision making (UCB, Thompson Sampling) |
| [`natural language processing/`](natural%20language%20processing) | Text cleaning and bag-of-words sentiment classification |
| [`deep learning/`](deep%20learning) | Artificial and convolutional neural networks with TensorFlow/Keras |
| [`dimensionality reduction/`](dimensionality%20reduction) | Reducing features (PCA, Kernel PCA) |
| [`model selection/`](model%20selection) | Evaluating and tuning models (k-fold CV, grid search) |

## Requirements

- Python 3.8+
- [Jupyter](https://jupyter.org/) (Notebook or Lab) to open and run the `.ipynb` files

Install the core libraries used across the notebooks:

```bash
pip install jupyter numpy pandas matplotlib scikit-learn scipy
```

A few folders need extra packages on top of the core set:

```bash
# association rule learning
pip install apyori

# natural language processing
pip install nltk

# deep learning
pip install tensorflow keras pillow
```

> Tip: using a virtual environment keeps these dependencies isolated.
>
> ```bash
> python3 -m venv .venv
> source .venv/bin/activate      # Windows: .venv\Scripts\activate
> pip install jupyter numpy pandas matplotlib scikit-learn scipy apyori nltk tensorflow keras pillow
> ```

## How to run

1. Clone the repository and `cd` into it.
2. Install the requirements above.
3. Launch Jupyter:
   ```bash
   jupyter notebook        # or: jupyter lab
   ```
4. Open any `.ipynb` file inside a topic folder and run the cells top to bottom
   (`Shift + Enter`). Each notebook loads its dataset from the same folder, so no
   path changes are needed.

Every topic folder has its own `README.md` describing the individual notebooks and any
notebook-specific setup.
