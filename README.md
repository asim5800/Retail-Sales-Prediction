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
<table>
<tr>
<th>Regression_Model</th>
<th>Train_MSE</th>
<th>Train_RMSE</th>
<th>Train_R2</th>
<th>Train_Adjusted_R2</th>
<th>Test_MSE</th>
<th>Test_RMSE</th>
<th>Test_R2</th>
<th>Test_Adjusted_R2</th>
</tr>
<tr>
    <td>Linear Regression</td>								
    <td>1.214859e+06</td>
    <td>1102.206527</td>
    <td>0.844978</td>
    <td>0.844975</td>
    <td>1.217627e+06</td>
    <td>1103.461202</td>
    <td>0.844943</td>
    <td>0.844929</td>
</tr>
<tr>
    <td>Lasso Regression</td>								
    <td>1.214485e+06</td>
    <td>1102.036953</td>
    <td>0.845026</td>
    <td>0.845012</td>
    <td>1.217348e+06</td>
    <td>1103.334986</td>
    <td>0.844979</td>
    <td>0.84496</td>
  </tr>
<tr>
    <td>Ridge Regression</td>
    <td>1.214486e+06</td>
    <td>1102.037084</td>
    <td>0.845026</td>
    <td>0.845022</td>
    <td>1.217348e+06</td>
    <td>1103.335147</td>
    <td>0.844979</td>
    <td>0.844965</td>
  </tr>
<tr>
    <td>Elastic Net Regression</td>								
    <td>1.214485e+06</td>
    <td>1102.036949</td>
    <td>0.845026</td>
    <td>0.845022</td>
    <td>1.217348e+06</td>
    <td>1103.334982</td>
    <td>0.844979</td>
    <td>0.844965</td>
  </tr>
<tr>								
    <td>Decsion Tree Regression</td>
    <td>1.362364e+06</td>
    <td>1167.203328</td>
    <td>0.826156</td>
    <td>0.826152</td>
    <td>1.367349e+06</td>
    <td>1169.337164</td>
    <td>0.825877</td>
    <td>0.825861</td>
  </tr>
<tr>
    <td>Random Forest Regression</td>								
    <td>5.596015e+04</td>
    <td>236.558981</td>
    <td>0.992859</td>
    <td>0.992859</td>
    <td>3.200686e+05</td>
    <td>565.746016</td>
    <td>0.959241</td>
    <td>0.959238</td>
  </tr>
</table>



## 4. Conclusion

Acheived MAPE of 5.65% and MAE = $376 showing predictions of model is higly accurate for the sales forecast. Generated insights by EDA and feature importance provide valuable tools to decide the amount of budget and inventory for upcoming sales.
