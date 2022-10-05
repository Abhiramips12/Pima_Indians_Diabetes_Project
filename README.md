# Pima Indians Diabetes Project
------------------------------
### Input Dataset
=====================

https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

Dataset details
=============================

1: Pregnancies: Number of times pregnant

2: Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test.

3: BloodPressure: Diastolic blood pressure (mm Hg)

4: SkinThickness: Triceps skinfold thickness (mm)

5: Insulin: 2-Hour serum insulin (mu U/ml)

6: BMI: Body mass index (weight in kg/(height in m)²)

7: DiabetesPedigreeFunction: Diabetes pedigree function

8: Age: Age (years)

9: Outcome: Class variable (0 or 1) 268 of 768 are 1, the others are 0


Description:

We predict whether a patient had diabetes


Introduction:

Diabetes is a chronic disease or group of metabolic disease where a person suffers from a extended

level of blood glucose in the body.

The objective of the dataset is to diagnostically predict whether or not a  patient has

diabetes,based on certain diagnostic measurements included in the dataset.

The datasets consist of several independent variable and one dependent variable.ie ,the

dependent variable is the outcome.Independent variables include the the number of pregnancies the

Patient has had,their BMI,insulin level,Blood Pressure,Glucose,Skin Thickness,Age.It is a classification

type dataset.


Attribute Information:

1: Pregnancies: Number of times pregnant

2: Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test.

3: BloodPressure: Diastolic blood pressure (mm Hg)

4: SkinThickness: Triceps skinfold thickness (mm)

5: Insulin: 2-Hour serum insulin (mu U/ml)

6: BMI: Body mass index (weight in kg/(height in m)²)

7: DiabetesPedigreeFunction: Diabetes pedigree function

8: Age: Age (years)

9: Outcome: Class variable (0 or 1) 268 of 768 are 1, the others are 0


Import the required libraries such as Numpy, Pandas, Sklearn, Matplotlib.

Then load the dataset. Dataset contains 450 rows and 9 columns.

Then do the data preprocessing.ie,EDA,Feature Engineering,Feature Selection.


In EDA(Exploratory Data Analysis),Analyse the Target Variable(Outcome) and Check the unique

values,value counts and correlation in target variable and also plot it.

First analyse the target variable ie outcome,and is found as an imbalanced dataset.

Then,checking the basic information about the dataset such as shape,basic info,describe etc and

checked for missing values.

Then correlation between target variable is found and is plotted as heatmap.

Then,Pair Plot is plotted

Then we found that there are missing values.Since certain variable in the dataset cannot be

zero,the zeros in the dataset are treated as nothing but missing values.And are printed using for loop.

Then we do the missing value treatment and the method adopted is ,Replacing with Median.

Then outlier treatment and here we use the technique is Outlier detection with Standard Deviation.

Splitting the dataset in to train and test sets.70% of the dataset is used for training and 30% for

testing.

Then Scaling Down

Scaled down the dataset using the StandardScaler

Train using fit_transform and Test using transform

Created a pickle file "scale.pkl" for scaling process using joblib.

Data Modelling

Here we apply the classification algorithms such as Logistic Regression,Decision Tree

Classifier,AdaBoostClassifier,Gradient Boosting,Random Forest,SVC and Voiting Classifier.

Checking train vs test accuracy scores.

Hyperparameter Tuning

It is done in all algorithms to find the best model,and the accuracy & best parameters are printed out.

From the output ,Random Forest Classifier found to be performing the best on the basis of accuracy

value.

Web FrameWork

I have used Flask for setting the backend API

The UI is set using HTML code.

And i have done the project in my local system and after push all the files to Github.Then deploy

the app using Heroku.
