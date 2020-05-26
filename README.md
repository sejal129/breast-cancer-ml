# Introduction
Approximately 70% of data science problems involve classification and logistic regression is a common solution for binary problems. Logistic regression has many applications in data science, but in the world of healthcare, it can really drive life-changing action.
Detected breast cancer by applying a logistic regression model on a real-world dataset and predict whether a tumor is benign (not breast cancer) or malignant (breast cancer) based off its characteristics.

# Independent Variables
This is a logistic regression model to identify correlations between the following 9 independent variables and the class of the tumor (benign or malignant).
1. Clump thickness
2. Uniformity of cell size
3. Uniformity of cell shape
4. Marginal adhesion
5. Single epithelial cell
6. Bare Nuclei
7. Bland chromatin
8. Normal nucleoli
8. Mitoses

Logistic regression can identify important predictors of breast cancer using odds ratios and generate confidence intervals that provide additional information for decision-making. Model performance depends on the ability of the radiologists to accurately identify findings on mammograms.

# Overview

To read about different modules refer to the [scikit-learn](https://scikit-learn.org/stable/index.html) site.
### Part 1: Data Preprocessing
##### 1. Importing the dataset
Imported the pandas library to read the dataset. The given dataset is multivariate defined over 10 different attributes. Each attribute is an integer.

There are two class of the tumor: Benign (not breast cancer) represented as 2 or Malignant (breast cancer) represented as 4 based off its characteristics in the dataset.

##### 2. Splitting the dataset into a training set and test set
The dataset was splitted using the test_train_split function imported from model_selection.

Out of Approx. 700 instances, 20% were splitted into test set remaining 80% were kept to train the dataset called as X_train, y_train, X_test, y_test.
    
### Part 2: Training and Inference
##### 1. Training the logistic regression model on the training set
Trained the logistic regression model to fit on the splitted X_train and y_train dataset.

##### 2. Predicting the test results
The trained classifier was used to predict the values in test set.

### Part 3: Evaluating the model
##### 1. Making the confusion matrix
The confusion matrix was created to evaluate the model depicting the approx percentage of the correct predicted value comparing from the given tets values. 

##### 2. Computing the accuracy with k-fold cross-validation
Calculated the Accuracy (96.70% approx) and Standard Deviation (1.97%).
