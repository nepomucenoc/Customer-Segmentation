# Customer Segmentation in Sample Sales Data
Customer segmentation creates groups of people with the same characteristics. This is a better way to understand the needs and preferences of each customer, so this information is useful to better target those needs and preferences in order to increase the revenue of some companies.

![image](https://github.com/nepomucenoc/Customer-Segmentation/assets/72771264/a86e0324-bac3-4110-9cd9-78830fb1cb8c)

Abstract vector created by vectorjuice - www.freepik.com

**Overview of the dataset:**

This data is about sales with prices, status, products, etc.

This dataset contains 2823 rows and 25 columns.

You can see this dataset in the link: https://www.kaggle.com/kyanyoga/sample-sales-data


**Dictionary of the dataset:**

* **ORDERNUMBER**:  Unique ID for each order made by a customer, number invoice;
* **QUANTITYORDERED**: Quantity of the products sold in the invoice, specified by ORDERNUMBER;
* **PRICEEACH**: Price each product;	
* **ORDERLINENUMBER**: 	
* **SALES**: Total value in invoice. (QUANTITYORDERED x PRICEEACH);	
* **ORDERDATE**: purchase date;
* **STATUS**: purchase status (canceled, in process, on hold, resolved, Disputed or shipped);
* **QTR_ID**:[ 1,2,3,4 ] for the Quarters of the Year;	
* **MONTH_ID**: purshase month;
* **YEAR_ID**: purshase year;
* **PRODUCTLINE**: Type of product; 	
* **MSRP**: Manufacturer's Suggested Retail Price, is the price that a manufacturer recommends for stores to sell their product. Some retailers may also refer to the MSRP as the "list price."	
* **PRODUCTCODE**: code of the product; 	
* **CUSTOMERNAME**: Name of the customer of the considered order; 	
* **PHONE**: client phone;	
* **ADDRESSLINE1**: Client adress;	
* **ADDRESSLINE2**: Client adress;
* **CITY**: purchase city;	
* **STATE**: purchase state;	
* **POSTALCODE**: number of postalcode;	
* **COUNTRY**: purchase country;
* **TERRITORY**: purshase territory;
* **CONTACTLASTNAME**: Fist client name;	
* **CONTACTFIRSTNAME**: Last client name;	
* **DEALSIZE**: Product size.

**Objective**:

The model must learn from the data and be able to make similarities between clients through unsupervised learning Clustering. Furthermore, will be made RFM Score with clients to separate into groups of clients with target "platinum", "gold", "silver", and "bronze", and with the client's "bronze" will be made Regression Model forecast sales to do campaigns to sale more and rescue this customer. 

## **Notebook**

**Checklist:**

1. Import the libraries;
2. Load dataset and information;
3. First preprocessing and visualization of the dataset;
4. RFM Modeling;
5. K-Means Clustering;
6. Using Purchase Forecasts (Prophet);
7. Regression Model;
8. LightGBM to Regression;
9. Conclusions of the project.

### **Abstract of the project:**

**1. Import the libraries:**

In this first part, it is imported the libraries and frameworks that are used during this project. 

**2. Load dataset and information:**

Also, it displays the data and some characteristics, like the number of samples and features, if exist null or NaN values in the dataset, and counts the unique values for each feature.

**3. First preprocessing and visualization of the dataset:**

In the third part, some graphics are made to visualize the dataset for some insights about the problem, for example, the correlation between the features. Besides, some features that aren't necessary are withdrawn.

**4. RFM Modeling:**

In this part, it is applied to customer segmentation, where we segmented the clients in groups to identify which client needs attention and predict how much these clients will spend and future campaigns to regard this client.

**5. K-Means Clustering:**

In this part, it is applied the Elbow Method to find the number of clusters in the dataset. After that, it is used them K-means to build the clusters and take some important insights from each group.

**6. Using Purchase Forecasts (Prophet):**

In this section, we will catch the clients that need attention and do purchase forecasts to offer products with the same price.

**7. Regression Model:**

With the client's group that needs attention, we use this data to predict with Regression how much these clients will spend and future campaigns to regard this client.

**8. LightGBM to Regression:**

The same thing will be done to predict how much these clients will spend and in the future to make campaigns to regard this client but is with the algorithm LightGBM.

**9. Conclusions of the project:**

This final part shows a summary of the results that are achieved in each part of the project.

