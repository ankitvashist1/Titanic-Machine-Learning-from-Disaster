# Titanic: Machine Learning from Disaster

## Introduction
This project is aimed to train a prediciton model to predict survival on the titanic. We are given features corresponding to every passenger (like Age, Gender, Sex etc.) and using these features we are supposed to calculate whether a person survived from Titanic mishap or not.

## Data Sets
- Source: [Kaggle](https://www.kaggle.com/c/titanic/overview)
- Size of the train data is 891*12
- Size of the test data is 418*11

***Description of Data Variables:***
**Train Data:**
| Variable | Definition |	         Key                       |
| -------- | ---------- | ---------------------------------- |
| PassengerId| Id of passenger|
| Survived | Survival	  |          0 = No, 1 = Yes           |
|Name| Name of the passenger|
| pclass	 | Ticket class|	           1 = 1st, 2 = 2nd, 3 = 3rd|
|sex|	      Sex	|
|Age|	      Age in years	|
|sibsp|# of siblings / spouses aboard the Titanic	|
|parch|# of parents / children aboard the Titanic	|
|ticket|	  Ticket number	|
|fare|	    Passenger fare	|
|cabin	|    Cabin number	|
|embarked	|Port of Embarkation|C = Cherbourg, Q = Queenstown, S = Southampton|

## Research Problems
***Problems we want to solve:***
We want to predict whether a person with certain features has survived the titanic mishap or not.
We will be using Classification model since our label is Nominal. We will use Logistic Regression, SVM, KNN, Decision Trees and Naive Bayes models.
- Data Cleaning (will need to take care of noisy data and missing values)
- Data Transformation (since our features possess nominal features hence, we will have to first
convert them into Numerical variables)
- Data Reduction (we need to check for features which are not at all important for our prediction
and remove them)

## Potential Solutions
To build prediction models, we need to go for required preprocessing as per the model:
1. Data Cleaning: We need to take care of the noisy data and missing values. For missing values
in Nominal features, we can use below mentioned techniques:
- Use the most frequent value to fill in missing values of that attribute
- Use the most frequent value belonging to the same class to fill in the missing values
- Build a prediction model (Classification – in case of Nominal feature) to predict missing values
(if the feature is extremely important).
2. Data Transformation: Since our features possess nominal features hence, we will need to
convert them into numerical variables.
3. Data Reduction: We need to take care of the unnecessary columns in the data set which have
very less correlation with the label and eventually drop them.
There will be various other issues while creating our prediction models. For example,
corresponding to every prediction model we need to incorporate different preprocessing
techniques. Naïve Bayes will consider Nominal values whereas KNN will consider Numerical
features, hence corresponding to every model, we need to do preprocessing and finally create
prediction model.

## Evaluations
We will use Accuracy metric for our Evaluation purpose.

## Expected Outcomes
Expectedly, we will build a model which will predict whether the passenger has survived or not.
