# Deep Learning for Forecasting the Australian Unemployment Rate using Stochastic Gradient Boosted Models (GBM): A Learning Curve

## Abstract

The COVID-19 crisis sets the development of unemployment rates in the spotlight of public interest. Pandemics are events that cannot be foreseen by any algorithm because they are so rare. However, it is important to understand the ‘normal’ evolution of unemployment in order to identify particular impacts of pandemics on employment, and what to do to improve the stability of the Australian labour market.
This report reflects my investigation into the evolution of the Australian unemployment rate using a machine learning algorithm and a neural network. The aim is to provide the basic model to effectively and efficiently predict the unemployment rate based on a set of predictors used by the Australian Bureau of Statistics.

The outcome is that neural networks do not perform as well as the gradient boosted decision trees selected for this assessment, in terms of RMSE of predictions. Neural networks require (by nature of complexity) significantly more computation time, and are not as interpretable as decision trees. However, as shown by the rather suboptimal predictive performance achieve, significant improvement will need to be achieved in further work dedicated to both methods. Such can be investigations into more sophisticated models in deep learning (e.g. LSTM), and attempts in other decision tree models. Also, improvement of the data may result in improved predictions.

## Data

The dataset for this work represents a sample of Australian national unemployment rates expressed in figures per quarters, from Q1 1981 to Q4 2019, as dependent variable, and a number of independent variables representing economic figures as described below. 

The data was collected from the Australian Bureau of Statistics (ABS). A total of 155 observations was collected.

## Method

Stochastic Gradient Boosted Models (GBM) with hyperparameters:

- Number of nodes per tree: Vary 2, 4 (if time left: 6); seen the limited number of variables my guess is that rather low numbers will do fine.
- Shrinkage parameter: 0.001, 0.005, 0.01, 0.05 Number of trees: 100, 250, 500, 750
- Loss function: “laplace”

### [Report with code in R](https://github.com/sachaschwab/R-LSTM-XBoost/blob/master/R%20code/A3_Sacha_Schwab_Markdown.Rmd)

