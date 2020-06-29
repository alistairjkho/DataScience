# K-Nearest Neighbours

KNN is a model that classifies data points based on the points that are most similar to it. It uses test data to make an “educated guess” on what an unclassified point should be classified as.

KNN is an algorithm that is considered both non-parametric and an example of lazy learning. What do these two terms mean exactly?

* Non-parametric means that it makes no assumptions. The model is made up entirely from the data given to it rather than assuming its structure is normal.
* Lazy learning means that the algorithm makes no generalizations. This means that there is little training involved when using this method. Because of this, all of the training data is also used in testing when using KNN.

<img src = https://cambridgecoding.files.wordpress.com/2016/01/knn2.jpg width=500>

### Pros

* This algorithm is one of the more simple techniques used in machine learning - Easy to use
* Quick calculation time
* Does not make any assumptions about the data (e.g. normal distribution)

### Cons

* Accuracy depends on the quality of the data
* Must find an optimal k value (number of nearest neighbours)
* Poor at classifying data points in a boundary where they can be classified one way or another (ambiguity)
* KNN is very time consuming to model each time as it has to compute the distance between neighbouring points for each point
* Difficult to save it as a model as it has to save the training data for each cluster 
* Useless to train beforehand because it constantly has to keep looking at every data point before it can make a prediction

For more detailed information on KNN, visit: https://medium.com/capital-one-tech/k-nearest-neighbors-knn-algorithm-for-machine-learning-e883219c8f26

# Folder contents

The python notebook in this folder contains a dataset from https://archive.ics.uci.edu/ml/datasets.php, which looks at a car evaluation dataset to determine which attributes affect the quality/class of the vehicle. (classification problem). The notebook will cover:

* Importing the dataset
* Dealing with irregular data - encoding
* Fitting the KNN model
* Hypertuning of the model to find the best hyperparameter (K)
* Using GridSearch CV for model tuning
* Validation of the model
