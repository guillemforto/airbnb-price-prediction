# Airbnb Price Prediction &nbsp; &nbsp; <img alt="airbnb_logo.png" src="airbnb_logo.png" width="55" height="75">

In view of the number of housing units in Paris, how to define a fair price according to the location, the equipment or the capacity of a unit?

## Context

Since its inception in 2008, the number of Airbnb rentals listed on its website has grown exponentially each year. In France, no city is more popular than Paris. This means that Paris is one of the most popular markets for Airbnb in Europe, with more than 60 000 homes listed in 2018.<br>

Since tree-based models such as XGBoost or CatBoost have proven to be the new best-in-class techniques in recent years, the main challenge of this competition was to find good features to predict the price.<br>
Unsurprisingly, some of these turned up to be the neighborhood, the number of accommodates and the number of bedrooms.<br>
If you want more details of what was done, feel free to check out the keynote presentation of this repository: [`keynote_pres.pdf`](keynote_pres.pdf).

**Dates:** November - December 2019<br>
This project was part of an in-class Kaggle competition, for the Quantitative marketing course at Toulouse School of Economics.

## Installation of libraries
To run the code, you'll need Python 3 installed with pip.<br>
Here is a non-exhaustive list of dependencies you might want to install:
```bash
pip install xgboost
pip install catboost
pip install tensorflow
pip install scikit-learn
```

## Running the code
Start by downloading the necessary data files:
- `train_airbnb.csv` contains the initial basic features available on Kaggle and the variable price from which to learn: https://www.dropbox.com/s/mq6905c2xhxqgzf/train_airbnb.csv?dl=0
- `test_airbnb.csv` contains new observations whose price is unknown: https://www.dropbox.com/s/umficstiqokaq6i/test_airbnb.csv?dl=0

You're then ready to run the notebook [`main_notebook.ipynb`](main_notebook.ipynb), which contains all the code to build the engineered features and to train the models. You'll need Jupyter notebook (>= v. 6.0.3) to run it.
