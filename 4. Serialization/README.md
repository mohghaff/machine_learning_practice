Machine Learning Practice -- Day 3

This notebook provides a simple demonstration of building and saving a linear regression model using scikit-learn and the pickle and joblib modules. It also shows how to make predictions on new data using the saved model.

Serializing the Model

We use the pickle module to serialize the trained model into a file named model_pickle. We use the open() function with the mode 'wb' (write binary) to create a file object and the dump() method from the pickle module to write the trained model object to the file object.

We can then deserialize the saved model from the file object using the pickle.load() method. In the example, we load the saved model from the file object myFile and predict the price of a house with 2600 square footage, 3 bedrooms, and 20 years of age.

We also serialize the trained model using the joblib module and save it to a file named model_joblib. We can then load the saved model using the joblib.load() method and make predictions on new data. In the example, we predict the price of a house with 2600 square footage, 3 bedrooms, and 2 years of age using the loaded mj model object.
