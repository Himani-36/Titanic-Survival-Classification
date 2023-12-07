# Titanic-Survival-Classification

## About Dataset:
The Titanic dataset is a widely used dataset that contains information on the passengers who were aboard the Titanic when it sank on its maiden voyage in 1912. The dataset includes features such as age, sex, passenger class, and fare paid, as well as whether or not the passenger survived the sinking. The dataset is often used for machine learning and data analysis tasks, such as predicting survival based on passenger characteristics or exploring patterns in the data.

## Column Description
PassengerId: unique identifier for each passenger
Survived: whether the passenger survived (1) or not (0)
Pclass: passenger class (1 = 1st class, 2 = 2nd class, 3 = 3rd class)
Name: name of the passenger
Sex: gender of the passenger
Age: age of the passenger (in years)
SibSp: number of siblings or spouses aboard the Titanic
Parch: number of parents or children aboard the Titanic
Ticket: ticket number
Fare: passenger fare
Cabin: cabin number
Embarked: port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

**Objective**: To predict the survival of passenger from the Titanic ship, with the use of Machine Learning algorithms.

**I followed the following process to analyze the data and present it:**

**Step 1: Importing required libraries**
Importing all the required basics data science libraries for processing the data. In this notebook, I have imported Numpy, Pandas for processing the data and matplotlib and seaborn for visualization.

**Step 2: Data Preprocessing**
Importing the data using pandas library.

**Step 3: Analyzing the data**
Before proceeding to Exploratory Data Analysis(EDA), I have analyzes the data by checking of missing values, shape of data, checking mean, median, maximum, minimum using _describe_ function.

**Step 4: Exploratory Data Analysis**
* While exploring data, I found that there are missing values. The features of Age, Cabin and Embarked has 19%, 77% and 0.2% of missing values respectively. 
* From the _Name_ feature I found that most priority has given to females(Mrs)








