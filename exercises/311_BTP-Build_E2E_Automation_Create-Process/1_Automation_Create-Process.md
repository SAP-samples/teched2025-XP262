### Create a Business Process Project

In this section you will also create the following

- Add a Data Type 
- Create and configure API trigger

> The lobby is a central page for creating, accessing, and managing your projects in SAP Build. You can access business application processes, company configured templates, and other resources for your end-to-end business process.

Choose **[Lobby]({link|https://xp262-tg0x69xc.eu10.build.cloud.sap/lobby})** to open the entry page of **SAP Build** Process Automation.

1. In the **Lobby**, choose **Create** and then **Create**.

   ![Lobby](./Images/311-1_Automation_Create-Process-001.png)

2. Select **Automated Process** and then **Next**.

   ![Create a Project](./Images/Build_an_Automation_Process.png)

3. Select **Process** and then **Next**.

   ![Create a Business Project](./Images/Business_Process.png)

4. On the next screen, enter the following:

    | Input Field | Input Value    |
    | ----------- | -------------- |
    | Project Name   | **Sales Orders Management {placeholder\|userid}**|
    | Description    | **Sales Orders Management Project {placeholder\|userid}**|

5. Choose **Review**.


   ![Project information](./Images/Sales_Order_Management_Project.png)

   > **Note:** Make sure to use the provided naming conventions. Otherwise, you will encounter issues later on in the exercise.

6. Choose **Create**

   ![Project Creation](./Images/Sales_Order_Proj_Create.png)

7. Choose **Accept** if prompted.

   ![Accept Disclaimer](./Images/311-1_Automation_Create-Process-004_Accept-Disclaimer.png)

### Create a Business Process

A new tabs opens with the newly created project. Inside a project, you can create a process. This process is equivalent to a workflow in any business scenario. You can create this process from different skills such as forms, decisions, automations.

1. In the **Create Process** dialog box, enter the following values and choose **Create**.

    | Input Field | Input Value    |
    | ----------- | -------------- |
    | Name   | **Order Processing**|
    | Description    | **A process to handle sales orders**|

   ![Create Process](./Images/Create_Process.png)

2. If you see the below prompt, please choose **Close**.

   ![Layout Prompt](./Images/Layout_Prompt.png)

3. The following will appear

   ![Create data type](./Images/Order_Processing.png)
  
### Create a Data Type

1. Choose on **(+)** **Create** > **Data Type**.    

![Create data type](./Images/311-1_Automation_Create_Process-6.png)

2. Name the data type **Sales Order** and Choose **Create**.

   ![Add new fields](./Images/Create_Data_Type.png)
   >Close **Project Content** if needed to see the **New Field**

3. Choose **New Field** to add new fields to the data type **Sales Order** and enter the following. 

     | Field Name             | Type   |
     | ---------------------- | ------ |
     | **material**             | String |
     | **quantity**             | Number |
     | **shipToParty**          | String |
     | **salesOrderType**       | String |
     | **salesOrganisation**    | String |
     | **distributionChannel**  | String |
     | **expectedDeliveryDate** | Date   |
     | **soldToParty**          | String |

![DataType TAble](./Images/New_Field.png)

4. Choose **Save** after following all the steps for the entries above.

   > **IMPORTANT:** The spelling and casing of the fields as well as any extra spaces is crucial, because for the API to trigger the process it will require the fields exactly as written.

5. Your final data type looks as below after adding all the Field names.

   ![DataType](./Images/Final_Data_Type.png)

### Create and Configure the API trigger

1. Navigate back to your **Order Processing** page, choose **Add a Trigger**. 

   ![New API Trigger](./Images/311-1_Automation_Create-Process-7.png)

2. Choose on **API Trigger**.

   ![](./Images/311-1_Automation_CallAPI.png)

3. Enter the name as **Sales Order Trigger** and choose **Create**.

   ![CreateAPITrigger](./Images/311-1_CreateAPITrigger.png)

4. A trigger has been added to your process. Choose the **<<** icon to open the **Process Details** screen.

   ![](./Images/Process_details_open.png)

5. Choose **Variables** and then choose **Configure** (under **Process Inputs**) to configure inputs.

   ![Inputs](./Images/Process_details_new.png)

6. In the **Configure Process Inputs** window, choose **Add Input** to add parameters.

     Add the following parameter:

     | **Name**                | **Type**      | **Required** |
     | ----------------------- | ------------- | ------------ |
     | **salesorderdetails** | **Sales Order** | **true**      |



7. Choose **Apply**.

   ![Add Inputs](./Images/311-1_Automation_Create-Process-7.3.png)

8. To save the Process, choose **Save** .

   ![Save Process](./Images/311-1_Automation_Create-Process_SaveProcess.png)


