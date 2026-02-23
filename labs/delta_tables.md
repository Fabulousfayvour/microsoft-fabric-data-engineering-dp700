# Creating Managed and External Delta Tables in Microsoft Fabric

## Objective
To create and understand the two types of Delta tables in Microsoft Fabric:
1. Managed (Internal) Delta Tables  
2. External (Unmanaged) Delta Tables  

This lab demonstrates how data is stored, managed, and governed in a Lakehouse environment.

---

## Prerequisites
- Microsoft Fabric Workspace
- Lakehouse created
- Sample dataset uploaded to OneLake (e.g., sales.csv)
- Fabric Notebook attached to Lakehouse

---

# Part 1: Create a Managed Delta Table

##  Step 1: Open a Fabric Notebook
1. Go to Microsoft Fabric Workspace  
2. Click **New → Notebook**  
3. Attach the notebook to your Lakehouse  

---

## 🔹 Step 2: Load Data into Spark

```python
df = spark.read.csv("/lakehouse/default/Files/sales.csv", header=True, inferSchema=True)
df.show()
```
Step 3: Create a Managed Delta Table
df.write.format("delta").mode("overwrite").saveAsTable("sales_managed")
or
df.write.format("delta").saveAsTable("managed_products")

## 🔹 Step 4: Verify the Table
SELECT * FROM sales_managed;
 Outcome (Managed Table)

Table stored in Spark-managed Lakehouse storage

Metadata and data fully controlled by Fabric

Dropping the table will delete the data



# Part 2: Create an External Delta Table
### 🔹 Step 1: Save Data to External Location in OneLake
df.write.format("delta").mode("overwrite").save("/lakehouse/default/Files/sales_external")
or
df.write.format("delta").saveAsTable("external_products", path="abfs_path/external_products")
### 🔹 Step 2: Register External Delta Table
CREATE TABLE sales_external
USING DELTA
LOCATION '/lakehouse/default/Files/sales_external';
### 🔹 Step 3: Query External Table
SELECT * FROM sales_external;

🔹 Step 4: Drop Table Test (Optional)
DROP TABLE sales_external;

 Data will remain in OneLake storage, proving it is external.

####  Outcome (External Table)

- Data stored in a user-defined location

- Spark manages only metadata

- Dropping the table does NOT delete data

##  Managed vs External Delta Tables Comparison

| Feature | Managed Delta Table | External Delta Table |
|----------|--------------------|----------------------|
| **Definition** | Table where Spark/Fabric manages both metadata and data storage | Table where Spark/Fabric manages metadata but data is stored in a user-defined location |
| **Data Storage Location** | Spark/Lakehouse managed directory | User-specified path (OneLake, ADLS Gen2, S3, etc.) |
| **Metadata Management** | Managed by Spark | Managed by Spark |
| **Data Deletion on DROP TABLE** | Data is deleted |  Data remains in storage |
| **Use Case** | Development, testing, internal analytics | Enterprise production systems |
| **Data Governance** | Moderate | Strong (better lifecycle control) |
| **Data Sharing** | Limited | Easy to share across tools and platforms |
| **Performance** | High | High (depends on storage and optimization) |
| **Typical Industry Usage** | Learning and small workloads | Large-scale enterprise analytics platforms |
 
 ## Key Learnings

- Managed tables are easier and suitable for testing and internal analytics

- External tables separate storage from compute, which is preferred in enterprise environments

- Delta Lake provides ACID transactions, versioning, and schema enforcement

- Microsoft Fabric Lakehouse supports both managed and external Delta tables in OneLake

  #### Conclusion

This lab demonstrates how Delta Lake tables are created and managed in Microsoft Fabric.
Understanding the difference between managed and external Delta tables is essential for designing scalable and governed data platforms.


