# Titanic-Survival-Classification

## About Dataset:
The Titanic dataset is a widely used dataset that contains information on the passengers who were aboard the Titanic when it sank on its maiden voyage in 1912. The dataset includes features such as age, sex, passenger class, and fare paid, as well as whether or not the passenger survived the sinking. The dataset is often used for machine learning and data analysis tasks, such as predicting survival based on passenger characteristics or exploring patterns in the data.

## Column Description
- PassengerId: unique identifier for each passenger
- Survived: whether the passenger survived (1) or not (0)
- Pclass: passenger class (1 = 1st class, 2 = 2nd class, 3 = 3rd class)
- Name: name of the passenger
- Sex: gender of the passenger
- Age: age of the passenger (in years)
- SibSp: number of siblings or spouses aboard the Titanic
- Parch: number of parents or children aboard the Titanic
- Ticket: ticket number
- Fare: passenger fare
- Cabin: cabin number
- Embarked: port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

### Objective: 
To predict the survival of passenger from the Titanic ship, with the use of Machine Learning algorithms.

**I followed the following process to analyze the data and present it:**

## Step 1: Importing required libraries
Importing all the required basics data science libraries for processing the data. In this notebook, I have imported Numpy, Pandas for processing the data and matplotlib and seaborn for visualization.

## Step 2: Data Preprocessing
Importing the data using pandas library.

## Step 3: Analyzing the data
Before proceeding to Exploratory Data Analysis(EDA), I have analyzes the data by checking of missing values, shape of data, checking mean, median, maximum, minimum using _describe_ function.

## Step 4: Exploratory Data Analysis(EDA)
* The survival rate of titanic data is 38.4% of total data.
* More female has survived than male. Out of 314 females 233 survived and out of 577 males only 109 survived. The survival ratio of female is more than male.
* Economic Class affected Survival rate and Passengers travelling with First Class had higher ratio of survival about 63% as compared to Class 2 and 3.
* Most of the fare lies between 0-100 dollars. Passengers who paid more fare has higher chances of survival. Fare like 514 dollars was purchased by very few(Outliers).
* Most of the Passengers were travelling Solo and most of them died. Solo Females were more likely to Survive as compared to males.
* Fare and Survival has positive correlation.
* While exploring data, I found that there are missing values. The features of Age, Cabin and Embarked has 19%, 77% and 0.2% of missing values respectively. 
* From the _Name_ feature I found that most priority has given to females(Mrs).
* Filled the missing values for _Embarked_ i used mode to fill, for age I plotted the boxplot of pclass and age and found that people that are travelling pclass 1 tend to be richer and older(mean age is 37).

## Step 5: Converting Categorical features to Ordinal
I converted features Sex and Embarked into ordinal by using map function so that extra columns does not get added.

## Step 6: Dropping unwanted columns
PassengerId, Name, Cabin and Ticket I dropped from data as PassengerId was not provided any significant information and Cabin has more than 77% of missing values.

## Step 7: Standarising the data
Standarize the data using StandardScaler() around mean 0.

## Step 8: Train_test_split
Spliting the data into 67% training and 33% test data

## Step 9: Applying ML algorithms
In this python notebook, I have applied 7 ML classification algorithm on titanic
- Logistic Regression
- Decision Tree
- Random Forest
- SVM
- Gradient Boosting
- XGBoost
- LightGBM

## Step 10: Hyperparameter Tuning
After hypertuning the models, XGBoost gave 88.9% accuracy then Gradient Boosting 88.8%.





