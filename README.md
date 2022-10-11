# Objective

The data have many features (18 behavioral features). We will now perform:

Data preprocessing
Clustering
Feature extraction to improve clustering
Experiment with various clustering models: KMeans, Agglomerative Hierarchical, Gaussian Mixture
Choosing the number of clusters
EDA to segment the customers
Concluding the project by giving marketing strategy based on what we learn from the data

# Data Description
Link to the dataset: Kaggle link

Following is the Data Dictionary for Credit Card dataset:

CUST_ID: Identification of Credit Card holder (Categorical)
BALANCE: Balance amount left in their account to make purchases
BALANCE_FREQUENCY: How frequently the Balance is updated, score between 0 and 1 (1 = frequently updated, 0 = not frequently updated)
PURCHASES: Amount of purchases made from account
ONEOFF_PURCHASES: Maximum purchase amount done in one-go
INSTALLMENTS_PURCHASES: Amount of purchase done in installment
CASH_ADVANCE: Cash in advance given by the user
PURCHASES_FREQUENCY: How frequently the Purchases are being made, score between 0 and 1 (1 = frequently purchased, 0 = not frequently purchased)
ONEOFFPURCHASESFREQUENCY: How frequently Purchases are happening in one-go (1 = frequently purchased, 0 = not frequently purchased)
PURCHASESINSTALLMENTSFREQUENCY: How frequently purchases in installments are being done (1 = frequently done, 0 = not frequently done)
CASHADVANCEFREQUENCY: How frequently the cash in advance being paid
CASHADVANCETRX: Number of Transactions made with "Cash in Advanced"
PURCHASES_TRX: Number of purchase transactions made
CREDIT_LIMIT: Limit of Credit Card for user
PAYMENTS: Amount of Payment done by user
MINIMUM_PAYMENTS: Minimum amount of payments made by user
PRCFULLPAYMENT: Percent of full payment paid by user
TENURE: Tenure of credit card service for user
Data Cleaning
One of the most important preprocessing steps in a Data Science project. In this project, I imputed missing values with the median value, dropped the CUST_ID column, then normalized the input values using StandardScaler(). You can check the codes here.

# Clustering
### Correlation Check
![Ca](https://user-images.githubusercontent.com/68142873/195020517-b80a218c-02a8-4375-af2c-925a094fc229.PNG)

# Clustering using K-Means
In this section we will perform K-Means clustering on the data and check the clustering metrics (inertia, silhouette scores).

## Inertia Plot
First, we make the inertia plot:

![3](https://user-images.githubusercontent.com/68142873/195020998-8d5c10b2-d751-4d4a-992a-6201904fc81b.PNG)

Using the elbow method, we pick a good number of clusters to be 6.

# Tsne with kmeans
![5](https://user-images.githubusercontent.com/68142873/195024510-82a5c17c-f5b4-4d1e-a46c-7254f2583caf.PNG)

# Tsne with isolation forest
![7](https://user-images.githubusercontent.com/68142873/195024982-8b77a4d2-004f-4955-a88a-bafda1180333.PNG)


