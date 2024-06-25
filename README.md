# Customer Segmentation using K-Means Clustering and Autoencoders

This project involves the analysis and segmentation of credit card customers using K-Means clustering and dimensionality reduction with autoencoders. 
The dataset used contains various attributes related to customer transactions and payment behaviors. 
The primary objective is to cluster customers into distinct groups to understand different customer behaviors and improve marketing strategies.

**Features:**
- `CUST_ID`: Identification of Credit Card holder 
- `BALANCE`: Balance amount left in customer's account to make purchases
- `BALANCE_FREQUENCY`: Frequency of balance updates
- `PURCHASES`: Amount of purchases made from account
- `ONEOFF_PURCHASES`: Maximum purchase amount in one-go
- `INSTALLMENTS_PURCHASES`: Amount of purchase done in installments
- `CASH_ADVANCE`: Cash in advance given by the user
- `PURCHASES_FREQUENCY`: Frequency of purchases
- `ONEOFF_PURCHASES_FREQUENCY`: Frequency of one-off purchases
- `PURCHASES_INSTALLMENTS_FREQUENCY`: Frequency of installment purchases
- `CASH_ADVANCE_FREQUENCY`: Frequency of cash advances
- `CASH_ADVANCE_TRX`: Number of cash advance transactions
- `PURCHASES_TRX`: Number of purchase transactions
- `CREDIT_LIMIT`: Credit card limit
- `PAYMENTS`: Amount of payment made by the user
- `MINIMUM_PAYMENTS`: Minimum amount of payments made by the user  
- `PRC_FULL_PAYMENT`: Percentage of full payment paid by the user
- `TENURE`: Tenure of credit card service for the user

## Data Preprocessing
The dataset is loaded and preprocessed by:
- Checking for missing values and filling them with mean values.
- Dropping unnecessary columns such as `CUST_ID`.
- Standardizing the data.

## Exploratory Data Analysis
Exploratory data analysis is performed to understand the distribution and correlation of different features. This includes:
- Descriptive statistics
- Histograms for feature distribution
- Correlation heatmap

## Clustering

### K-Means Clustering
K-Means clustering is applied to the standardized dataset to segment the customers. The elbow method is used to find the optimal number of clusters.

### Optimal Number of Clusters
The elbow method is applied, and the optimal number of clusters is determined. In this case, 7 clusters are chosen based on the elbow point in the inertia plot.

### Cluster Interpretation
The cluster centers are analyzed to understand the characteristics of each cluster. For example:
- Transactors: Customers who pay the least amount of interest charges and are careful with their money.
- Revolvers: Customers who use credit cards as a loan, with high balances and cash advances.

## Dimensionality Reduction with Autoencoders
Autoencoders are used to reduce the dimensionality of the dataset. This involves:
- Building an autoencoder model
- Training the autoencoder
- Using the encoder part of the model to reduce the dimensions of the dataset

## Visualization
The results are visualized using:
- Histograms of various clusters
- Scatter plots of the principal components obtained from PCA

## Conclusion
The project successfully segments the customers into distinct groups using K-Means clustering and autoencoders for dimensionality reduction.
These clusters provide valuable insights into customer behaviors, which can be used for targeted marketing strategies.

## License
This project is licensed under the MIT License .
