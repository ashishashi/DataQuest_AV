
#DataQuest_AV

##Problem

Road transport in India is one of the most frequently used means of transport for a common man. Each year the number of vehicles on the road keeps increasing, but with that comes the risk of road-accidents and fatalities. In 2017 alone, almost 1.5 lakh people were killed in road accidents across the country.In this dataset, you have been provided with the details of road accidents in Dehradun District of Uttarakhand State.In particulr we ask you to apply machine learning tools to predict the criticality of the accident(0 or 1).The evaluation metric for this competition is AUC ROC score. 

We start by importing the dataset then by reading it.The dataset had columns named time and date which were converted to four variables(Feature Engineering) named day_of_week, month, year and time_category in order to extract out maximum possible information from these features.Further data-preprocessing was done followed by some data exploration.The dataset was highly imbalanced and so different techniques like Random OverSampling, UnderSampling, SMOTE were implemented in combination with different algorithms like XGboost and Decision tree and finally; there performance was compared to XGboost and Tree models without any sampling.SMOTE in combination with XGboost performed best but not really up to the mark.Finally; neural network was trained by altering the class_weights suitably to improve the AUC ROC score.With this as the final model; we as a team of 2 ended up at 19th position in the competition.

PYTHON As usual, we will first download our datasets locally, and then we will load them into data frames in both, python.The dataset has been uploaded alongwith the code file.In Python, we use pd.read_csv to read CSV files into pandas data.frame variables.

##Libraries used :

1)library(pandas) #to read .csv file

2)library(sklearn) #for train_test_split, LabelEncoder and evaluation metrics

3)library(matplotlib) #for data visualisation

4)library(xgboost) #for applying XGboost

5)library(imblearn) #for applying SMOTE, Oversampling and UnderSampling

6)library(sklearn.Tree) #for Decision Tree

7)library(e1071)#for SVM

8)library(keras) #for building neural network model and training
