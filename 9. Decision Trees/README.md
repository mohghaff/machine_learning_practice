Machine Learning Practice -- Day 8

This code uses the Titanic dataset, available as a CSV file at /content/titanic.csv, to build a classification model that predicts whether a passenger survived the sinking of the Titanic or not. The code performs data preprocessing and uses a Decision Tree classifier from Scikit-learn to train and test the model.

We encode the 'Sex' column as a numerical variable using the LabelEncoder class. Then, we use SimpleImputer to fill the missing values in the 'Age' column with the mean age. We apply isnull().sum() to check if there are still any missing values in the DataFrame.

After preprocessing the data, we split it into training and testing sets using train_test_split. We separate the features (i.e., all columns except 'Survived') into X, and the target variable (i.e., 'Survived') into y. We set the test size to be 0.2, which means 20% of the data will be used for testing, and we set a random seed to ensure reproducibility.
