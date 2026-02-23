# Data Processing with Apache Spark in Microsoft Fabric

#  Objective
To transform and analyze data using Apache Spark notebooks in Microsoft Fabric.

---

##  Step-by-Step Process

### Step 1: Create a Notebook
1. Open Fabric Workspace
2. Click **New → Notebook**
3. Attach the notebook to the Lakehouse

---

### Step 2: Load Data into Spark

```python
df = spark.read.csv("/lakehouse/default/Files/sales.csv", header=True)
df.show()
```

Step 3: Clean and Transform Data

Remove duplicates
Convert data types
Create derived columns

df_clean = df_clean.withColumnRenamed("OldColumn", "NewColumn")
Step 4: Save as Delta Table
df_clean.write.format("delta").mode("overwrite").saveAsTable("sales_silver")

#### Outcome

Cleaned data stored in Delta Lake format

Silver layer dataset created in Lakehouse



###  Key Learnings

- Spark enables distributed data processing

- Fabric notebooks support PySpark and SQL

- Delta format improves performance and reliability
