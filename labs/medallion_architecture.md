# Implementing Medallion Architecture in Microsoft Fabric

##  Objective
To design and implement a Medallion Architecture (Bronze, Silver, Gold layers) in Microsoft Fabric Lakehouse.

---

##  Step-by-Step Process

###  Bronze Layer (Raw Data)
- Ingest raw data using Dataflows or file uploads
- Store raw datasets in Lakehouse Files

---

### Silver Layer (Cleaned Data)
- Use Spark notebooks to clean and transform data
- Save transformed data as Delta tables

---

###  Gold Layer (Analytics Ready)
- Aggregate and optimize datasets
- Create business-ready tables for reporting

---

##  Outcome
- Layered Lakehouse architecture implemented
- Clean analytics-ready datasets created
---

## Key Learnings
- Medallion architecture improves data quality
- Layered approach supports scalable analytics
- Fabric Lakehouse supports multi-layer Delta tables
