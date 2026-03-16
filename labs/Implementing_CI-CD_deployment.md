## To implement deployment pipeline in Macrosoft Fabric; below are the steps to achieve it.

### **STEP 1:** CREATE WORKSPACES
Create workspaces for development, testing and deployment:
   - Development workspace
   - Test workspace
   - Deployment

### **STEP 2:**  CREATE A DEPLOYMENT PIPELINE
A pipeline is used to manage your workspace content through the deployment stages continously delivering the latest content to the userrs.
This will be craeted with three different stages automatically.

Now, create a deployment pipeline.
  - In the menu bar on the left, select Workspaces.
  - Select Deployment Pipelines, then New pipeline.
  - In the Add a new deployment pipeline window, give the pipeline a unique name and select Next.
  - In the new pipeline window, select Create and continue.

### **STEP 3:** ASSIGN WORKSPACE TO THE SATGES OF THE DEPLOYMENT PIPELINE
Assign a workspace on each deploymwnt stage and select a workspace that matches the name of the stages, then assign for each deployment stage.

  - On the left menu bar, select the pipeline you created.
  - In the window that appears, expand the options under Assign a workspace on each deployment stage and select the name of the workspace that matches the name of the stage.
  - Select the check mark Assign for each deployment stage.


### STAGE 4: CREATE CONTENT
Create an intem in your workspace. This can be created in the **Development** workspace:

Fabric items haven’t been created in your workspaces yet. Next, create a lakehouse in the development workspace.

  - In the menu bar on the left, select Workspaces.
  - Select the Development workspace.
  - Select New Item.
  - In the window that appears, select Lakehouse and in the New lakehouse window, name the lakehouse, LabLakehouse. Make sure the “Lakehouse schemas (Public Preview)” option is disabled.
  - Select Create.
  - In the Lakehouse Explorer window, select Start with sample data to populate the new lakehouse with data.
   - Populate the lakehouse with a sample data

### STEP 5: DEPLOY CONTENT BETWEEN STAGES

Deploy the craeted lakehouse from the **Development* stage to the **Test** and **Production** stages.
This is because the item craeted in development workspace is only a stage item in the source, which in this case refers to the development stage and are not synchronized with other stages.
Deploy the **lakehouse from the Development stage to the Test and Production stages.**

  - Select the **Test** stage in the deployment pipeline canvas.
  - Under the deployment pipeline canvas, select the checkbox next to the Lakehouse item. Then select the **Deploy** button to copy the lakehouse in its current state to the Test stage.
  - In the Deploy to next stage window that appears, **select Deploy**. There is now an X in a circle in the Production stage in the deployment pipeline canvas. The lakehouse exists in the Development and Test stages but not yet in the Production stage.
  - Select the **Production** stage in the deployment canvas.
  - Under the **deployment pipeline** canvas, select the checkbox next to the Lakehouse item. Then select the Deploy button to copy the lakehouse in its current state to the Production stage.
  - In the Deploy to next stage window that appears, **select Deploy**. The green check marks between the stages indicates that all stages in sync and contain the same content.
  - Using deployment pipelines to deploy between stages also updates the content in the workspaces corresponding to the deployment stage. Let’s confirm.
  - In the menu bar on the left, select **Workspaces.**
  - Select the **Test** workspace. The lakehouse was copied there.
  - Open the **Production** workspace from the Workspaces icon on the left menu. The lakehouse was copied to the Production workspace too.



