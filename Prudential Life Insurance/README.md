**Problem Statement:** 

The project aims to develop a predictive model that can classify risk levels using data points in the existing life insurance assessment.

 

**Dataset Overview:**

In the dataset, there are 128 columns which consists of 60 categorical features, 13 numerical features, 5 discrete features and 48 dummy variables. The target is an ordinal measure of risks with 8 levels relating to final decision associated with the applicant. 

 

**Data Exploration:**

**Checking for null values:** 

Few columns in the dataset consisted of null values. For example, some columns that have null values are Employment_Info_1, Employment_Info_4. Total there are 13 columns which are having NULL values.

**Outliers:**

![outliers](https://user-images.githubusercontent.com/61173652/80275212-7a9a4580-86fd-11ea-9a99-5a789a989dc0.png)

From the above box plot, we can clearly visualize that the numerical features such as Ht, Wt, BMI consist of Outliers. Outliers are nothing but extreme values that deviate from other observations on data.

 

 

 

**Distribution of rows by Response variable:**

![response](https://user-images.githubusercontent.com/61173652/80275265-c5b45880-86fd-11ea-819c-8f672f838559.png)

Grouping the low risk associated with life insurance policy into one class. Now the response variables have 4 classes of risk.

 

 

![grouping_response](https://user-images.githubusercontent.com/61173652/80275280-d95fbf00-86fd-11ea-990f-88acd1116092.png)

 

 

 

 

**Treating Outliers:**

IQR score to filter out the outliers by keeping only valid values.

![treating_outliers](https://user-images.githubusercontent.com/61173652/80275288-e67cae00-86fd-11ea-91f7-32ae493a768d.png)

 

**Feature Selection and Encoding Features:**

Analyzing the dataset, we found that there are many categorical columns. To handle categorical columns, we are using Pandas get dummies encoding technique.It is a one step procedure to get the dummy variables for categorical features.

Dropping the columns which are irrelevant or does not contribute towards the target variable. For example Medical_History_10 feature is having more number of null values. Also ID feature we have dropped.

**Building Models:**

Splitting the dataset into 80% training set and 20% testing set. Finally we developed different Classification models. From all the classification models, RandomForest performs the best. It gave an accuracy around 64.61%. 

![final_result](https://user-images.githubusercontent.com/61173652/80275295-f3999d00-86fd-11ea-940f-b3b147a445b3.png)

 

 

 

 

 

 

 

 
