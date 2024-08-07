# MySQL-Project: Supply Chain optimisation
Source: Shivan Kumar Case study Project work

# Problem:
A company is in the retail industry and sources products from various suppliers. The database contains information about suppliers, products, orders, and shipments, which can be leveraged to improve supply chain operations.

#Database Schema

# Table 1: 
# Suppliers Table
It contains the following information:
- supplier_id (Primary Key)
- supplier_name
- contact_person
- phone_number

# Table 2: Products Table
It contains the following information:
- product_id (Primary Key)
- product_name
- description
- unit_price
- quantity_in_stock

# Table 3: Orders Table
It contains the following information:
- order_id (Primary Key)
- product_id (Foreign Key)
- supplier_id (Foreign Key)
- order_date
- quantity_ordered
- order_status

# Table 4: Shipments Table
It contains the following information:
- shipment_id (Primary Key)
- order_id (Foreign Key)
- shipment_date
- delivery_date
- shipping_company
- tracking_number

# TO FIND:

1) Find the top 5 suppliers with the highest total quantity ordered:

- Here I have used the join function to join the suppliers table with the orders table.
- Then I have used "group by" to find the total quantity ordered per supplier id.
- In the last, I have used "order by" to find the top 5 suppliers.

2) Calculate the average delivery time for each shipping company:

- Here I have used the DATEDIFF function to find out the difference between the shipment date and the delivery date.
- Then, I have used the AVG function to find out its average.

3) Identify Seasonal Demand Patterns:

- Here I have used the date format function.

4) Forecast Future Demand:

- For this, I have used DATEFORMAT, Group BY, Order by, SUM, etc.

5) Calculate the total number of orders made each month:

- Use of Count function.

# OTHER BASIC QUESTIONS ANSWERED ARE:

- Display orders that are in progress (order_status = 'In Progress')
- Find the earliest and latest order dates
- Calculate the total revenue generated from orders
-  List suppliers who have not yet made any orders
