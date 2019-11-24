# Sparkify
Udacity Datascience Nano Degree Capstone Project

This project is to predict if Sparkify users are likely to cansel their subscriptions. The code was developed with Jupyter Notebook on the Spark framework running on an IBM cluster. And the process is data exploring, data engineering and model building.

## Motivation
Based on Sparkify data, we can see users' behavior. The purpose is to use these event data to develop an accurate machine learning model predicting whether a "Sparkify" user is likely to churn.

## Blog Post
The full discussion of my project and code are in this blog post.

## What's Inside
Sparkify_local.ipynb: original Jupyter Notebook code running on local machine with a small subset of the whole dataset. It's used to explore and clean data and try some feature engineering before using IBM working on the large data set.  
Sparkify_local.html: the html type of Sparkify_local.ipynb.  

Sparkify_cloud.ipynb: original Jupyter Notebook code running on IBM cluster. Data exploring part were done in local machine. In addition, this code splits the total dataset into train and test data; train machine learning models; choose and tune models and evaluate accuracy.  
Sparkify_cloud.html: the html type of Sparkify_cloud.ipynb.  

## Credits
I relied on two main references during this project:  
https://spark.apache.org/docs/2.1.1/ml-classification-regression.html   
https://medium.com/@kennyflutes/using-apache-spark-to-predict-user-churn-c4a50a2520e8  

## Libraries Used
pyspark.sql.SparkSession  
pyspark.sql.functions  
pyspark.sql.types  
pyspark.ml.feature: VectorAssembler, StandardScaler  
pyspark.ml.classification.LogisticRegression, GBTClassifier 
pyspark.ml.evaluation.MulticlassClassificationEvaluator 
pyspark.ml.tuning.CrossValidator, ParamGridBuilder 
pandas  
numpy 
matplotlib 
