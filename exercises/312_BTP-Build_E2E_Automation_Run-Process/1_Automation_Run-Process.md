### Release the Business Process Project.

To run the process, you have to first release and then deploy the business process project.

Releasing a project creates a version or snapshot of the changes, and deploying the project makes it available in runtime to be consumed. You can only deploy a released version of the project.

1. In the Process Builder, to release a project, Choose**Release** button on the top-right corner of the screen and provide a description in the popup dialog.

   ![released](./Images/312-1_Automation_Run-Process-1.png)

   > Every time you release, a new version will be created. The version is incremented automatically based on how you want to store the changes in the repository like major or minor update or just as a patch.

   If you are releasing for the first time, then the version will start with **1.0.0**. Next time you release, the version numbers will be automatically updated.

2. Choose the **Release** button.

   ![Release](./Images/312-1_Automation_Run-Process-2.png)

### Deploy the Released Project.

1. Once the project is released successfully, choose the **Deploy** button on the top-right corner of the screen.

   ![Deploy](./Images/312-1_Deploy-1.png)

   **Note**: If you do not see the **Deploy** option you may ned to manually change from the **Editable** to the **Released** version of your project:
   ![](./Images/editable-released.png)

2. Select the **Public** environment and Choose **Deploy**.

   ![Deploy](./Images/312-1_Deploy-2.png)

3. Choose **Deploy**.

   ![Deploy](./Images/312-1_Deploy-3.png)

4. Select the destination **S4HANA_CLOUD_CPI** from the drop down and Choose **Deploy**.

   ![Deploy](./Images/312-1_Deploy-4.png)

   > **S4HANA_CLOUD_CPI** refers to a BTP destination that leverages an SAP Integration Suite integration flow (iFlow) to post Sales Order data to the SAP S/4HANA Cloud tenant. The iFlow utilizes an OData ABAP API to manage the creation of Sales Orders in S/4HANA Cloud. This process aligns with the principles of a "clean core" approach, ensuring minimal customizations and preserving the standard capabilities of the S/4HANA Cloud system.

5. Once the deployment is successful, you will see a changed status.

   ![Deploy](./Images/312-1_Deploy-5.png)

   > You cannot edit released or deployed projects. To continue working on your project, you need to select the Editable version of your project (at the top of the page).

### Publish to the SAP Build Library.

1. After you have released and deployed the process, go to the SAP Build Lobby and find your project (i.e. **Sales Orders Management {placeholder\|userid}**).

2. Once you have found the process with at least one available version, Choose the **Navigate** arrow on the right.

   ![Navigate](./Images/312-1_Library-1.png)

3. Select the **Versions** tab, locate your **Deployed** version, and select the **Publish to Library** icon.

   ![Publish](./Images/312-1_Library-2.png)

4. Select the version (you may use the most recent version - if several versions are available) and choose the **Publish** button. Afterwards, your process is ready to run.

   ![Publish](./Images/312-1_Library-3.png)

You have successfully released, deployed, and published your process. Now, your process will be visible from other SAP Build products in the SAP Build Library section. It is time to test the process and see the results.


