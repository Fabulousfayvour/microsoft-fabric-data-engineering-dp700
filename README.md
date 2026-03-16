# Microsoft Fabric Data Engineering (DP-700) Learning Repository

##  Overview
This repository documents my hands-on learning journey in **Microsoft Fabric Data Engineering (DP-700)**, focusing on modern lakehouse architecture, data ingestion, transformation, analytics, and orchestration using Microsoft Fabric.

The goal of this repo is to demonstrate practical implementation of **enterprise-grade data engineering concepts** using Microsoft Fabric, Delta Lake, Apache Spark, and Medallion architecture.

---

## Learning Path
- Microsoft Certified: Azure Data Fundamentals (DP-900) ✅ Completed https://github.com/Fabulousfayvour/azure-data-fundamentals-dp900
- Microsoft Certified: Fabric Data Engineer Associate (DP-700)  ✅ Completed

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


---

## Managing a Fabric Environment

Continuous Integration and Continuous Delivery (CI/CD)
Monitoring Fabric Activities
Securing Data Access
Administering a Fabric Environment

### Implement Continuous Integration and Continuous Delivery (CI/CD) in Microsoft Fabric

##### Overview:
Continuous Integration and Continuous Delivery (CI/CD) ensures that data solutions are developed, tested, and deployed efficiently and consistently.

In Microsoft Fabric, CI/CD is implemented using:

- Git Integration
- Version Control
- Deployment Pipelines
- Fabric APIs

These tools allow teams to collaborate on Fabric assets like Lakehouses, Notebooks, Pipelines, and Warehouses while maintaining version control and automated deployments.

### Key Concepts
#### **Continuous Integration (CI)**

Continuous Integration is the process of automatically integrating code changes from multiple developers into a shared repository.

##### Benefits include:
- Early detection of errors
- Improved collaboration
- Consistent development environments

#### **Continuous Delivery (CD)**

Continuous Delivery ensures that validated changes can be deployed automatically to production environments.
This reduces manual deployment errors and speeds up delivery.

How CI/CD Works in Microsoft Fabric
**Fabric supports CI/CD through:** Git Integration

Fabric workspaces can be connected to Git repositories (GitHub or Azure DevOps) to track changes in:
Notebooks, Data pipelines, Lakehouses, Warehouses, Reports
This allows version history and collaborative development.

##### Deployment Pipelines

**Deployment pipelines** allow you to promote changes across environments: Development, Test, Production.
Pipelines ensure consistent deployment of Fabric artifacts.

**Fabric APIs**
Fabric APIs enable automation of CI/CD workflows, allowing DevOps pipelines to deploy Fabric items programmatically.

---

## Monitor Activities in Microsoft Fabric

**Overview:**
Monitoring is essential for ensuring system reliability, performance, and operational health.

Microsoft Fabric provides monitoring tools that allow administrators and engineers to track activities across the platform.

**Key monitoring tools include:**
- Monitoring Hub
- Microsoft Fabric Activator

 #### Monitoring Concepts

**Monitoring helps organizations:** Track job execution, detect failures, measure system performance, trigger alerts and automated responses.

#### Monitoring Hub in Microsoft Fabric
The Monitoring Hub provides a centralized dashboard for monitoring: Data pipeline runs, notebook executions, Spark jobs, Data refresh activities

**Features include:**
i. Activity history
ii. Job status tracking
iii. Performance insights

#### Microsoft Fabric Activator

Microsoft Fabric Activator enables real-time data monitoring.
It allows users to define conditions or patterns in streaming data and automatically trigger actions such as:
i. Alerts
ii. Notifications
iii. Workflow automation

---

## Secure Data Access in Microsoft Fabric
**Overview:**

Security in Microsoft Fabric is implemented using a multi-layer security model that protects data at multiple levels.

**Security is enforced through:**
i. Workspace permissions
ii. Item-level permissions
iii. Granular access control
iv. Fabric Permissions Model

Fabric uses role-based access control (RBAC).
Common workspace roles include:
i. Admin
ii. Member
iii. Contributor
iv. Viewer

Each role defines the level of access to workspace resources.

#### Workspace Permissions

Workspace permissions determine who can access or manage resources within a workspace.

Examples:

Admin can manage settings and users.

Contributors can create and modify artifacts.

Item-Level Permissions

Item-level permissions allow administrators to control access to specific resources, such as:
i. Lakehouses
ii. Warehouses
iii. Reports
iv. Notebooks

#### Granular Security Controls

Granular security enables fine-grained access control such as:
- Row-level security
- Column-level security
- Dataset permissions

This ensures users only see data relevant to them.

---

## Administer a Microsoft Fabric Environment
**Overview**

Microsoft Fabric is a Software-as-a-Service (SaaS) analytics platform that integrates data engineering, data science, and business intelligence into a unified environment.

**Fabric administrators are responsible for:**

i. Configuring platform features
ii. Managing user access
iii. Enforcing governance policies
iv. Monitoring usage and capacity
v. Fabric Administration Tasks


The Admin Center provides centralized management tools for administrators.

**It allows admins to:**
- Manage tenant settings
- Configure capacity
- Monitor usage
- Control feature access
- Managing User Access


**Administrators can control access to Fabric resources by:**
- Assigning roles
- Managing permissions
- Restricting workspace creation
This ensures proper governance across the organization.

#### Data Governance in Fabric
**Data governance ensures that data is:**
- Secure
- Compliant
- Properly managed

**Fabric governance features include:**

- Data lineage
- Access auditing
- Sensitivity labels
- Policy enforcement

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

### Managing a microsoft fabric environment

####  Implement continuous integration and continuous delivery (CI/CD) in Microsoft Fabric
- Define CI/CD and describe how it's implemented in Fabric.
- Implement version control and Git integration.
- Use deployment pipelines to automate the deployment process.

#### Monitor activities in Microsoft Fabric
- Apply monitoring concepts to Microsoft Fabric
- Use Monitoring Hub in Microsoft Fabric 
- Trigger actions using Activator in Microsoft Fabric

#### Administer a Microsoft Fabric environment
Microsoft Fabric is a SaaS solution for end-to-end data analytics. As an administrator, you can configure features and manage access to suit your organization's needs.

---

##  Errors & Troubleshooting
This repo also documents real-world issues encountered during learning, including:
- Spark notebook configuration issues

The **Errors** folder demonstrates **problem-solving and troubleshooting skills**, which are critical for data engineering role. https://github.com/Fabulousfayvour/microsoft-fabric-data-engineering-dp700/tree/main/errors

---

