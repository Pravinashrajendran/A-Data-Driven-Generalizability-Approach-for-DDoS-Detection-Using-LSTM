# A Data-Driven Generalizability Approach for DDoS Detection Using LSTM

## Overview

This research project explores the use of a Long Short-Term Memory (LSTM) neural network to classify network traffic for Distributed Denial-of-Service (DDoS) detection. The repository description references the CIC-DDoS2019 dataset and comparison with traditional machine-learning classifiers.

The goal is to study whether sequential traffic patterns can help distinguish benign from malicious traffic. This README documents the stated research direction; it does not claim a specific accuracy or performance improvement without reproducible result files.

## Research questions

- Can sequential traffic features be used by an LSTM-based classifier for DDoS detection?
- How does the LSTM approach compare with selected traditional machine-learning models?
- How do preprocessing and feature selection affect evaluation?

## Intended workflow

1. Obtain the appropriate CIC-DDoS2019 data and review its licence and usage terms.
2. Inspect and clean the traffic data, handling missing values and non-numeric fields as appropriate.
3. Split the dataset into training, validation, and test sets without data leakage.
4. Fit preprocessing steps using the training set only.
5. Train an LSTM model on correctly shaped sequential input and train comparison models.
6. Evaluate with precision, recall, F1-score, confusion matrix, and other relevant metrics.
7. Record the exact split, features, parameters, environment, and results so the experiment can be reproduced.

## Technology stack

The project description identifies the following tools:

- Python
- TensorFlow / Keras
- scikit-learn
- Pandas
- NumPy

Confirm package versions and available training scripts before attempting to reproduce the experiment.

## Dataset

The project references **CIC-DDoS2019**. Use the official dataset source and follow its terms. Do not assume that the HTML file or downloaded assets currently in this repository are a clean, complete dataset or a reproducible data pipeline.

## Repository status and reproducibility

The current repository contains the README plus a number of downloaded web assets and files with generic or opaque names. These are not self-explanatory source-code filenames, so the project needs a separate cleanup pass before it can be presented as fully reproducible research.

Recommended structure for the next iteration:

```text
.
├── README.md
├── requirements.txt
├── data/
│   └── README.md
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_preprocessing.ipynb
│   └── 03_model_training_evaluation.ipynb
├── src/
│   ├── preprocessing.py
│   ├── train_lstm.py
│   └── evaluate.py
├── results/
│   └── README.md
└── docs/
    └── methodology.md
```

This is a recommended target layout, not a description of files already present. Avoid committing large raw datasets, downloaded site assets, credentials, or environment-specific files unless there is a clear reason and permission to do so.

## How to reproduce

The current repository does not yet provide enough clearly named scripts and dependency information to give a verified end-to-end command sequence. Once the preprocessing, training, and evaluation entry points and their dependencies are identified, add exact commands here, along with expected outputs.

## Evaluation checklist

- [ ] Document dataset source and selected attack classes
- [ ] Document preprocessing and feature selection
- [ ] Document train/validation/test strategy
- [ ] Compare LSTM with clearly specified baselines
- [ ] Report precision, recall, F1-score, and confusion matrix
- [ ] Save random seeds, package versions, and model configuration
- [ ] Include results only when traceable to reproducible runs

## Responsible use

This project is intended for research and education. Use traffic datasets and test environments only in accordance with their terms and with appropriate authorisation.

## Author

**Pravinash SMR**
