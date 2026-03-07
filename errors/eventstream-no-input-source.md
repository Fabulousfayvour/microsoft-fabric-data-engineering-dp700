# Troubleshooting: Eventstream "No Input Source Connected" Error

## Issue

While configuring an Eventstream pipeline in Microsoft Fabric, the destination node displayed the following error:

"No input source is connected"

This prevented the Eventstream from publishing successfully.

## Cause

The destination node (bikes-table) was not connected to the upstream event stream.

Current pipeline:

Bicycles → Bicycle-data-stream     bikes-table 

The destination requires a valid input connection.


<img width="676" height="483" alt="blurred publish" src="https://github.com/user-attachments/assets/d1a23c73-5d2a-4820-a660-e935e792961b" />

## Solution

Connect the stream output to the destination.

Correct pipeline:

Bicycles → Bicycle-data-stream → bikes-table

Steps:

1. Drag the connector from **Bicycle-data-stream**
2. Connect it to **bikes-table**
3. Configure the destination table
4. Click **Publish**

## Result

After connecting the nodes and publishing the Eventstream, the pipeline executed successfully and streaming data was stored in the Eventhouse table.


<img width="738" height="470" alt="published sorted" src="https://github.com/user-attachments/assets/7c61b3c9-c3ae-455f-935a-c9b81ae236c0" />

