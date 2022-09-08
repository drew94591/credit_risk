# Credit Risk
This application uses various techniques to train and evaluate models with imbalanced classes.  It also uses a dataset of historical lending activity to build both an original model and a resampled
model to determine the accuracy in identifying the creditworthiness of borrowers.

---


## Technologies

This application leverages python 3.7 with the following libraries and packages:

* [numpy](https://numpy.org) - The fundamental package for scientific computing in Python.

* [path](https://docs.python.org/3/library/pathlib.html) - Used to define file path

* [pandas](https://github.com/pandas-dev/pandas) - A flexible and power data analysis/manipulation Python library used in financial calculations.

* [scikit-learn](https://scikit-learn.org/) - A Python machine learning library that provides supervised and unsupervised learning algorithms.

* [imbalance-learn](https://pypi.org/project/imbalanced-learn/) - A Python package offering a number of re-sampling techniques commonly used in datasets showing strong between-class imbalance.

---

## Installation Guide

Before running the application first install the following dependencies.

```python
pip install -U scikit-learn
conda install -c conda-forge imbalanced_learn
```

---

## Usage

To use the credit risk application you must first launch Jupyter Lab by executing the following command within Git Bash:

```python
jupyter lab
```

Within Jupyter Lab you should then be able to run and execute the following notebook:

``` python
credit_risk_resampling.ipynb
```

## Overview of the Analysis

* The purpose of the application is to evaluate several linear regression models using the provided dataset to accurately train, predict, test and identify the creditworthiness of borrowers.
* The financial information contained within the data set such as loan size, interest rate, borrower's income, debt-to-income ratio, number of accounts, derogatory marks, and total debt helps the models predict what the loan status for each borrower would be.
* Using the value_counts function of the loan status, we should be able to predict if the borrower's loan is a healthy loan or a high-risk loan.
* The machine learning process follows a basic pattern of model-fit-predict.  In this three-stage pattern, the machine learning algorithm is provided data (the model stage), and the algorithm learns from this data (the fit stage) to form a predictive model (the predict stage).
* The data set provided appears to be imbalanced.  Thus we ran two separate LogisticRegression models, one with the original data set as is and the other with a RandomOverSampler for a more balanced data set.  With these two models we are trying to evaluate which one had the most accuracy in predicting a borrower's loan status comparing the precision and recall scores.

## Results

* Machine Learning Model 1:
  * Model 1 used the original data set as is and had a balanced accuracy score of around 95%.  The precision score for this model was 85% and the recall score was 91%.

* Machine Learning Model 2:
  * Model 2 used the resampling of the data set and had a balanced accuracy score of 99% which increased compared to Model 1.  Though the precision score for this model slightly dropped 1% to 84% than in Model 1. The recall score significantly improved to around 99%. 

## Summary

* Since both the accuracy score and the recall score has increased substantially in Model 2 compared to Model 1 without sacrificing much in regards to precision we can determine that Model 2 performed the best and is the model that should be used.
* The accuracy performance in trying to predict the number of high-risk loans is much more important than predicting the number of healthy loans because you wouldn't want to issue any new loans to a borrower whose already in a high-risk loan.

---

## Contributors

Brought to you by [Drew Herrera](https://www.linkedin.com/in/drew94591).

---

## License

Licensed under the MIT License. Copyright 2022 Drew Herrera.


