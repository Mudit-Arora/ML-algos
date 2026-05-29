# Natural Language Processing

A basic NLP pipeline that turns raw text into features and classifies sentiment.

## Notebook

| File | What it does |
| --- | --- |
| `natural_language_processing.ipynb` | Cleans restaurant reviews (lowercasing, removing non-letters, removing stopwords, Porter stemming), builds a bag-of-words matrix with `CountVectorizer`, then trains a Gaussian Naive Bayes classifier and reports a confusion matrix and accuracy. |

## Dataset

- `Restaurant_Reviews.tsv` — 1,000 restaurant reviews, each labelled positive (1) or
  negative (0). Tab-separated (note the `delimiter='\t'` in the notebook).

## Requirements

```bash
pip install jupyter numpy pandas matplotlib scikit-learn nltk
```

The notebook also downloads the NLTK stopwords list on first run:

```python
import nltk
nltk.download('stopwords')
```

This download cell is included in the notebook — run it once before the cleaning step.

## How to run

```bash
jupyter notebook natural_language_processing.ipynb
```

Launch Jupyter from this folder so the notebook can read `Restaurant_Reviews.tsv`. Run
the cells top to bottom (including the `nltk.download` cell) to clean the text, train the
model, and view the results.
