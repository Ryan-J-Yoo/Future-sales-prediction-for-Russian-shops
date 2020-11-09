# Future-sales-prediction-for-Russian-shops
The project origin: https://www.kaggle.com/c/competitive-data-science-predict-future-sales/data

The goal of this project is to use the past 34 months daily historical sales data of Russia stores to predict the total amount of products will be sold in the next month (35th month). Obviously, it is a time series problem.
## Data Description
sales_train.csv - the training set. Daily historical data from January 2013 to October 2015.
test.csv - the test set. You need to forecast the sales for these shops and products for November 2015.
sample_submission.csv - a sample submission file in the correct format.
items.csv - supplemental information about the items/products.
item_categories.csv  - supplemental information about the items categories.
shops.csv- supplemental information about the shops.
Data fields
ID - an Id that represents a (Shop, Item) tuple within the test set
shop_id - unique identifier of a shop
item_id - unique identifier of a product
item_category_id - unique identifier of item category
item_cnt_day - number of products sold. You are predicting a monthly amount of this measure
item_price - current price of an item
date - date in format dd/mm/yyyy
date_block_num - a consecutive month number, used for convenience. January 2013 is 0, February 2013 is 1,..., October 2015 is 33
item_name - name of item
shop_name - name of shop
item_category_name - name of item category
## Model Selection
For the model, LSTM (Partially applied) and XGBoost were used.
## Evaluation Method
Root mean squared error was used to evaluate final submission, and true target values are clipped into [0,20] range.
## Result
The best result ended up with RMSE 
