# Deep Learning

Neural networks built with TensorFlow / Keras.

## Notebooks

| File | Model | Dataset |
| --- | --- | --- |
| `artificial_neural_network.ipynb` | Artificial Neural Network (ANN) for binary classification | `Churn_Modelling.csv` |
| `convolutional_neural_network.ipynb` | Convolutional Neural Network (CNN) for image classification (cat vs. dog) | image folder — **not included**, see below |

### ANN
Predicts whether a bank customer will leave (churn). Encodes categorical columns,
scales features, builds a dense Keras model, trains it, and evaluates with a confusion
matrix and accuracy.

### CNN
Classifies images using Keras `ImageDataGenerator`. The notebook expects an image
dataset laid out like this in a `dataset/` folder **next to the notebook**:

```
dataset/
├── training_set/
│   ├── cats/
│   └── dogs/
├── test_set/
│   ├── cats/
│   └── dogs/
└── single_prediction/   # or check/ — single images to classify
```

This image dataset is **not included** in the repository. Download a cat/dog image set
(e.g. the standard "Cats and Dogs" dataset) and arrange it as above before running the
CNN notebook.

## Datasets

- `Churn_Modelling.csv` — 10,000 bank customers with a 0/1 "Exited" label (used by the ANN).

## Requirements

```bash
pip install jupyter numpy pandas tensorflow keras pillow scikit-learn
```

- `tensorflow` / `keras` — the deep learning framework.
- `pillow` — required by Keras to load and preprocess images for the CNN.
- `scikit-learn` — used by the ANN for encoding/scaling and evaluation.

> A GPU is optional; these models are small enough to train on a CPU, just more slowly.

## How to run

```bash
jupyter notebook        # then open either notebook
```

Launch Jupyter from this folder. Run the ANN notebook directly. For the CNN notebook,
first create the `dataset/` folder described above, then run the cells top to bottom.
