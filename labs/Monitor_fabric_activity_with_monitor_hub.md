## The monitoring hub in Microsoft Fabric provides a central place where you can monitor activity. You can use the monitoring hub to review events related to items you have permission to view.

### STEP 1: CREATE A WORK SPACE
Before working with data in Fabric, create a workspace in a tenant with the Fabric capacity enabled.

  - Navigate to the Microsoft Fabric home page
  - In the menu bar on the left, select Workspaces.
  - Create a new workspace with a name of your choice, selecting a licensing mode in the Advanced section that includes Fabric capacity (Trial, Premium, or Fabric).

### STEP 2: CREATE A LAKEHOUSE

  - On the menu bar on the left, select Create.
  - In the New page, under the Data Engineering section, select Lakehouse.
  - Give it a unique name of your choice.

### STEP 4: CREATE AND MONITOR A DATAFLOW
**In Microsoft Fabric a Dataflow (Gen2)  is used to ingest data from a wide range of sources.**
**In this lab, we’ll use a dataflow to get data from a CSV file and load it into a table in the lakehouse.**

  - On the Home page for the lakehouse, in the **Get data** menu, select **New Dataflow Gen2.**
  - Name the new dataflow and select **Create.**
  - In the dataflow designer, select **Import from a Text/CSV file** **(Note: You can also upload a file from your local computer)**
  - Then complete the Get Data wizard to create a data connection by inserting your **Text/CSV file data link** using anonymous authentication.
  - **Publish the dataflow.** Publishing the dataflow allows the data you have injested to be loaded into your lakehouse.
      - **Note:** An Alternative method of publishing **(because the publish option has been recently removed in Fabric as at 14th-March-2026)** is to **save and run** your dataflow, from the home tab: click on **save and run** ribbon.
  - Refresh your lakehouse; in the lakehouse explore pane, expand dataflow > then table to find your file.
  -  In the navigation bar on the left, select Monitor to view the monitoring hub and observe that your dataflow is in-progress (if not, refresh the view until you see it).

### STEP 5: CREATE AND MONITOR A SPARK NOTEBOOK
In Microsoft Fabric notebooks are used to run Spark code.

  - On the menu bar on the left, select **Create**. In the New page, under the **Data Engineering section**, select **Notebook**.
  - In the notebook editor, in the Explorer pane, select **Add data items** and then select **Existing data sources**.
  - Add the lakehouse you created previously.
  - Expand the lakehouse item until you reach the products table.
  - In the … menu for the products table, select **Load data > Spark**. This adds a new code cell to the notebook as shown here:


**A new code is auto-generated, Use the ▷ Run all button to run all cells in the notebook to view the first 100 rows frm the data, this gives a snapshot of what the data is all about. It will take a moment or so to start the Spark session, and then the results of the query will be shown under the code cell.**

- #### STOP THE RUNNING SESSION: On the toolbar, use the ◻ (Stop session) button to stop the Spark session.
- In the navigation bar, select Monitor to view the monitoring hub, and note that the notebook activity is listed.


### STEP 6: MONITOR HISTORY OF AN ITEM
**Some items in a workspace might run multiple times. The monitoring Hub is use to view their run history**.
  - In the navigation bar, return to the page for your workspace. Then use the ↻ (Refresh now) button for your Get Product Data dataflow to re-run it.
  - In the navigation pane, **select the Monitor page to view the monitoring hub and verify that the dataflow is in-progress**.
  - In the … menu for the Get Product Data dataflow, select Historical runs to view the run history for the dataflow

--- 

## TO MONITOR DATA PIPELINES IN MONITORING HUB 

**Track pipeline execution and analyze activity logs.**

#### STEPS:
- Create a Data Pipeline in Fabric.
- Execute the pipeline.
- Open Monitoring Hub.
- Locate the pipeline run.
- Review execution details including:
  - Status
  - Duration
  - Logs
  - Expected Outcome

**You can observe the execution history and diagnose pipeline issues.**

