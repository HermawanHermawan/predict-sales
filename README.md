PROJECT DESCRIPTION

This project aims to apply regression to predict the sale price of Bulldozers. The dataset being used is a time series data as it contains sales-date component. In this case, we will make use of sales in the past to predict sales in the future. We will try to answer a question, such as:

"How well can we predict the future sale price of a bulldozer, given its characteristics and previous examples of how much similar bulldozers have been sold for?"


The dataset itself can be retrieved from Kaggle https://www.kaggle.com/competitions/bluebook-for-bulldozers/data. There are three main files in the csv format included in the dataset, namely :

1. Train.csv
It contains historical bulldozer sales examples up to 2011 with around 400,000 observations and 50 features, including SalePrice which is the target variable.

2. Valid.csv
It contains historical bulldozer sales examples from January 1 2012 to April 30 2012 with around 12,000 observations with the same features as in Train.csv.

3. Test.csv
It contains historical bulldozer sales examples from May 1 2012 to November 2012 with around 12,000 examples but missing the SalePrice attribute, as this is what will predicted. 


As for the evaluation, we will follow the evaluation metric set by Kaggle, namely root mean squared log error (RMSLE). As with many regression evaluations, the goal will be to get this value as low as possible.


PROJECT STEPS

1. Exploratory Data Analyis
2. Parsing Dates
3. Sort DataFrame by saledate
4. Add datetime parameter for saledate column
5. Converting Columns containing string into categories
6. Filling Missing Values
7. Modeling
8. Building an evaluation function
9. Hyperparameters Tuning with RandomizedSearchCV
10. Train a model with the best hyperparameters
11. Preprocessing the test dataset
12. Make predictions on test data
13. Finding Feature Importance
