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


## Clustering Cryptocurrencies Using K-means

Deliverable 3: Clustering Cryptocurrencies Using K-means

Create the elbow curve to find the best value for K to be used in K-means

![Screen Shot 2021-09-02 at 3.18.08 AM](https://i.imgur.com/vBuGvtf.png)

From the elbow curve it can be seen, that the best value for K is 4, as the line becomes horizontal after 4.

Executing the K-means model with the clusters as 4

![Screen Shot 2021-09-02 at 3.21.04 AM](https://i.imgur.com/okXlHoc.png)

Create a new DataFrame including predicted clusters and cryptocurrencies features

![Screen Shot 2021-09-02 at 3.23.21 AM](https://i.imgur.com/AfjZbPR.png)


## Visualizing Cryptocurrencies Results

Deliverable 4: Visualizing Cryptocurrencies Results

1. The three dimensional diagram: 3D-Scatter with the PCA data and the clusters

![Screen Shot 2021-09-02 at 3.27.27 AM](https://i.imgur.com/ADRWjWM.png)

It can been seen that BitTorrent is the only cryptocurrency in the class 2


2. The scatter plot

![Screen Shot 2021-09-02 at 3.31.21 AM](https://i.imgur.com/MHaQGpZ.png)


#   Cryptocurrencies-Analysis-Summary

The cryptocurrency input data has been preprocessed and processed through PCA, K-means and visualizations to create the set of tradable cryptocurrencies.

There are a total of 532 tradable cryptocurrencies

![Screen Shot 2021-09-02 at 3.35.26 AM](https://i.imgur.com/8dqUsPP.png)

A table has been created with the tradable cryptocurrencies

![Screen Shot 2021-09-02 at 3.35.52 AM](https://i.imgur.com/fN6tDrU.png)

Most of the cryptocurrenices belong to class 0 and 3.

The table and the visualizations can be analyzed to make investment decisions on the most feasible crytocurrencies.







