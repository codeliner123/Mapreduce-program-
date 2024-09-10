Problem Statement

The goal is to calculate the total revenue generated from sales for each product 

in a given dataset containing transaction details.

2. Description

The code is designed to process a CSV file containing sales transactions using the 

MapReduce framework (mrjob). Each transaction has a TransactionID, ProductID, Quantity, 

Price, and Date. The mapper function extracts the ProductID, Quantity, and Price from 

each line, calculates the revenue for each transaction, and yields it. The reducer 

function then aggregates the revenues by ProductID to calculate the total revenue per product.

3. Instructions on How to Run the Code

1. Install the necessary libraries by running:

 pip install mrjob

2. Save the provided Python code into a file, e.g., sales_revenue.py.

3. Prepare your input CSV data in the format:

 TransactionID, ProductID, Quantity, Price, Date

4. Run the code with the following command:

 python sales_revenue.py <inputfile.csv>

5. The output will display the total revenue generated for each product.
