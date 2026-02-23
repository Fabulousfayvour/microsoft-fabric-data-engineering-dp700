# Data Ingestion in Microsoft Fabric

## Objective
To ingest data into Microsoft Fabric using Dataflows Gen2, and file uploads to OneLake.

---

##  Prerequisites
- Microsoft Fabric Workspace
- Lakehouse created
- Sample dataset (CSV or Parquet)

---

##  Step-by-Step Process

### Method 1: Ingest Data Using Dataflows Gen2
1. Open Microsoft Fabric portal
2. Navigate to **Data Factory**
3. Click **New → Dataflow Gen2**
4. Select data source (CSV, SQL Database, Web, etc.)
5. Use Power Query Online to:
   - Remove null values
   - Rename columns
   - Change data types
6. Save and publish the dataflow to Lakehouse

---

###  Method 2: Upload Files to OneLake
1. Open Fabric Workspace
2. Open the Lakehouse
3. Click **Files → Upload**
4. Upload dataset (e.g., sales.csv)


##  Outcome
- Raw data successfully ingested into OneLake
- Data available in Lakehouse Files and Tables


---

##  Key Learnings
- Dataflows Gen2 provides no-code ingestion and transformation
- OneLake acts as a unified data storage layer
