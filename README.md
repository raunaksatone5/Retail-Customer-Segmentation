# Retail-Customer-Segmentation
![image](https://user-images.githubusercontent.com/102457644/192557276-75f9297d-ac4f-482d-9b25-3e02a2afe764.png)


## **Problem Description**

### In this project, your task is to identify major customer segments on a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.


## <b> Data Description </b>

### <b>Attribute Information: </b>

* ### InvoiceNo: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation.
* ### StockCode: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
* ### Description: Product (item) name. Nominal.
* ### Quantity: The quantities of each product (item) per transaction. Numeric.
* ### InvoiceDate: Invice Date and time. Numeric, the day and time when each transaction was generated.
* ### UnitPrice: Unit price. Numeric, Product price per unit in sterling.
* ### CustomerID: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
* ### Country: Country name. Nominal, the name of the country where each customer resides.

## Business Use Case:
* Targeted Marketing: By segmenting customers based on their behavior, interests and demographics, businesses can tailor their marketing campaigns and promotions to specific groups, resulting in higher response rates and conversions.
* Cross-selling and Upselling: Customer segmentation can help businesses identify customers who are likely to purchase complementary or premium products, and target them with personalized recommendations.
* Customer Retention: By understanding customer behavior and preferences, businesses can design and implement strategies to reduce churn and increase customer loyalty.
* Personalized Customer Experience: Segmentation can help businesses understand customer needs and tailor their offerings, such as product recommendations, customer service, and overall experience, to meet those needs.
* Improved Customer Insights: Customer segmentation provides valuable insights into customer behavior and preferences, which can inform future business decisions and strategies.
* Optimization of Resource Allocation: By prioritizing and focusing resources on high-value customer segments, businesses can optimize their marketing and sales efforts, reduce costs, and increase ROI.

## Data Pre-Processing
* Implemented libraries such as pandas, numpy,matpplotlib,seaborn,Scikit-learn
* Got the descriptive information of the data.
* checked for null values if any
* Checked for Outliers and duplicated values if any.

## Data Cleaning
* got rid of rows with null customerID
* got rid of duplicated values
* Dropped the id column since it is of no significance to our model training
* Imputed null values with knn imputer and simple imputer
* treated outliers

## Exploratory Data Analysis
* visualized maximum ordering countries.
* Visualized month wise orders
* checked the distribution of Revenue with the help of boxplot.

## Feature Engineering
* Applied RFM analysis which allows you to segment customer by the frequency and the value of purchases and how recent was the purchase.
* labelled customer based on the RFM score range 1-4
* Performed log transforamtion on RFM features to noramalize them.

Model training :
* Used Elbow method, silhouete score, davies bouldin score to come up with optimum value of cluster for K-means
* plotted dendogram baased on agglomerative hierrachical clustering.
* found optimum cluster value to be 2 in both the clustering methods.
