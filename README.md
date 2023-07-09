## Unsupervised Learning

## Libraries used : Pandas, Numpy, Sci-learn kit, MatplotLib, Seaborn 

## Data - 18 features with 8950 points 

## Features
* CUSTID: Identification of Credit Card holder
* BALANCE: Balance amount left in customer's account to make purchases
* BALANCE_FREQUENCY: How frequently the Balance is updated, score between 0 and 1 (1 = frequently updated, 0 = not frequently updated)
* PURCHASES: Amount of purchases made from account
* ONEOFFPURCHASES: Maximum purchase amount done in one-go
* INSTALLMENTS_PURCHASES: Amount of purchase done in installment
* CASH_ADVANCE: Cash in advance given by the user
* PURCHASES_FREQUENCY: How frequently the Purchases are being made, score between 0 and 1 (1 = frequently purchased, 0 = not frequently purchased)
* ONEOFF_PURCHASES_FREQUENCY: How frequently Purchases are happening in one-go (1 = frequently purchased, 0 = not frequently purchased)
* PURCHASES_INSTALLMENTS_FREQUENCY: How frequently purchases in installments are being done (1 = frequently done, 0 = not frequently done)
* CASH_ADVANCE_FREQUENCY: How frequently the cash in advance being paid
* CASH_ADVANCE_TRX: Number of Transactions made with "Cash in Advance"
* PURCHASES_TRX: Number of purchase transactions made
* CREDIT_LIMIT: Limit of Credit Card for user
* PAYMENTS: Amount of Payment done by user
* MINIMUM_PAYMENTS: Minimum amount of payments made by user
* PRC_FULL_PAYMENT: Percent of full payment paid by user
* TENURE: Tenure of credit card service for user

## Basic Stats of the Data

* Mean balance is $1564 
* Balance frequency is frequently updated on average ~0.9
* Purchases average is $1000
* One off purchase average is ~$600
* Average purchases frequency is around 0.5
* Average ONEOFF_PURCHASES_FREQUENCY, PURCHASES_INSTALLMENTS_FREQUENCY, and CASH_ADVANCE_FREQUENCY are generally low
* Average credit limit ~ 4500
* Percent of full payment is 15%
* Average tenure is 11 years

## Data Pre-processing
#### Fill out missing data points (null elements)
*  Filled up the missing elements with mean of the 'MINIMUM_PAYMENT'
*  Filled up the missing elements with mean of the 'CREDIT_LIMIT'
#### Checked for duplicate entries
#### Converting text data into numbers 

## Done the Kernel Density Estimate 
* distplot combines the matplotlib.hist function with seaborn kdeplot(). KDE Plot represents the Kernel Density Estimate
* KDE is used for visualizing the Probability Density of a continuous variable and demonstrates the probability density at different values in a continuous variable.

![image](https://github.com/Aniket2k15/Market-Segmentation/assets/138878014/e155e2da-6de8-43c1-848f-c530fa044647)


## Scaled the data using StandardScalar()

## Finding the optimal number of clusters using elbow method 
* The elbow method is a heuristic method of interpretation and validation of consistency within cluster analysis designed to help find the appropriate number of clusters in a dataset
* If the line chart looks like an arm, then the "elbow" on the arm is the value of k that is the best.

![image](https://github.com/Aniket2k15/Market-Segmentation/assets/138878014/cc0231b2-6827-4fdb-951f-dc970e4c3d48)


## Ploting the histogram of various clusters
![image](https://github.com/Aniket2k15/Market-Segmentation/assets/138878014/49a1b43d-88e6-4b88-b3d9-a3d164552392)

## Obtaining the principal components 
![image](https://github.com/Aniket2k15/Market-Segmentation/assets/138878014/43785f11-0233-49a4-93cd-44adfdf2905a)

## Concatenating the clusters labels to 2 components 
![image](https://github.com/Aniket2k15/Market-Segmentation/assets/138878014/0d10bb69-d881-46d3-8a7d-5d9443970fb1)

# Plotting the Final segmented Groups

![image](https://github.com/Aniket2k15/Market-Segmentation/assets/138878014/448992aa-53c1-44ed-a59c-0bf51694ea18)










  





























