## Create a Microsoft Fabric Data Warehouse
** In this lab, I will Create a Fabric Data Warehouse and configure database objects.

#### Prerequisites
- A workspace

### Step 1: Create the Warehouse
  - Click New Item.
  - Select Warehouse.
  - Enter: "NameYourWarehouse"
  - Click Create.

**Fabric automatically provisions the warehouse environment.**

### Step 2: Create Warehouse Schemas

Open the SQL query editor and run:

CREATE SCHEMA sales;

Schemas help organize database objects logically.

Step 3: Create Tables

Create a table to store sales data:

CREATE TABLE sales.orders
(
OrderID INT,
CustomerName VARCHAR(100),
Product VARCHAR(100),
Quantity INT,
OrderDate DATE
);
