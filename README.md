# IRIS-Dataset-Analysis

## Case Study : Data Analysis of IRIS Dataset (the most sought datasets for Classification Problems) using Linear Regression and K-Nearest-Neighbor Algorithms

## Data : 

Iris Dataset is one of the most sought datasets for classification problems. The dataset consists of 150 instances; 50 samples from each of three species of Iris (Iris setosa, Iris virginica and Iris versicolor). Four features were measured from each sample: the length and the width of the sepals and petals, in centimeters. Based on the combination and study of all these features in the sample, we were able to distinguish one species from another, by trying out the model using both KNN Algorithm and Logistic Regression. 

The dataset has attributes : features (sepal length, sepal width, petal length, petal width) and target (the three species apportioned into : setosa, virginica and versicolor).
The dataset has been taken from the built in dataset redily available in the sklearn library. But the csv form of the data set can be also found on kaggle or in .data format from <a href = 'https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'>https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data</a>


## Study and Methodology : 

The datasets were divided into input and target(output). The dataset was found out to be on Bunch datatype, hence the datasets were smootly divided into Data(consisting of 4 input columns: sepal length, sepal width, petal length, petal width) acting as the input for the model and target (having one output column) acting as the output. 
Then after the segregation , the data and the target were passed on to the model as different objects and were converted to numerical values(matrices) using NumPy. In the following step, the data was stored in X and the target in y, i.e the class was instantiated. Finally, we tried to fit the model on to the datasets and manually gave some input value in order to predict the accuracy rate or how well the model fitted for a particular algorithm. 
