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

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.


---

## Contributors

Brought to you by [Drew Herrera](https://www.linkedin.com/in/drew94591).

---

## License

Licensed under the MIT License. Copyright 2022 Drew Herrera.


