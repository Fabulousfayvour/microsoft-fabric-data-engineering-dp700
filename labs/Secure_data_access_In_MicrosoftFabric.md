## SECURE DATA ACCESS IN MICROSFT FABRIC
### Microsoft Fabric has a multi-layer security model for managing data access. Security can be set for an entire workspace, for individual items, or through granular permissions in each Fabric engine. 
**In this lab, I will describe how to secure data using workspace, and item access controls and OneLake data access roles.**


---

### Configure Workspace Permissions
**This is done to assign roles to users in a Fabric workspace.**

#### Steps:
- Open a Fabric Workspace.
- Navigate to Access Settings.
- Add a user.
- Assign a role:
  - Admin
  - Member
  - Contributor
  - Viewer
- Save the changes.

**Expected Outcome:** **Users gain appropriate access based on assigned roles.**


---
### Apply Item-Level Permissions
**You can restrict access to a specific Fabric artifact, to enable users have access to only item(s) that is needed to get their wprk done.**

#### Steps:
- Select a Lakehouse or dataset.
- Open Manage Permissions.
- Assign specific users access.
- Define permission levels.

**Expected Outcome: Only authorized users can access the selected artifact.**
