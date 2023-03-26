Machine Learning Practice -- Day 10

The wine dataset is loaded using the load_wine() function from sklearn.datasets. The data is then stored in a Pandas dataframe using pd.DataFrame(). The columns of the dataframe are named using wine.feature_names. The target variable is added to the dataframe as a column named 'target'.

The dataset is then split into training and testing sets using the train_test_split() function from sklearn.model_selection. The test_size parameter is set to 0.2, which means that 20% of the data will be used for testing, and the remaining 80% will be used for training. The random_state parameter is set to 123 for reproducibility.

Two Naive Bayes models are trained on the training data: Gaussian Naive Bayes and Multinomial Naive Bayes.

The Gaussian Naive Bayes model is trained using the GaussianNB() function from sklearn.naive_bayes. The fit() method is used to fit the model on the training data, and the score() method is used to calculate the accuracy of the model on the testing data.

The Multinomial Naive Bayes model is trained using the MultinomialNB() function from sklearn.naive_bayes. The fit() method is used to fit the model on the training data, and the score() method is used to calculate the accuracy of the model on the testing data.
