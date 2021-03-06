# Linear Regression - Fuel Consumption 
The purpose of the project is to explore linear regression models in scikit-learn and fit a model to predict CO2 emissions from a fuel consumption data from various automobiles. We start by calculating a correlation matrix for the numeric variables in our dataset to check for linearity in our data. A heat map is a good way of visualizing the matrix.

![](https://raw.githubusercontent.com/khuzemasunel/Linear-Regression/master/Images/Corr_heatmap.png)

As seen, data shows high linearity between the explanatory variables (features) and the target variable. Even all features have a strong linear relationship with the target variable, "CO2EMISSIONS", we  pick top 3 varaibles as features instead of all of them to prevent overfitting and make a rather generalized model. Hence, "CYLINDERS","ENGINESIZE", and "FUELCONSUMPTION_HWY" are used as features to predict "CO2EMISSIONS".

![](https://raw.githubusercontent.com/khuzemasunel/Linear-Regression/master/Images/co2es.png)

![](https://raw.githubusercontent.com/khuzemasunel/Linear-Regression/master/Images/co2fcc.png)

 
We choose multiple regression models to choose the top performing model.

| Model          | Score |
|----------------|-------|
| Ridge          | 0.856 |
| Lasso          | 0.856 |
| ElasticNet     | 0.855 |
| Lasso_lars     | 0.697 |
| Bayesian_ridge | 0.856 |

