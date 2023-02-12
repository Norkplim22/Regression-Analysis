## Regression-Project

# Introduction
Corporation Favorita is an Ecuador based organization involved in the setting up and administration of department stores and supermarkets. They deal in the retail of different family of products from food supplies to automotives and real estates. For this project I explored the sales data of different stores all around the country and got insights into the products and sales made on a daily over the course of 5 years. The goal is to use current sales data to predict future sales.

All analysis were conducted following the CRISP-DM framework.

# Data used.
train.csv

The training data, comprising time series of features (01–01–2013 to 15–08–2017), store_nbr, family, and on promotion as well as the target sales.
store_nbr identifies the store at which the products are sold.
family identifies the type of product sold.
sales give the total sales for a product family at a particular store at a given date. Fractional values are possible since products can be sold in fractional units (1.5 kg of cheese, for instance, as opposed to 1 bag of chips).
On promotion gives the total number of items in a product family that were being promoted at a store at a given date.

test.csv

The test data, having the same features as the training data. You will predict the target sales for the dates in this file.
The dates in the test data are for the 15 days after the last date in the training data (15–08–2017).

transaction.csv

Contains date, store_nbr and transaction made on that specific date.

stores.csv

Store metadata, including city, state, type, and cluster.
cluster is a grouping of similar stores.

oil.csv

Daily oil price which includes values during both the train and test data timeframes. (Ecuador is an oil-dependent country and its economic health is highly vulnerable to shocks in oil prices.)

holidays_events.csv

Holidays and Events, with metadata

# Insights from data analysis
The data was made of sales from 01-01-2013 to 31-08-2017
The primary data for the analysis is the train and test data. These dataset had no missing values.
The supplementary data:oil, store, holidays and transaction data were also important depending on the question of interest.

Hypothesis and Questions
Null hypothesis: Product sales are directly correlated with special events.

Alternate hypothesis: Product sales are independent of events.

Questions.

1. Which dates have the lowest and highest sales for each year and which year recorded many sales? Which time of year are most purchases made? 

2016 recorded the highest sales. Most purchases were made in the month of July and especially on Sundays. January first of every year recorded lower sales.

2. A magnitude 7.8 earthquake struck Ecuador on April 16, 2016. Did the earthquake impact sales?

The earthquake happened on April 16th, 2016. In the week of the earthquake (14th-21st April), sales increased highly compared to other week and peak on the day of the earthquake but began to plunge after the earththquake for almost two weeks before picking up again. To confirm the sales pattern was as a result of the earthquake and not just a general pattern during these two months, analysis of the other years is necessary for further insight. Insight from the other years revealed that the earthquake impacted sales.

3. Are certain groups of stores selling more products? (Cluster, city, state, type) and which family of products are the most purchased?

Yes, stores in the city of Quito and Pichincha state specifically in cluster 14 are selling more products than other stores.

4. Are sales affected by promotions, oil prices and holidays?

Sales are affected by promotions, seasons and events. Seasons like dry and rainy seasons, christmas season and also salary payments.

# Author
Linda Adzigbli


# Medium article
https://medium.com/@cnorkplim/time-series-regression-project-corporation-favorita-sales-prediction-5034936973b