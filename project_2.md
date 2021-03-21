# Project 2: Modeling with DHS Data

[Back to Home Page](https://jeremy-swack.github.io/applied-machine-learning/)

## Background on the Data

For my project, I chose Egypt. The data is a Standard DHS from 2014. The resulting persons object from the data has roughly 65500 observations.

## R Script: Logistic Regression

As shown by the following plot, the model with the highest AUC is the third point with an area of .6305613.

![img_1](lr_plot.png)

I chose the penalty associated with the 3rd point because the 3rd point had the highest AUC. Because it has the largest AUC, it means that model was picking up the most correlation that could be found with th five given variables.

Finally, below are the produced ROC plots for all 5 levels of wealth.

![img_2](lr_auc.png)

The model is clearly better at predicting levels 1 and 5, but there is still clear separation for levles 2-4 as well. This means there is more clear correlation between the variables we choose for our model and the highest and lowest levels of wealth. However, it is less clear for the middle values of wealth.

## R Script: Random Forest Ensemble

Below is a plot of the randomly selected predictors as well as the minimal node size.

![img_3](rf_res.png)

After selecting the best possible model, I produced the ROC plots for the model.

![img_4](rf_auc.png)

These ROC plots are very similar to the logsitic regression ROC plots. Once again, the model is able to differentiate wealth levels 1 and 5 the best. However, it seems the random forest model is slightly better at differentiating between wealth level 2-4, but this difference is very slight at best.

## Python Script: Logistic Regression

After training the logistic model, I got the following characteristics:

| Name of Output | Value |
| --- | ----------- |
| Accuracy | 0.7856011 |
| average_loss | 0.48615587 |
| loss | 0.48615107 |
| global_step | 15380 |

After adding the derived feature columns:

| Name of Output | Value |
| --- | ----------- |
| Accuracy | 0.78365034 |
| average_loss | 0.48245367 |
| loss | 0.48246303 |
| global_step | 15380 |

## Python Script: Gradient Boosting Model using Decision Trees

## Analyzing all the Models
