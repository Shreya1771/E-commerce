# E-commerce
MySql

mysql> select * from admin;
+---------+-----------+---------------+
| AdminID | AdminName | AdminPassword |
+---------+-----------+---------------+
|       1 | admin     | admin         |
+---------+-----------+---------------+
1 row in set (0.00 sec)

mysql> select * from category;
+------------+--------------+------------------------------------+
| CategoryID | CategoryName | Description                        |
+------------+--------------+------------------------------------+
|        111 | Women        | All products under women category. |
|        112 | Men          | All products under men category.   |
|        113 | Kids         | All products under kids category.  |
+------------+--------------+------------------------------------+
3 rows in set (0.00 sec)

mysql> select * from customer;
+------------+----------------+----------+--------+---------+------------+--------------------+----------+-------------+------------------+
| CustomerID | CustomerName   | Address  | City   | Country | Phone      | Email              | Password | ShipAddress | PendingShipments |
+------------+----------------+----------+--------+---------+------------+--------------------+----------+-------------+------------------+
|          1 | Ram            | Delhi    | Delhi  | India   | 9999111111 | ram@gmail.com      | ram      | Delhi       |                5 |
|          2 | Rita           | LA       | LA     | USA     | 1234567890 | rita@gmail.com     | rita     | LA          |                5 |
|          3 | Anannya Uberoi | Shalimar | Delhi  | India   | 8881       | anannya@gmail.com  | anannya  | Shalimar    |                5 |
|          4 | Sarthika       | Rohini   | Delhi  | India   | 998        | sarthika@gmail.com | sarthika | Rohini      |                5 |
|          5 | Katy           | Albany   | NY     | USA     | 773        | katy@gmail.com     | katy     | NY          |                5 |
|          6 | Logan          | Mumbai   | Mumbai | India   | 8711       | logan@gmail.com    | logan    | Mumbai      |                5 |
+------------+----------------+----------+--------+---------+------------+--------------------+----------+-------------+------------------+
6 rows in set (0.00 sec)

mysql> select * from orderdetails;
+---------+-----------+------------+
| OrderID | ProductID | CustomerID |
+---------+-----------+------------+
|       1 |        11 |          1 |
|       2 |        15 |          5 |
|       3 |        11 |          1 |
+---------+-----------+------------+
3 rows in set (0.00 sec)
mysql> select * from orders;
+---------+------------+------------+-----------+-----------------+--------+-------------------+------------+------------+
| OrderID | CustomerID | SupplierID | PaymentID | DeliveryCharges | Amount | TransactionStatus | ShipDate   | OrderDate  |
+---------+------------+------------+-----------+-----------------+--------+-------------------+------------+------------+
|       1 |          1 |      11111 |         1 |              50 |    500 | success           | 2017-04-20 | 2017-04-15 |
|       2 |          5 |      11112 |         2 |              50 |    500 | success           | 2017-04-20 | 2017-04-15 |
|       3 |          1 |      11111 |         3 |              50 |    500 | success           | 2017-04-20 | 2017-04-15 |
+---------+------------+------------+-----------+-----------------+--------+-------------------+------------+------------+
3 rows in set (0.01 sec)

mysql> select * from payment;
+---------+-----------+-----------------+--------+
| OrderID | PaymentID | DeliveryCharges | Amount |
+---------+-----------+-----------------+--------+
|       1 |         1 |              50 |    500 |
|       2 |         2 |              50 |    500 |
|       3 |         3 |              50 |    500 |
+---------+-----------+-----------------+--------+
3 rows in set (0.00 sec)

mysql> select * from productorder;
+-----------+----------+--------+--------------+
| ProductID | Quantity | Status | DeliveryDate |
+-----------+----------+--------+--------------+
|        11 |        1 |        |              |
|        15 |        1 |        |              |
|        11 |        1 |        |              |
+-----------+----------+--------+--------------+
3 rows in set (0.00 sec)

mysql> select * from suppliers;
+------------+-------------------+-------------+---------+
| SupplierID | SupplierName      | Address     | Country |
+------------+-------------------+-------------+---------+
|      11111 | Dhanraj Textiles  | Delhi       | India   |
|      11112 | Pricely           | LA          | USA     |
|      11113 | ABCD Suppliers    | Noida       | India   |
|      11114 | Mango Biz         | South Delhi | India   |
|      11115 | Lilliput Clothing | Delhi       | India   |
+------------+-------------------+-------------+---------+
