# Advanced-Regression
This responsitory used to complete the assignment from Upgrad Course

## Agenda
* [Problem statement](#problem-statement)
* [Dataset](#approach-methods)
* [Data Understanding, Preparation and EDA ](#data-understanding-preparation-and-eda)
* [Training Step](#training-step)
* [Model Building and Evaluation](#model-building-and-evaluation)
* [Environment](#environment)
* [Usage](#usage)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)

## Problem statement
- A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia.

- The company wants to know:
1. Which variables are significant in predicting the price of a house, and
2. How well those variables describe the price of a house.

- I train a model which predicts price of houses with the available independent variables.This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

## Dataset
- You can find data in 'data/train.csv'
- Click [here](https://cdn.upgrad.com/UpGrad/temp/87f67e28-c47e-4725-ae3c-111142c7eaba/data_description.txt) for the details of the various variables.

## Data Understanding, Preparation and EDA  
- Data visualize
- Drop columns had over 70% null value
- Drop columns had only one value
- Transform columns (encoding, datetime, ect.)
- Fillna by mean, mode value
- Imute outlier (Fill outlier with mean, mode value)

## Training Step
- Load processed data
- Drop correlative dependence columns
- LabelEcoder categorical columns
- Split x,y from train data
- Feature selections (default: [25%, 50%, 75%, 99%]). We use feature ranking with recursive feature elimination ([RFE](https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.RFE.html))
- Scaling numerical columns
- Train with [Linear Regression model](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html), [Decission Tree Regressor model](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeRegressor.html)
## Model Building and Evaluation

## Environment
```bash
cd src
pip install -r requirement.py
```

## Usage
I impletation as in ipynb file and py file.
* I complete my assignment in house_predict.ipynb
* I run train.py if you want to utilize my model.
```bash
cd src
python train.py
```


## Acknowledgements

1. https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html
2. https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeRegressor.html

## Contact
Created by [Huynh Viet Cuong](https://cuonghv0298.github.io/) - feel free to contact me!