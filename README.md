# Instacart-EDA-ProductRecommendation-and-clustering

Objective
We have two objectives in this project
1.	To perform Exploratory Data Analysis on the dataset using Spark and Pandas. We are also doing a performance comparison between the two
2.	Market Basket Analysis : 

Market Basket Analysis is a technique based on the theory that if you buy a certain group of items, you are more or less likely to buy another group of items. Market basket analysis may provide the companies with insights to understand the purchase behavior of a customer. This information can then be used for purposes of influencing sales, promotions, loyalty programs, store design, and discount plans, etc.
a.	Our first objective here is to recommend products to the user based on the current item selected by the user. We will be using Association rules to determine which products to recommend to the user.
b.	Secondly we have used KMeans clustering to divide the customers into groups or clusters based on their common characteristics (i.e what kind of products they buy) and determine which set of customers prefers buying which set of products.

Dataset Description : 
aisles.csv : This file contains different aisles and there are total 134 unique aisles.
departments.csv: This file contains different departments and there are total 21 unique departments.
orders.csv: This file contains all the orders made by different users and to which set (prior, train, test) an order belongs.
products.csv: This file contains the list of total products and their aisle as well as department. The number of products in different aisles and different departments are different.
order_products_prior.csv : This file gives information about which products were ordered and in which order they were added in the cart. It also tells us that if the product was reordered or not. In this file there is an information of total orders through which total products (around 50k) were ordered.
order_products_train.csv: This file gives information about which products were ordered and in which order they were added in the cart. It also tells us that if the product was reordered or not.


Libraries used: 
The only third-party libraries that we have used are for Spark. The instructions on downloading and setting environment variables for those are present in the first 3 cells of  
‘EDA and Performance Comparison between Spark and Pandas’  Google Colab Notebook.
Running them would install and set up variables in the Colab Environment.

Issues and Challenges
1.	The main issue we faced was memory issue. The main reason for it was that the entire RAM allocated to Google Colab was being used up leading to crashing of the sessions. Accordingly actions have been taken in the code like Garbage Collection and reducing DataFrame size. Instructions and comments on how to run the code to avoid memory error have been mentioned in the code.
2.	We have plotted the graphs using pandas DataFrame since Spark does not having functions to plot graphs.


