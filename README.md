# SQL Data Mining Assignment

## Description
This assignment focuses on practicing data mining with SQL. It involves creating a database to store product information and executing SQL queries to retrieve specific data that answers a business question. The primary goal is to showcase products with a price under $100 and understand how to manipulate and retrieve data using SQL effectively.

## Database Structure
### Database: `assignment_db`
- **Table: `products`**
- 
  - `id INT (Auto-increment, Primary Key)
  - `product_name VARCHAR(255) (Name of the product)
  - `category VARCHAR(255) (Category of the product)
  - `price DECIMAL(10,2) (Price of the product)
  - `stock_quantity INT (Available stock for the product)

### Sample Data
| id | product_name              | category           | price  | stock_quantity  |
|----|---------------------------|--------------------|------- |-----------------|
| 1  | Wireless Mouse            | Electronics        | 29.99  | 150             |
| 2  | Bluetooth Headphones      | Electronics        | 49.99  | 75              |
| 3  | Yoga Mat                  | Fitness            | 19.99  | 200             |
| 4  | Coffee Maker              | Home Appliances    | 89.99  | 50              |
| 5  | USB-C Charging Cable      | Accessories        | 9.99   | 300             |
| 6  | Desk Organizer            | Office Supplies    | 12.99  | 200             |
| 7  | HDMI Cable                | Accessories        | 14.99  | 200             |
| 8  | Water Bottle              | Fitness            | 15.99  | 120             |
| 9  | Laptop Stand              | Accessories        | 25.00  | 150             |
| 10 | Fitness Tracker           | Wearables          | 49.99  | 90              |
| 11 | Gaming Keyboard           | Electronics        | 79.99  | 80              |
| 12 | Smartwatch                | Wearables          | 99.99  | 60              |

# SQL Queries
# Query to Retrieve Products Under $100
To find products with a price under $100, the following SQL query is used:

# Query
SELECT * FROM products WHERE price < 100 ORDER BY price ASC;

# Explanation

*SELECT : This statement selects all fields from the products table.
WHERE price < 100: This condition filters the results to only include products priced under $100.
ORDER BY price ASC: This sorts the resulting products in ascending order based on their price.

# Screenshots
The output of the SQL query can be found in the file named SQLQuery.png. This screenshot demonstrates the result set obtained after executing the query, showing the products that meet the specified criteria.

## How to Run
Ensure you have a MySQL server running.
Create the assignment_db database using the provided SQL scripts.
Insert the sample data into the products table.
Run the SQL query to view the filtered results.
Conclusion
# This assignment has enhanced my understanding of SQL data retrieval and data mining concepts. I am now better equipped to handle business-related queries using SQL effectively
