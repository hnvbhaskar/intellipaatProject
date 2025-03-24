







Capstone Project - II



Online Retail Store





Submitted By

HNV Bhaskar
Hyderabad
 
Table of Contents



1. 	Problem Statement
2. 	Project Objective
3. 	Data Description
4. 	Data Pre-processing Steps and Inspiration
5. 	Choosing the Algorithm for the Project
6. 	Motivation and Reasons For Choosing the Algorithm
7. 	Assumptions
8. 	Model Evaluation and Techniques
9. 	Inferences from the Same
10. 	Future Possibilities of the Project
 

Problem  Statement:
	An online retail store is trying to understand the various customer purchase patterns for their firm, you are required to give enough evidence-based insights to provide the same

Project Objective:
	The project objective is to identify the customer purchase patterns based in their recent, frequent, and the money they spent on visiting stores. 

Data Description:
	The dataset contains the following features and their corresponding description.
Feature Description
Invoice 	Invoice Number
Stock code	Product ID
Description	Product Description
Quantity	Quantity of the product
Invoice Date	Date of Purchase
Price 	Price of the Product per Unit
Customer ID	Customer ID
County	Region of the Purchase
	
	
 
Data Pre-processing Steps and Inspiration:
The pre-processing steps are:
	Checking the unique values present in each column.
	Checking the information of each column to check the missing values and data types present in the dataset.
	Checking the descriptive statistics of the dataset. 
	Nearly  24% values of CustomerID column are missing. So, I had dropped those values. There is “total amount”  column is missing, so we had multiplied the quantity and price to get the total amount for entire dataset.
	Checking the percentage of the purchase distribution of the dataset.
	Invoices generated from each country is depicted using the bar diagram and most of them are from UK.
	The total revenue of each country is also plotted.
	Most purchased items are plotted for each country with the stacked bar.

 
Choosing the Algorithm for this Project:
	The machine learning algorithm we chose for this project is Cluster analysis using K-Means. Apart from that, we chose RFM (Recency, Frequency, Monetary) analysis which is widely used business strategy in the corporate sector to identify the customer purchase patterns.


Motivation and Reasons for Choosing the Algorithm:

K-Means Algorithm:
✓ It is a simple centroid-based and commonly used clustering algorithms. This algorithm tries to minimize the variance of data points within a cluster. K-means is best used on smaller data sets because it iterates over all of the data points 
 RFM Analysis:
	RFM analysis is a marketing technique used to quantitatively rank and group customers based on the recency, frequency and monetary total of their recent transactions to identify the best customers and perform targeted marketing campaigns. 
RFM analysis ranks each customer on the following factors:
Recency:		How recent was the customer's last purchase? Customers who recently made a purchase will still have the product on their mind and are more likely to purchase or use the product again. Businesses often measure recency in days. But, depending on the product, they may measure it in years, weeks or even hours.

Frequency: 	How often did this customer make a purchase in a givenperiod? Customers who purchased once are often are more likely topurchase again. Additionally, first time customers may be good targetsfor follow-up advertising to convert them into more frequent customers.

Monetary: 	How much money did the customer spend in a given period? Customers who spend a lot of money are more likely to spend money in the future and have a high value to a business. 

Segmentation of customers in RFM analysis:
 	Customer segmentation, this process is used to produce targeted direct marketing campaigns tailored to specific customer types. It enables businesses to use email or direct mail marketing to target messages that a large swath of specific kinds of customers are more likely to respond to. This is based on the score of the customer score. Some examples of this type that are included in the analysis are:
	Lost Customer
	Customer Needed Attention
	Loyal Customer
	Champion
	Recent Customer
	Top Customer Needed Attention
	Top Recent Customer
	Top Loyal Customer
	Top Lost Customer
 
Assumptions:
	The Customer ID values are not imputed with mean or any other method. Because, they are the unique values, by altering which results in a huge variation in the dataset. So, we dropped them.
 
The outliers from the box plot after the RFM analysis, are removed.
 
Model Evaluation and Techniques:

The K-Means algorithm using the Elbow method, it has suggested to categorize the dataset into three. After implementing the analysis, the three different clusters have been categorized into lost customer, current customer, and best customer.RFM analysis is categorized into nine categories Lost, Customer Needed Attention, Loyal, Champion, Recent, Top Recent, Top Customer Needed Attention, Top Loyal, Top Lost
Inferences from the Same:
	From both (K-Means & RFM) analysis, we conclude that the retail store should be focus more on the Lost/Needed Attention customer. Best customers are also high compared to current customer, it provides an insight of maintaining the best service to the customers.

Future Possibilities of the Project:
	The store should take feedback on improving the customer satisfaction. Take necessary steps on improving the customer needs, inventory management, quality of products, and advertising may increase the sales of the stores

•  Data loading and exploration
•  Data cleaning and preprocessing
•  Exploratory data analysis (EDA)
•  Customer segmentation using RFM analysis
•  Pattern mining (e.g., association rules or frequent itemsets)
•  Predictive modeling (e.g., time series analysis or recommendation systems)
















Capstone Project-I



Forecasting of Sales Data of Wallmart





Submitted By

HNV Bhaskar
Hyderabad
 
Table of Contents
1. 	Problem Statement
2. 	Project Objective
3. 	Data Description
4. 	Data Pre-processing Steps and Inspiration
5. 	Choosing the Algorithm for the Project
6. 	Motivation and Reasons For Choosing the Algorithm
7. 	Assumptions
8. 	Model Evaluation and Techniques
9. 	Inferences from the Same
10. 	Future Possibilities of the Project
 

Problem Statement

A retail company is suffering to maintain its inventory to meet the dynamic requirement of the customer needs. The company is failing to supply the goods as per the demand on the hour of need.  It is also found difficult to maintain store wise inventory as the demand of the goods is different for each store.

Project Objective

The main objective of this project is to :-
	Understand the current / average sales of the goods 
	Understand the store wise sales 
	Determine the pattern of store wise sales 
	Forecast store wise demand for the upcoming quarter

Data Description

Dataset Description:-
We have following data set with regards to store wise sales data for the last one year.
Store	Date	Weekly Sales	Holiday Flag	Temperature	Fuel Price	CPI	Unemployment
Store/ location	Week of sale	Sales per given week per given store	Is holiday?	Temp of day of sale	Cost of fuel in the region	Consumer Price Index	Rate of Unemployment

 
Data Preprocessing Steps And Inspiration

Data Collection:-
Utilizing the given Wallmart dataset for 45 stores of 143 weeks of sales along with fuel price, temperature, number of holidays, CPI and unemployment details. This data is in raw and unorganized format with different data types.
Data Preparation
- Observed few dates of few stores is in text format. Converted all the dates into mm/dd/yyyy format.
- Identify the unique values present in each column
- Data types of each column must be analyzed and corrected (as done for date column)
- Identify the correlation of each column with other columns. There should be no positive or negative correlation between variables/ columns. 
- Segregation of entire dataset based on income across 45 stores. 
- Segregated the data as per below :-
	- Weekly sales summary across all 45 stores
	- Total 143 Weeks sales summary against each store
	- Store wise average values of Temperature, Fuel price, Holiday count and 	unemployment
Data input
The organized data, summary and average values would be the input to the algorithms to get the conclusion or predictions
Data Processing
Based on the initial processing and pictorial representation of the organized data, the following high level statements are made:-
	- Summary of sales is directly proportional to CPI and unemployment
	- Summary of sales is not symmetric and observed most ups and down based on 	various parameters
	- Summary of sales is not intermittently dependent on fuel price and temperature
 
Data Output and Interpretation
Conclusions of data processing points would be the outcome of data preparation


Data Analysis and Understanding
Data Formatting:-



 
Conclusion from Data Processing:-
- Categorize the data based on the weekly sales using cluster analysis
- predict the income of each store based on the analysis
- Forecasting of weekly sales using some time series machine learning models

 

Choosing the Algorithm For the Project

Identify a model: Various models are used for forecasting, depending on the data type, business context, and the level of complexity required. The most appropriate model for forecasting will depend on the data being analyzed, the business context, and the level of complexity required. In many cases, a combination of different models may be used to achieve the most accurate and reliable forecasts. Your model evaluation process should be well considered. Some commonly used models include:
	Time series forecasting models: Ideal for forecasting time series data like stock prices or sales data.
	Regression Analysis: 
	Exponential smoothing models: Effective for forecasting time series data, placing more weight on recent data.
	ARIMA models: Best for data that showcases complex patterns like seasonality or trends.

Motivation behind using the Algorithm:- Since we have the past history of the sales,  where the quantity of sales is dependent on other factors such as week, isHoliday  etc, regression is the best suitable process for finding the dependency between the variables. Sometimes we may need to use other models integrated with the regression techniques to get more accurate forecasting results.

K-Means Algorithm:	It is a simple centroid-based and commonly used clustering algorithms. This algorithm tries to minimize the variance of data points within a cluster. K-means is best used on smaller data sets because it iterates over all of the datapoints/
 
Hence, we have small dataset which needs to be studied based on the centroid to divide the dataset into different clusters, this algorithm is much more appropriate compared to other clustering algorithms.
 
Regression Machine Learning Algorithms:  	We choose the regression algorithms, because our target is to predict the weekly sales. I have chosen different regression machine learning algorithms to check which algorithm provides the best accuracy score and RMSE.
 
Forecast Analysis: 	Among the time series models that were present, the most suitable models are ARIMA and SARIMAX are used for the predictions of weekly sales. We used ARIMA model for the forecast of the weekly sales across different stories for next six months.

Auto Regressive Moving Average (ARIMA) Model:-

- visualize the time series data
- make the time series data stationary
- plot the correlation and auto correlation charts
- construct the ARIMA and seasonal ARIMA models
- use the model for predictions


Assumptions

The following assumptions are made for the sales forecast for the Wallmart store for the next 3 months:-

-  We take only 2-5 stores data instead of working on 45 stores as its assumed the category of the stores are same

- Each model would be fed with different scope of data

Model Evaluation and Technique

 
	The predictive analysis where the regression algorithms are used, the models were evaluated using the RMSE values and score of the used models. 

	The forecast analysis where ARIMA and SARIMAX are used, the models were evaluated using the RMSE value

Inferences from the Same:

	Firstly, we implemented the cluster analysis on the dataset using the K-Means algorithm, this helps to divide the cluster into three different cluster using the elbow method and silhouette score. The cluster analysis has clusters labelled as 0,1, and 2.The cluster groups are assigned to each store.

	This analysis shows that, the cluster “0” labelled stores have good weekly sales; whereas the cluster “1” stores has high weekly sales and the cluster “2” has relatively low weekly sales compared to other clusters. Later, we had plotted Monthly and Yearly sales with respect to each cluster id. From these plots, we observed that the sales are decreasing continuously for each cluster with increasing year. The sales are high in the month of November and December for each cluster. In the next step, we proceeded with the prediction of sales using the different regression algorithms. For this, we created a user-defined function with different algorithms along with the default parameters to predict the sales we have taken the example of selecting the store “1” to predict the income generated with different ML algorithms and got good regression score but the RMSE values are quite high. 

	In the final step, to forecast the sales we used the ARIMA and SARIMAX models. Initially, we all did the pre-processing steps for the time series analysis to check stationary using ADF fuller test and seasonal decompose, autocorrelation and partial-autocorrelation for the correlation. Later, we divide the dataset into the train and test, and using the ARIMA, SARIMAX models to train the data and predicting the sales using the test data. After this analysis, we forecasted the predictions using SARIMAX model for six years


Future Possibilities:-
The future possibilities that could include in the project is adding the location of each store, that helps to increase the sales. Customer feedback would also help to know the type of products that customers are interested to purchase and this would help us in doing another analysis of Recency, Frequency, Monetary (RFM).

