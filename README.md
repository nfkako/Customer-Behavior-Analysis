# Customer Behaviour Analysis
### Project Overview

Hello and welcome!

1. Are you a retail business seeking a broader understanding of your customers' behaviours?
2. Are you interested in increasing your sales and customer satisfaction?

If yes, then look no further.

This project aims to answer the above critical business questions using Recency, Frequency, Monetary (RFM) analysis and Machine Learning techniques such as K-means clustering for customer segmentation, and by applying Market Basket Analysis (MBA) technique in order to find the items that customers purchase together. This helps the retail business store or website design their layout in a manner that meets customer satisfaction and boosts sales at the same time. 

### Data Description
This Online Retail II dataset contains all the transactions occurring for a UK-based and registered, non-store online retail between 01/12/2009 and 09/12/2011.The company mainly sells unique all-occasion gift-ware. Many customers of the company are wholesalers.

The dataset consists of over 1m rows, and below are the columns and their descriptions:
- **Invoice**: Invoice number. A 6-digit number uniquely assigned to each transaction. If this code starts with the letter 'c', it indicates a cancellation.
- **StockCode**:Product (item) name.
- **Description**: Product (item) name. Nominal.
- **Quantity**: The quantities of each product (item) per transaction.
- **InvoiceDate**: Invoice date and time. The day and time when a transaction was generated.
- **Price**: Unit price. Product price per unit in Great Britain Pounds GBP.
- **Customer ID**: Customer number. A 5-digit number uniquely assigned to each customer.
- **Country**: Country name. The name of the country where a customer resides.

#### Sprint1
In this stage I have done the first pass of EDA in order to explore the dataset and identify data quality issues, feature engineering opportunities and any other notable observations regarding data preprocessing.

*Main Issues*

- Missing values:   
  - Customer ID: 240k           
  - Description: 4k

- Bad Documentation
  - 1.2k items have more than one description.
  - 300 items have no description at all (missing values).

- Item price is not constant:
  - For example: a Car Flag price ranges between £0.42 - £1,000

- Other charges/expenses:
  - Bank Charges
  - Amazon Fees
  - Bad debt Adjustment

##### Feature engineering to calculate:
- Recency 
- Frequency		
- Monetary

Details can be found in `Notebooks` folder in Sprint1 file.

#### Sprint2

This sprint of the project covers:

- Exploratory Data Analysis EDA
- Recency, Frequency, Monetary RFM Analysis
- Clustering

 In the EDA the main focus will focus on data cleaning where I will be dealing with the issues mentioned in sprint1, then I will move forward with feature engineering to create a dataframe and calculate the RFM metrics (Recency, Frequency and Monetary values) for each customer. The final section of this sprint would be clustering where I will basically try different algorithms with a range of K values and evaluate their performance using sillouette score.

Refer to Sprint2 notebook in `Notebooks` folder for more details.

### Final Stage

This stage of the project will integrate Market Basket Analysis within each customer group to analyze product associations and purchasing patterns specific to each ot them.


`Data`: This folder contains the link to the dataset as well as a cleaned copy of it.

`Notebooks`: This folder contains all python code notebooks used in project.

`Presentation files`: This folder condtains all the presentation files for this project.
