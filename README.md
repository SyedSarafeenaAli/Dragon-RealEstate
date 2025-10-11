# NOTES:-

Regression: In machine learning, regression is a supervised learning (dataset provided is labelled) method that uses knowledge of the connection between independent variables (features) and a continuous target variable to predict continuous numerical values. In order to translate input features into a continuous output—such as house prices, stock trends, or temperatures for new, unseen data—a model must be trained on a labelled dataset.

Regression Metrics: Common regression metrics in scikit-learn include -                                                                                          
1. Mean Absolute Error (MAE)
2. Mean Squared Error (MSE)
3. R-squared (R²) Score
4. Root Mean Squared Error (RMSE)

# OBJECTIVE:-

The Dragon-RealEstate project aims to develop a prediction model that, given a collection of property and geographical characteristics, predicts the sale price of residential real estate (houses). The goal is to give all parties involved in real estate (buyers, sellers, and agents) a tool to obtain an equitable, data-driven appraisal of a property based on its features and location.
Estimate the anticipated market price of a property based on its input factors, such as its size, number of rooms, location, etc.
Assist in decision-making by determining which features have the biggest impact on price, identifying listings that are overpriced or underpriced, and offering advice on how to enhance features to raise value.
The model should ideally include interpretability (so users can trust and comprehend predictions) and generalise well to new, unseen houses.

# PROBLEM STATEMENT:- 

A vector of characteristics characterising a home (and perhaps its surroundings) is the input.
A scalar, or estimated sale price, is the output (continuous value).
Key factors and limitations:
1. Numerous correlated variables affect real estate prices; managing nonlinearity, feature interaction, and multicollinearity is crucial.
2. Error metrics may be disproportionately impacted by outliers, such as extremely expensive or inexpensive homes.
3. There may be inconsistent or missing values in the dataset (e.g., categorical encoding errors, missing feature values).
4. Temporal or spatial effects: time (year, market trends) and place (neighbourhood, accessibility to facilities) may be important.
5. In order for the model to generalise to houses that are not visible, overfitting must be avoided.
6. Real-world utility should be reflected in evaluation measures, such as Mean Absolute Error, Root Mean Squared Error, and possibly percentage error metrics.
Hence, the project can be claimed as a Regression (Supervised Learning) problem aiming to forecast home values based on property attributes, emphasising precision, applicability, and comprehensibility.

# DATASET AND FEATURES:- 

SOURCE: The dataset “Dragon Real Estate – Price Predictor” is available on Kaggle.

Link: https://www.kaggle.com/datasets/arslanali4343/real-estate-dataset

DATASET STRUCTURE AND FEATURES:

An inferred schema of the dataset, combining common features seen in such repos and the traditional Boston housing features. 

COLUMN/FEATURE	:   TYPE          :            DESCRIPTION

CRIM	          : Numeric(float)	:  Per capita crime rate by town/neighborhood

ZN	            : Numeric	        :  Proportion of residential land zoned for large lots

INDUS	          : Numeric         :  Proportion of non-retail business (industrial) acres per town

CHAS	          : Binary/Integer	:  Charles River dummy variable (1 if tract bounds river, else 0)

NOX	            : Numeric         :  Nitric oxides concentration (parts per 10 million)

RM	            : Numeric	        :  Average number of rooms per dwelling

AGE	            : Numeric	        :  Proportion of owner-occupied units built prior to some cutoff (e.g. 1940)

DIS	            : Numeric	        :  Weighted distances to employment centers

RAD	            : Integer	        :  Index of accessibility to radial highways

TAX	        	  : Numeric         :  Full-value property tax rate per $10,000

PTRATIO         : Numeric	        :  Pupil-teacher ratio by town

B               : Numeric         :  A transformation involving proportion of black population 

LSTAT           : Numeric	        :  % lower status of the population (i.e. socioeconomic measure)

MEDV/PRICE   	  : Numeric	        :  Target — median value of homes (in $1000s) or sale price
