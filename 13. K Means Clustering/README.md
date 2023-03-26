Machine Learning Practice -- Day 9

This code demonstrates how to perform k-means clustering on the Iris dataset using the Scikit-Learn library. K-means is an unsupervised machine learning algorithm used to group data points into a specific number of clusters. In this example, the two variables, "pedal_length" and "pedal_width" were used to cluster the Iris dataset into three clusters. The code also includes visualizations of the resulting clusters and an elbow plot to help determine the optimal number of clusters.

Data preprocessing
In this section, the "sepal_length" and "sepal_width" columns are dropped from the DataFrame since we only want to use the "pedal_length" and "pedal_width" variables for clustering. The column names are then changed to "pedal_length" and "pedal_width" for convenience. The data is then scaled using the MinMaxScaler from Scikit-Learn to ensure that the "pedal_length" and "pedal_width" variables are on the same scale.

K-means clustering

In this section, the KMeans function from Scikit-Learn is used to perform k-means clustering on the "pedal_length" and "pedal_width" variables. The number of clusters is set to 3. The resulting clusters are then added to the DataFrame under the "cluster" column.

Visualization

In this section, the resulting clusters are visualized using Matplotlib. The scatter function is used to plot the "pedal_length" and "pedal_width" variables for each cluster.

Finally, the "elbow method" was used to determine the optimal number of clusters for KMeans clustering algorithm. The elbow method is a heuristic used in cluster analysis to determine the appropriate number of clusters to include in the model. The method involves running KMeans clustering algorithm multiple times with different number of clusters, and plotting the resulting sum of squared errors (SSE) against the number of clusters
