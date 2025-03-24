# Churn prediction and analysis
In this project we intend to predict the churning of clients via 
machine learning methods, and then to explain these predictions 
using different techniques. This is based on my master's thesis on 
this same topic. The objective is to structure the code and modify 
the code to make it more clear and effective.

This project is composed of different tasks, which are represented 
in different files. 

    - Data cleaning files.
	- Data visualization files
	- Preprocessing files.
	- Modelling files.
	- Explanation files.

The data can be obtained from [here](https://www.kaggle.com/datasets/merishnasuwal/auto-insurance-churn-analysis-dataset.).

## Data cleaning files
In this step we eliminate variables, remove registers and impute
values where pertinent.

## Data visualization
These files create visualizations of type histogram for each of the different variables,
separated by type of variable: numerical, categorical but numerically codified and categorical.

## Preprocessing
In this phase we prepare the data for the modelling phase. We eliminate several variables and
remove null values from others, either by removing observations or by imputing values.

In this phase we use ordinal encoding, scaling, boruta algorithm for feature selection and SMOTE to prepare the data.
Moreover, the data will be split with 50-25-25, for training, validation and testing, respectively.
The data will be trained on both the regular and the augmented datasets, but will only be evaluated on the regular
evaluation test (without SMOTE).

## Modelling
We will train three kinds of models with cross-validation: a random forest, a 
gradient boosting model, and a neural network. We will use grid search on their parameters to find the best model, 
again using cross validation.

## Evaluation
We want to evaluate the models both locally and globally. We will use several metrics for the evaluation and LIME for 
explanations of the models.
