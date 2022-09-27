# Rossman_store_sales_prediction

Rossman store sales prediction Project Description 
Business Problem 
Rossmann manages approximately 3,000 pharmacies in seven European nations. Currently, Rossmann shop managers must forecast their daily sales six weeks in advance. There are a number of variables that affect retail sales, including promotions, competition, school and state holidays, seasonality, and location. Due to the fact that hundreds of different managers anticipate sales based on their own circumstances, the accuracy of the findings might vary significantly.
Data Description
Src : https://www.kaggle.com/c/rossmann-store-sales/data 
The dataset is obtained from Kaggle and contains the following information:
1.	Id - an Id that represents a (Store, Date) duple within the test set 
2.	Store - a unique Id for each store 
3.	Sales - the turnover for any given day (this is what you are predicting) 
4.	Customers - the number of customers on a given day 
5.	Open - an indicator for whether the store was open: 0 = closed, 1 = open 
6.	StateHoliday - indicates a state holiday. Normally all stores, with few exceptions, are closed on state holidays. Note that all schools are closed on public holidays and weekends. a = public holiday, b = Easter holiday, c = Christmas, 0 = None 
7.	SchoolHoliday - indicates if the (Store, Date) was affected by the closure of public schools 
8.	StoreType - differentiates between 4 different store models: a, b, c, d 
9.	Assortment - describes an assortment level: a = basic, b = extra, c = extended 
10.	CompetitionDistance - distance in meters to the nearest competitor store 
11.	CompetitionOpenSince[Month/Year] - gives the approximate year and month of the time the nearest competitor was opened 
12.	Promo - indicates whether a store is running a promo on that day 
13.	Promo2 - Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating 
14.	Promo2Since[Year/Week] - describes the year and calendar week when the store started participating in Promo2 
15.	PromoInterval - describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store 
Project Objective 
The major objective of this initiative is to provide historical sales data for 1,115 Rossmann locations. In this project, the 'Sales' of Rossmann outlets will be estimated.
Project Approach 
1.	Exploratory Data Analysis: Exploratory data analysis is the process of analyzing a dataset in order to comprehend its properties. In this phase, the following will be determined.
a)	Identifying the number of unique users 
b)	Platforms used by the users the most 
c)	Correlations 
d)	Checking for null / inconsistent values and various other insights are drawn. 
2.	Imputation: This phase entails filling in missing values in a suitable manner so that data is not destroyed.
3.	Outliers Detection and removal: Outliers are points that are unusually separated from the rest of the data. These types of anomalies in the data are identified and deleted.
4.	Further Exploratory Data Analysis: Further EDA is conducted to get a deeper understanding of the data and identify a few unique situations.
5.	Label Encoding and One hot encoding: Machine learning algorithms for regression can only interpret input in the form of numbers; thus, it is necessary to label the non-numerical data I possess in order to convert it to numerical data.
6.	Model Building and evaluation: On the dataset, many regression techniques are performed, and the model that best fits the dataset is chosen. The models used to this data set are:
1.	Linear Regression 
2.	SGD Regression 
3.	Random Forest Regressor 
4.	Decision Tree Regressor 
7.	Feature Importance Analysis: Once the appropriate model has been chosen (which, in our instance, is the Random forest regressor since it provides the highest train and test accuracy), it is necessary to comprehend which characteristics contribute the most or least to the outcome.
Project development using VSCode
The ipython notebook is modularized into several functions, allowing the user easy access to those functions whenever they are needed. The folder for modularized code is structured as stated below.
Once you unzip the modular_code.zip file you can find the following folders within it. 
1.	Input: The input directory includes all of the data available for analysis. In our scenario, the folder will include three CSV files: a). store.csv, b). test.csv, c). train.csv 
2.	Src: The src folder contains the project's source code. This folder includes the modularized code for each of the preceding phases. The following is also included:
1.	ML_pipeline: The ML pipeline is a folder that includes all the suitably designated Python files containing the functions.
2.	engine.py: These Python routines are then invoked inside the engine.py file
3.	output: The output folder includes all.pkl files representing the trained models for this data. These models may be simply imported and used in the future; the user is not required to train all models from scratch.
4.	Lib: The lib directory is a reference directory. It includes the ipython notebook from the videos.
 
Project Takeaways 
1.	Understanding the problem statement 
2.	Data exploration 
3.	Data Visualization 
4.	Handling missing values 
5.	Handling Outliers 
6.	Exploring exceptional cases 
7.	Converting categorical to numeric forms 
8.	Creating heatmaps 
9.	Feature selection & its importance 
10.	Implementation using linear regression 
11.	Implementation using stochastic gradient descent 
12.	Implementation using random forest 
13.	Implementation using decision trees 
14.	Understanding feature importance 

