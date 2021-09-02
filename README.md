#   Cryptocurrencies-Analysis

## Overview of Project
Accountability Accounting is an investment bank. They want to discover trends in new Cryptocurrencies to invest in the most profitable ones.
The company is interested in offering a new Cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. 
Martha is a senior manager for the Advisory Services Team at Accountability Accounting. The objective of this project is to assist Martha in creating a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.
The data Martha will be working with is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she has decided to use unsupervised learning. To group the cryptocurrencies, Martha decided on a clustering algorithm. She’ll use data visualizations to share her findings with the board.

## Purpose

The required input credit card credit dataset is available in a Comma Separated Values (CSV) file

The purpose of this project is to provide the below deliverables:

Deliverable 1: Preprocessing the Data for PCA
Deliverable 2: Reducing Data Dimensions Using PCA
Deliverable 3: Clustering Cryptocurrencies Using K-means
Deliverable 4: Visualizing Cryptocurrencies Results

## Results

## Preprocessing the Data for PCA

Deliverable 1: Preprocessing the Data for PCA

There are a number of steps taken to preprocess the data.

They are listed below:

1. Keep all the cryptocurrencies that are being traded

![Screen Shot 2021-09-02 at 2.35.45 AM](https://i.imgur.com/1LhNlud.png)


2. Keep all the cryptocurrencies that have a working "algorithm"

![Screen Shot 2021-09-02 at 2.36.27 AM](https://i.imgur.com/dVPgXwx.png)


3. Remove the "IsTrading" column

![Screen Shot 2021-09-02 at 2.37.16 AM](https://i.imgur.com/7ppuwso.png)


4. Remove rows that have at least 1 null value

![Screen Shot 2021-09-02 at 2.46.48 AM](https://i.imgur.com/ZovD3lH.png)


5. Keep the rows where coins are mined

![Screen Shot 2021-09-02 at 2.47.22 AM](https://i.imgur.com/XzETBor.png)


6. Create a new DataFrame that holds only the cryptocurrencies names

![Screen Shot 2021-09-02 at 2.48.00 AM](https://i.imgur.com/q2c3CS9.png)


7. Drop the 'CoinName' column since it's not going to be used on the clustering algorithm

![Screen Shot 2021-09-02 at 2.48.55 AM](https://i.imgur.com/9BBUmQR.png)


8. Use get_dummies() to create variables for text features


![Screen Shot 2021-09-02 at 2.49.46 AM](https://i.imgur.com/GG2Fl9B.png)

The above screenshot shows the dataset which has been executed through all the preprocessing steps.
There are 532 cryptocurrencies which have remained after the preprocessing steps.


## Reducing Data Dimensions Using PCA

Deliverable 2: Reducing Data Dimensions Using PCA

Before applying the PCA, Standardize the data with StandardScaler()

![Screen Shot 2021-09-02 at 3.11.28 AM](https://i.imgur.com/yYfmS1W.png)


Using PCA to reduce dimension to three principal components

![Screen Shot 2021-09-02 at 3.12.10 AM](https://i.imgur.com/vDB5ZbM.png)

Create a DataFrame with the three principal components.

![Screen Shot 2021-09-02 at 3.12.51 AM](https://i.imgur.com/ts50Uyd.png)






#   Cryptocurrencies-Analysis-Summary

It can be seen that all the models have very low precision for high risk credit/loan. This means that these models show weak precision in determining which credit risk is high. 
However the Easy Assemble Adaboost Classifier has the highest accuracy of 93%. For high risks, the sensitivity is 91%, which is high, and shows that this model can detect the high risk credits. However the precision is still very low for high risks. However the precision is good for detecting low risk credits.
Of all these models, Easy Assemble Adaboost Classifier seems to be the most feasible to be used for Credit Risk Analysis, although it has the shortcoming of a low precision for high risks.






