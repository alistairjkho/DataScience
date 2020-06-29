# Support Vector Machine

Support Vector Machines is a classification technique that finds a 'hyperplane' or a boundary between the two classes of data that maximizes the margin between the two classes. 

There are many planes that can separate the two classes, but only one plane can maximize the margin or distance between the classes.

* Pros: accurate in high dimensionality
* Cons: prone to over-fitting, does not directly provide probability estimates

<img src = https://miro.medium.com/max/809/1*GPFxwsE4cqcPxul4GWGp1A.png>

## Hyperplanes

* A straight line to divide data
* A line is created by computing the equal distance between points
* The best hyperplane is ones with a big **MARGIN** and largest distance between points, a.k.a support vectors
* This is to maximise the empty space so we can sepearte the two classes and do more accurate predictions
* There also exists soft margins, another parameter that allows some outliers to sit in-between the hyperplane
* This may make soft margins more accurate in certain cases
* Hard margins reject the outliers within the hyperplane

## Problems with SVMs
* If data is not properly segmented, difficult to create hyperplanes
* Problems can be fixed by using **KERNELS** - basically a function
* A function that takes the existing dimensions and returned a new dimension
* Kernels can bring the data into 3 dimensions

<img src = https://miro.medium.com/max/1400/1*3t_Gn5yuirT6fSC-sbxKAA.png width=500>

* There may different types of kernels

For further information see: [Medium Article](https://medium.com/@zachary.bedell/support-vector-machines-explained-73f4ec363f13)

# Folder Contents

In python notebook in this folder investigates certain features of a dataset to determine if the SVM machine learning model can determine malignant or benign breast cancer. The content is based on [Tech with Tim's YouTube Channel](https://www.youtube.com/watch?v=45ryDIPHdGg). The notebook will cover:

* Importing data
* Fitting the data into the model
* Changing the types of kernels and comparing them to improve scoring
* Predicting and validating the data
* Comparison with K-Nearest Neighbours machine learning algorithm
