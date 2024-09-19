# Question1  
You are given a dataset of a fictional e-commerce platform. The dataset includes tables for users, products, orders, and order items. Design and write SQL queries to:

a. Find the top 5 customers by total spend in the last 30 days.

b. Find Most purchased product till date.

#Explaination 

#Ans 1.  
As in question it is asked that that you have to print top 5 customers by total spend in last 30 days.This means we need to check for any purchases made between August 20, 2024, and September 19, 2024 (current date).

we have joined the 2 tables namely users and orders in which we can see that there are no orders placed after August 10, 2024. Therefore, no customer has made any purchases within the last 30 days. As a result, the query will not return any customers since no purchases fall within the specified time frame.

If there had been customers making purchases during the last 30 days, the query would have displayed the top 5 customers by their total spend.

#Ans 2.
As in the question it is asked that we have to print most purchased product till date so for this we join the products table and order_items table for finding the required output. 
As there are 5 products with purchasing quantity till date 
Laptop: 3
Smartphone: 3
Headphones: 4
Running Shoes: 2
Backpack: 4

Both the Headphones and Backpack have the highest purchase quantities, with a total of 4 each. Therefore, the query should return both products as they are tied for the most purchased products till date.
OUTPUT:
+------------+--------------+----------------+
| product_id | product_name | total_quantity |
+------------+--------------+----------------+
|          5 | Backpack     |              4 |
|          3 | Headphones   |              4 |
+------------+--------------+----------------+
 

