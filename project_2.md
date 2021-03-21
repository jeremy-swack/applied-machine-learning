# Project 2: Modeling with DHS Data

[Back to Home Page](https://jeremy-swack.github.io/applied-machine-learning/)

## R Script: Logistic Regression

As shown by the following plot, the model with the highest AUC is the third point with an area of .6305613.

![img_1](lr_plot.png)

I chose the penalty that came with the script as it seemed to a model that could differentiate between all 5 levels of wealth.

```
lr_reg_grid <- tibble(penalty = 10^seq(-4, -1, length.out = 30))
```

Finally, below are the produced ROC plots for all 5 levels of wealth.

![img_2](lr_auc.png)

The model is clearly better at predicting levels 1 and 5, but there is still clear separation for levles 2-4 as well.

## R Script: Random Forest Ensemble

## Python Script: Logistic Regression

## Python Script: Gradient Boosting Model using Decision Trees

## Analyzing all the Models
