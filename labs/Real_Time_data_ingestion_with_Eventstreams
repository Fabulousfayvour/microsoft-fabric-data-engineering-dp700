 ##  Objective

Create an Eventstream in Microsoft Fabric to ingest streaming data and store it in Eventhouse for real-time analytics.

#### **Step 1: Create a Fabric Workspace**
- Open Microsoft Fabric portal.
- Click Workspaces.
- Select New Workspace.
Enter: Workspace Name: RealTimeAnalytics-Lab
Description: Fabric Real-Time Data Analytics Lab

- Click Create.

#### **Step 2: Create an Eventstream**

- Inside the workspace, click New Item.

- Select Eventstream.
Enter: Name: IoT-Streaming-Events
- Click Create.

The Eventstream canvas opens where streaming sources and destinations are configured.

#### **Step 3: Connect a Streaming Data Source**

- In the Eventstream canvas, click Add Source.

- Select one of the following sources:

  - Azure Event Hub

  - Sample streaming data

  - Custom application

- Choose Sample streaming data for the lab.
Configure: Source Name: SampleDeviceData
- Click Add.

The Eventstream now begins receiving simulated streaming events.

#### **Step 4: Apply Event Transformations**

Event transformations allow you to filter, aggregate, or enrich streaming data before storage.
- Select the source node in the Eventstream.
- Click Add Transformation.
- Choose Filter Transformation.

Configure a rule such as: Temperature > 30

This filters events where temperature readings exceed 30 degrees.
- Save the transformation.

**Step 5: Store Streaming Data in Eventhouse**

- Click Add Destination.
- Select Eventhouse (KQL Database).

Configure: Eventhouse Name: StreamingEventhouse

Database Name: IoTDatabase

Table Name: TemperatureEvents

- Click Save.

**The streaming data is now stored in Eventhouse for real-time analytics.**
