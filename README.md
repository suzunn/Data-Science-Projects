# Data Science Projects

This repository collects notebook-based machine learning and deep learning experiments across tabular data, image classification, natural language processing, recommendation systems, and time series forecasting.

## Project Map

| Area | Contents |
| --- | --- |
| `Classification/` | Credit decisions, customer segmentation labels, game win-rate prediction, AutoML classification, and survey-style classification notebooks. |
| `Clustering/` | Customer clustering and a small clustering walkthrough. |
| `Computer Vision/` | CNN and TensorFlow examples for CIFAR-10, Fashion MNIST, Kannada MNIST, digit recognition, parasite images, and traffic signs. |
| `Natural Language Processing (NLP)/` | Sentiment, review, disaster tweet, duplicate-question, and Amazon review classification notebooks. |
| `Recommendation System/` | Cosine-similarity examples for Netflix and TEDx-style recommendations plus a product recommendation notebook. |
| `Regression/` | House pricing and advertising regression examples. |
| `Time Series/` | Stock and ridership forecasting notebooks. |
| `zingat house pricing/` | Web scraping and regression notebooks for housing-price analysis. |

The root `defect-prediction-xgboost-83.ipynb` notebook is kept at the top level because it is a standalone XGBoost defect prediction experiment.

## Working With The Notebooks

Most projects are self-contained Jupyter notebooks. A typical local workflow is:

```bash
python -m venv .venv
.venv\Scripts\activate
python -m pip install jupyter pandas numpy scikit-learn matplotlib seaborn
jupyter notebook
```

Some notebooks use additional libraries such as TensorFlow, XGBoost, PySpark, or AutoML packages. Install those only for the notebook you plan to run so the base environment stays small.

## Maintenance Notes

- Keep new notebooks inside the closest topic folder instead of adding more top-level files.
- Add a short markdown introduction near the top of each notebook that names the dataset, target variable, and evaluation metric.
- Avoid committing generated datasets, model artifacts, or local notebook checkpoint folders.
- Before committing notebook changes, restart the kernel and run all cells so outputs match the current code.
