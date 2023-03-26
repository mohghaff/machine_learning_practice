Machine Learning Practice -- Day 12

The following code performs linear regression on a Melbourne Housing dataset using different regularization techniques, Lasso and Ridge regression.

First, the required libraries are imported, which include pandas for data manipulation and sklearn for machine learning algorithms. Then, the dataset is loaded into a pandas dataframe from a csv file named Melbourne_housing_FULL.csv.

Next, the columns of interest are selected and missing values are handled. Specifically, the columns 'Propertycount', 'Distance', 'Bedroom2', 'Bathroom', 'Car' are filled with zeros using the .loc method. The columns 'Landsize' and 'BuildingArea' are filled with their respective means using the .fillna() method. Rows with any remaining missing values are dropped using the .dropna() method.

The categorical columns are then converted into numerical values using one-hot encoding via the .get_dummies() method. The target variable 'Price' is then separated from the features and the dataset is split into training and testing sets using train_test_split() from sklearn with a test size of 0.3 and a random state of 2.

The first model is then built using the LinearRegression() method and trained on the training dataset using the .fit() method. The R-squared value of the model is computed using the .score() method on the testing dataset and a value of 0.139 is obtained.

The Lasso and Ridge regression models are then built using Lasso() and Ridge() methods respectively, with an alpha value of 50, maximum iterations of 100, and a tolerance of 0.1. These models are then trained on the training dataset using the .fit() method and the R-squared values are computed using the .score() method on the testing dataset. The Lasso regression model has a score of 0.664, while the Ridge regression model has a score of 0.667.
