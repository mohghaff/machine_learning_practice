Machine Learning Practice -- Day 4

This notebook demonstrates how to use scikit-learn to perform a linear regression on a dataset containing categorical and numerical features. Specifically, it demonstrates how to use LabelEncoder, OneHotEncoder, ColumnTransformer, and LinearRegression classes from scikit-learn to preprocess the data and train a linear regression model.

Data Preprocessing
The code reads in a dataframe df, which contains a column 'Car Model' with categorical variables. The code uses pandas get_dummies function to one-hot encode the 'Car Model' column and then merges the resulting dummy variables with the original dataframe.

Label Encoding
The code uses LabelEncoder from scikit-learn to encode the categorical variable 'Car Model' into numerical values.

One-Hot Encoding
The code uses ColumnTransformer and OneHotEncoder from scikit-learn to perform one-hot encoding on the first column of x ('Car Model').
