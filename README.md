# Future-sales-prediction-for-Russian-shops
The project origin: https://www.kaggle.com/c/competitive-data-science-predict-future-sales/data

The goal of this project is to use the past 34 months daily historical sales data of Russia stores to predict the total amount of products will be sold in the next month (35th month). Obviously, it is a time series problem.
## Model Selection
For the model, LSTM (Partially applied) and XGBoost were used.
## Evaluation Method
Root mean squared error was used to evaluate final submission, and true target values are clipped into [0,20] range.
## Result
The best result ended up with RMSE 
