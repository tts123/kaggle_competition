# kaggle_competition
### House Prices: Advanced Regression Techniques
### Predict sales prices and practice feature engineering, RFs, and gradient boosting

#### Step 1: Download data from kaggle, clean and analyze (https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)
#### Step 2: By Supervised learning the data and using advance regression techniques, get the best model to predict the sales price.
#### Step 3: Use the best model in the unseen data to predict the house prices.

#### Obervation:
#### I have download data from kaggle, cleaned and analyzed. Since the data had large number of columns, I divided the data into categorical and continuous data. Some of the columns had a lot of missing values so I decided to drop them. For continuous value, I have replace the missing value with the mean and for categorical value, I replace the missing value with the one having higher number of frequency. After finding the correlation to the sale price, I decided to drop the columns that aren't helping that much. At the end I merged the two data into one.

#### I tried simple linear, multiple and polynomial regression, lasso and ridge regression (which are not in this notebook) and xgbregressor and lgbregressor. Out of all, I got the best result with lgbregressor with 97% training score and 87% cross value score.  

#### Finally, I cleaned and analyzed the test data just like the train data. I used the lgbregressor model to the test data to get the final house sale price. After converting the data frame to csv, I submitted the csv to the kaggle competition and got public score of 0.43.



