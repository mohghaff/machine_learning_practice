Machine Learning Practice -- Day 6

The code is performing a logistic regression classification task on HR data. The dataset contains information about employees such as their satisfaction level, last evaluation, number of projects, average monthly hours, time spent in the company, work accidents, department, salary, and whether or not they left the company. The objective is to build a model that predicts whether an employee is likely to leave the company based on the given features.

Encoding categorical data
The categorical data columns in the dataset, department and salary, are encoded using the LabelEncoder() function. The encoded data is stored in a new DataFrame named encoded_df.

One-hot encoding
The department column contains categorical data with more than two categories, which is not suitable for label encoding. Therefore, one-hot encoding is performed using the ColumnTransformer() and OneHotEncoder() functions. The encoded data is stored in the X variable, which contains all the features except the target variable (left).

Splitting the dataset
The dataset is split into training and testing sets using the train_test_split() function from the sklearn.model_selection library. The X_train, X_test, y_train, and y_test variables are used to store the training and testing sets.

Scaling the data
The data is then scaled using the MaxAbsScaler() function from the sklearn.preprocessing library. The scaled training and testing sets are stored in the X_train and X_test variables, respectively.

Making predictions
The predict() function is used to make predictions on the testing data, and the predicted values are stored in an array.

Evaluating the model
Finally, the score() function is used to evaluate the model's performance on the testing data. The score is displayed, which represents the accuracy of the model.
