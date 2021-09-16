# IRIS-Dataset-Analysis

## Case Study : Data Analysis of IRIS Dataset (the most sought datasets for Classification Problems) using Linear Regression and K-Nearest-Neighbor Algorithms

## Data : 

Iris Dataset is one of the most sought datasets for classification problems. The dataset consists of 150 instances; 50 samples from each of three species of Iris (Iris setosa, Iris virginica and Iris versicolor). Four features were measured from each sample: the length and the width of the sepals and petals, in centimeters. Based on the combination and study of all these features in the sample, we were able to distinguish one species from another, by trying out the model using both KNN Algorithm and Logistic Regression. 

The dataset has attributes : features (sepal length, sepal width, petal length, petal width) and target (the three species apportioned into : setosa, virginica and versicolor).
The dataset has been taken from the built in dataset redily available in the sklearn library. But the csv form of the data set can be also found on kaggle or in .data format from <a href = 'https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'>https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data</a>


## Study and Methodology : 

The datasets were divided into input and target(output). The dataset was found out to be of Bunch datatype, hence the datasets were smootly divided into Data(consisting of 4 input columns: sepal length, sepal width, petal length, petal width) acting as the input for the model and target (having one output column) acting as the output. 
Then after the segregation , the data and the target were passed on to the model as different objects and were converted to numerical values(matrices) using NumPy. In the following step, the data was stored in X and the target in y, i.e the class was instantiated. Finally, we tried to fit the model on to the datasets and manually gave some input value in order to predict the accuracy rate or how well the model fitted for a particular algorithm. 


## Training and Testing :

### Manually Testing And Training :

Initially we tried to perform the traning and testing manually, by manually giving out the percentage of train and test datasets (in our case : we used 70% of dataset for training and the rest for testing). 

We tranied and tested the datasets for different values of k in a KNN algorithm and also for Logistic Regression and found out differences in their accuracy levels. The accuracy level also varied when the test size and the random state of the algorithm vaired. 

### Using K Fold Cross Validation :

Normally to improve our model accuracy, we would want to have maximum of train and test data points. But that's not possible in a normal test-train split because any one of them(train or test) must be less than the other. For every point we add in a test dataset, we lose a point from the train dataset.<br> 
So in order to resolve this trade off problem we used K Fold Cross Validation technique to train and test our model. This technique follows the procedure of dividing the dataset into k bins and literally iterating and trying out different permutations and combinations for both train and test data so that the model fits accurately. 

## Conclusion :

From our study we found out that :

●  The K fold Cross Validation can be the best technique to implement for traning and testing our model compared to the Normal train-test-split technique <br>
●  Under the  K fold Cross Validation technique logistic regression has a better accuracy rate that any value of k for KNN.<br>
●  Accuracy of the model is dependent on value of k in KNN, type of Algorithm, the test/train size and the random state.
