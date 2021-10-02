# Retail-Sales-Prediction

<p align="center">
  <img width="460" height="300" src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b2/Ro%C3%9Fmann-Markt_in_Berlin.jpg/1024px-Ro%C3%9Fmann-Markt_in_Berlin.jpg">
</p>

Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied. My work includes various plots and graphs , visualizations , feature engineering , ensemble techniques , different ML algorithms with their respective parameter tuning , analysis and trends . Predictions are of 6 weeks of daily sales for 1,115 stores located across Germany.

In this project, the Kaggle Rossman challenge is being taken on. The goal is to predict the Sales of a given store on a given day. Model performance is evaluated on the root mean absolute percentage error (MAPE).


The dataset consists of two csv files: store.csv and train.csv

Data Files:

train.csv holds info about each store. store.csv holds the sales info per day for each store.

The repo contains main.py that runs the main script from step one until the end.


## 1. Business Problem.
Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.

## 2. Solution Strategy
My strategy to solve this challenge was:

Step 01: Data Description: Use statistics metrics to identify data distributions.

Step 02: Feature Engineering: Derive new attributes based on the original variables to better describe the phenomenon that will be modeled.

Step 03: Exploratory Data Analysis: Explore the data to find insights and better understand the impact of variables on model learning.

Step 04: Feature Selection: Selection of the most significant attributes for training the model.

Step 05: Machine Learning Modelling: Machine Learning model training.

Step 06: Hyperparameter Fine Tunning: hoose the best values for each of the parameters of the model selected from the previous step.

Step 07: Convert Model Performance to Business Values: Convert the performance of the Machine Learning model into a business result.



## 3.Machine Learning Model Implementation and performance
At this stage models used : *Linear Regression, *Lasso Regression, *Random Forest Regressor

	                                        Training score                Testing score 
			Linear Regression	0.780750		       0.782392
			
			Lasso Regression	0.780731		       0.782369
			
			Random Forest    	0.993811             	       0.956433





## 4. Conclusion

Acheived MAPE of 5.65% and MAE = $376 showing predictions of model is higly accurate for the sales forecast. Generated insights by EDA and feature importance provide valuable tools to decide the amount of budget and inventory for upcoming sales.
