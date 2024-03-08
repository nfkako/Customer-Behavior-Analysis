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
- **InvoiceNo**: Invoice number. Nominal. A 6-digit integral number uniquely assigned to each transaction. If this code starts with the letter 'c', it indicates a cancellation.
- **StockCode**: Product (item) code. Nominal. A 5-digit integral number uniquely assigned to each distinct product.
- **Description**: Product (item) name. Nominal.
- **Quantity**: The quantities of each product (item) per transaction. Numeric.
- **InvoiceDate**: Invoice date and time. Numeric. The day and time when a transaction was generated.
- **UnitPrice**: Unit price. Numeric. Product price per unit in sterling (£).
- **CustomerID**: Customer number. Nominal. A 5-digit integral number uniquely assigned to each customer.
- **Country**: Country name. Nominal. The name of the country where a customer resides.

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

#### Feature engineering to calculate:
- Recency 
- Frequency		
- Monetary

Details can be found in `Notebooks` folder in Sprint1 file.

### Next Stept

For the next stage of the project I will be conducting data cleaning, feature engineering and data preprocesing in order to deal with the issues identified in Sprint1, then I will use K-means clustering to devide the customers into different groups based on their purchasing behaviours...


`Data`: This folder contains the link to the dataset.

`Notebooks`: This folder contains all python code notebook used in project.

`Presentation files`: This folder condtains all the presentation files for this project.
