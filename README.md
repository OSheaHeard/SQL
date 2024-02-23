In this SQL I am querying a database with multiple tables to quantify statistics about a Superstore Database.

#1. Write your own SQL query that uses a SELECT statement to order the items by price
SELECT item_name, price
FROM superstore
ORDER BY price desc;

#2. Write your own SQL query that will show a statistic about the item prices, like a sum, average, minimum, maximum, or count.
SELECT SUM (price)
FROM superstore;

#3. Write your own SQL query that will show a statistic about the price for items in the category of "Kitchen Supplies".
SELECT SUM(price),category
FROM superstore
WHERE category= 'Kitchen Supplies';

#4. Come up with your own question about the data and try to answer it using SQL.
SELECT SUM(stock_quantity), item_name
FROM superstore
WHERE item_name= 'Air Purifier';
