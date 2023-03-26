Machine Learning Practice -- Day 13

KNN is a type of supervised machine learning algorithm which can be used for both regression and classification problems. It is a non-parametric algorithm that uses the entire dataset to classify new data points based on their similarity to the training set. In this documentation, we will be using KNN to classify handwritten digits from the digits dataset.

Dataset:
The digits dataset is a preloaded dataset in Scikit-learn that consists of 1797 8x8 images of digits, where each pixel is represented as an integer from 0 to 16.

Step 1: Importing Required Libraries
We begin by importing the necessary libraries. In this case, we need NumPy, Scikit-learn, Matplotlib and Seaborn libraries.

Step 2: Loading the Dataset
We load the digits dataset using the load_digits function provided by Scikit-learn. Then, we split the dataset into training and testing sets using the train_test_split function with a test size of 0.2.

Step 3: Creating the KNN Model
We create a KNN model with 5 neighbors using the KNeighborsClassifier function from Scikit-learn. Then we fit the model to the training data using the fit() method. We also calculate the accuracy score of the model on the test data using the score() method.

Step 4: Testing the KNN Model with Different Values of K
We create multiple KNN models with different numbers of neighbors using a for loop. We store each model’s accuracy score and print it out along with the number of neighbors used.

Step 5: Evaluating the Model’s Performance
We make predictions on the test set using the model and store the results in y_pred. Then we create a confusion matrix using the confusion_matrix function provided by Scikit-learn. Finally, we visualize the confusion matrix using a heatmap using Matplotlib and Seaborn libraries.
