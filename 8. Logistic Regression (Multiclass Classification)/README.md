Machine Learning Practice -- Day 7

Iris Dataset

The purpose of this code is to classify the iris dataset using logistic regression. The iris dataset is a commonly used dataset in machine learning and contains information about the sepal length, sepal width, petal length, and petal width of three different species of iris flowers (setosa, versicolor, and virginica).

The dataset is split into training and testing sets using the train_test_split function from sklearn.model_selection. The function takes the iris_data.data and iris_data.target as inputs, along with a test_size of 0.2, which means 20% of the data will be reserved for testing.

The accuracy of the model is then evaluated on the test data using the score method of the model object. A confusion matrix is then created using the confusion_matrix function from sklearn.metrics. The function takes in the actual labels y_test and predicted labels y_predicted as inputs.
