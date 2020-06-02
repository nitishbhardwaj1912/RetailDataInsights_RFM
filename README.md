> #### Don't find customers for your products,
> #### Find products for your customers. 
> #### <cite>-Seth Godin</cite>

<p align="center">
  <img width="400" height="250" src="https://cdn.dribbble.com/users/2788963/screenshots/6836348/bullseyeloop.gif" alt="Customer Focussed">
  </p>
  
<p align="center">
Image reference: [1] 
</p>

# Finding Insights from Retail Data
This repository contains objects related to finding insights from Retail Data.

## About Dataset

The raw data for this business problem is fetched from the SQLite database. The database consists of three tables: Transactions, Products and Segments.

Data is fetched from the database using the SQLite3 connector provided in Python.

The semantic description of the three tables mentioned in the Data Collection section is mentioned below:

1. `transactions`: contains detailed information about each product a customer has purchased. A transaction consists of one or more products purchased by a customer indexed by unique transaction id. Following columns are present in this table:
	* `trans_id`: the transaction id
	* `cust_id`: the customer id
	* `prod_id`: the product id
	* `item_qty`: the quantity of the product that is being purchased
	* `item_price`: the per-unit price of the product (NOTE: the total revenue for a product is `item_qty * item_price`)
	
2. `products`: contains detailed attributes about each product.
	* `prod_id`: the product id (same meaning as in `transactions`)
	* `prod_name`: the product name
	* `brand`: the brand of the product
	* `category`: the category of the product
	
3. `segments`: contains a history of customer segmentation labelling for each customer. Segments are computed periodically for all current customers and appended to the table after each computation. The current (most up to date) active segment for each customer is specified by `active_flag = 'Y'` column.
	* `cust_id`: the customer id (same meaning as in `transactions`)
	* `seg_name`: the segment of this customer
	* `update_dt`: the date when this segment was updated
	* `active_flag`: whether or not this segment is the active segment for this customer

## Business Problem

COVID 19 had a hard hit on all the industries in the year 2020. It forced most of the businesses to move online. It inspired customers to buy and try more products online. Only the organizations which are constantly evolving and making continuous structural changes aligned to customer needs would be able to sustain in this ever-changing time.

The year 2020 motivated a lot of the organizations to spend more money on finding insights on their data to provide a better customer experience to increase customer engagement and sales.

The business problem is having raw retail data from various sources and finding the opportunities to find insights that would help re-align the business for better growth.

## Detailed Project Report can be viewed at this link:
<a href="https://nbviewer.jupyter.org/github/nitishbhardwaj1912/RetailDataInsights_RFM/blob/master/Nitish%20Bharadwaj_Project%20Report_FINDING%20INSIGHTS%20FROM%20RETAIL%20DATA.pdf">Project Report</a>

## Detailed Project Presentation can be viewed at this link:
<a href="https://nbviewer.jupyter.org/github/nitishbhardwaj1912/RetailDataInsights_RFM/blob/master/Nitish%20Bhardwaj_Project%20Presentation_FINDING%20INSIGHTS%20FROM%20RETAIL%20DATA.pdf">Project Presentation</a>

## Project output, code and analysis performed can be viewed at this link:
https://nitishbhardwaj1912.github.io/RetailDataInsights_RFM/

## References:
[1] "Bullseye", Dribbble, 2020. [Online]. Available: https://cdn.dribbble.com/users/2788963/screenshots/6836348/bullseyeloop.gif. [Accessed: 31- May- 2020].