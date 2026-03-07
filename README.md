# Microsoft Fabric Data Engineering (DP-700) Learning Repository

##  Overview
This repository documents my hands-on learning journey in **Microsoft Fabric Data Engineering (DP-700)**, focusing on modern lakehouse architecture, data ingestion, transformation, analytics, and orchestration using Microsoft Fabric.

The goal of this repo is to demonstrate practical implementation of **enterprise-grade data engineering concepts** using Microsoft Fabric, Delta Lake, Apache Spark, and Medallion architecture.

---

## Learning Path
- Microsoft Certified: Azure Data Fundamentals (DP-900) ✅ Completed
- Microsoft Certified: Fabric Data Engineer Associate (DP-700)  In Progress

---

## Key Concepts Covered

###  Data Ingestion in Microsoft Fabric
- Dataflows Gen2 (Power Query Online)
- Data Pipelines (Data Factory in Fabric)
- Real-time ingestion using Eventhouse (KQL Databases)
- File-based ingestion into OneLake

---

###  Lakehouse Implementation
- Creating Fabric Workspaces
- Creating and managing Lakehouses
- Apache Spark notebooks for data processing
- Delta Lake tables for structured analytics

---

###  Medallion Architecture
- **Bronze Layer** – Raw ingestion
- **Silver Layer** – Cleaned and transformed data
- **Gold Layer** – Aggregated analytics-ready data

---

###  Data Analytics & Visualization
- Semantic models
- Power BI integration with Fabric Lakehouse
- SQL Analytics Endpoint querying

---

###  Orchestration & Automation
- Data pipelines for ingestion and transformation
- Scheduling and dependency management

---

##  Real-Time Intelligence in Microsoft Fabric

In this topic, I learned how to **ingest, process, store, visualize, and act on data in motion** to generate insights from events as they happen.

### Key Topics Covered

- Using **Eventstream** for real-time data ingestion and processing
- Working with **Eventhouse** to store and analyze real-time event data
- Creating **real-time dashboards** for monitoring streaming data
- Using **Activator** to trigger automated actions based on event conditions

### Key Microsoft Fabric Components Used

- Real-Time Hub
- Eventstream
- Eventhouse
- KQL Database
- Real-Time Dashboard
- Activator

---

## Implementing a Data Warehouse with Microsoft Fabric

This topic focused on building and managing a **modern cloud data warehouse using Microsoft Fabric**.

### Key Topics Covered

- Creating and querying data in a Fabric **Warehouse**
- Loading data into a **Microsoft Fabric Data Warehouse**
- Querying the warehouse using **SQL**
- Monitoring warehouse performance and query execution
- Implementing **security and access control**

### Key Skills Practiced

- Data ingestion into Fabric warehouses
- Writing SQL queries for analytical workloads
- Monitoring query performance
- Securing warehouse objects and managing permissions

  
## Repository Structure

| Folder | Description |
|--------|-------------|
| `labs/` | Step-by-step lab documentation |
| `errors_and_troubleshooting/` | Errors faced and solutions |
| `certifications/` | Microsoft Learn badges and progress |

---

##  Labs Included

###  Data Ingestion
- Ingest data using Dataflows Gen2
- Orchestrate ingestion with Fabric Pipelines
- Real-time ingestion using Eventhouse

###  Lakehouse Implementation
- Create Workspace and Lakehouse
- Load data into OneLake
- Spark transformations

###  Delta Lake Tables
- Create managed Delta tables
- Time travel & ACID transactions

### Medallion Architecture
- Bronze → Silver → Gold transformation workflows

###  Analytics
- SQL queries on lakehouse
- Power BI semantic models

###  Real-Time Intelligence (RTI)

#### Creating Eventstreams
- Create and configure **Eventstreams**
- Connect streaming data sources
- Apply event transformations

#### Eventhouse and Streaming Storage
- Store streaming data in **Eventhouse**
- Understand **KQL databases**
- Manage real-time event data

#### Querying Real-Time Data
- Query streaming data using **KQL (Kusto Query Language)**
- Filter and aggregate event data
- Analyze event patterns in real time

#### Real-Time Visualization
- Create **Real-Time dashboards**
- Monitor streaming data metrics
- Visualize event trends and live data

#### Automation with Activator
- Create **Activator rules**
- Detect conditions from streaming events
- Trigger automated actions and alerts

###  Fabric Data Warehouse

#### Creating and Managing Warehouses
- Create a **Microsoft Fabric Warehouse**
- Manage warehouse objects (tables, schemas)
- Configure warehouse settings

#### Loading Data into Warehouse
- Load data using **COPY INTO**
- Load data using **Pipelines**
- Perform batch data ingestion

#### Querying and Monitoring Warehouse
- Query warehouse data using **SQL**
- Monitor query performance
- Track warehouse usage and activity

#### Securing the Warehouse
- Implement **role-based access control (RBAC)**
- Manage user permissions
- Secure warehouse data and queries

---

##  Errors & Troubleshooting
This repo also documents real-world issues encountered during learning, including:
- Spark notebook configuration issues

This **Errors** folder demonstrates **problem-solving and troubleshooting skills**, which are critical for data engineering role.

---

