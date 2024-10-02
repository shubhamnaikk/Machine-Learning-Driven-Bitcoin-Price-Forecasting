# Project Overview

Created a random forest model to forecast Bitcoin prices using historical price and sentiment data, achieving
accurate next-day predictions.
Transitioned to XGBoost and incorporated advanced predictors, resulting in improved accuracy and robustness
in price forecasts.
Developed a robust backtesting system to evaluate model performance, enabling extensions to other
cryptocurrencies and multi-day predictions.

**Project Steps**

* Load in data
* Clean and merge data
* Create an initial machine learning model and estimate accuracy
* Switch to a more powerful model and improve our predictors

File overview:

* `prediction.ipynb` - a Jupyter notebook that contains the code to predict Bitcoin prices
* `sentiment.ipynb` - a Jupyter notebook that creates our wikipedia edit dataset.

# Local Setup

## Installation

To follow this project, please install the following locally:

* JupyerLab
* Python 3.8+
* Python packages
    * pandas
    * yfinance
    * scikit-learn
    * xgboost
    * mwclient
    * transformers

## Running

First, run the code in `sentiment.ipynb` to generate a new Wikipedia edits dataset.  The dataset committed in the repo is old, and this will get the edits up to the present day.

Second, run the code in `prediction.ipynb`.  By default, this will load data from an existing `btc.csv` file.  Removing that code will ensure that it downloads the newest data from Yahoo Finance.
