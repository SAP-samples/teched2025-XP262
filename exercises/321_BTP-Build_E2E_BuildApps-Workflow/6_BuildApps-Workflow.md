1. Select **Preview**.

    ![Launch](./Images/launch.png)

2. Select **Open web preview**.

    ![](./Images/open_preview.png)


3. Select your project, **Create Sales Order {placeholder|userid}**.

    ![Launch preview](./Images/launch-preview.png)

4. Enter the following values in your form:

    | Field | Value |
    |-------|-------|
    | Customer | {placeholder\|userid} Bikes |
    | Material | MZ-FG-C900 |
    | Quantity  | 1200 |
    | Delivery Date  | 2024-12-01 |

5. Select **Get Approval**.

Your process should be triggered and require approval (since the quantity figure is above 10).

You should see the toast message indicating the workflow was triggered, and with the process instance ID.

![Preview toast](./Images/launch-toast.png)

You can also see the results of the call in the **[SAP Build]({link|buildlobby})** Monitor.

6. Go to the **Monitoring** tab, then **Process and Workflow Instances**. 

![Preview Monitor](./Images/monitor_workflow.png)

The first process listed should be the one you just triggered.

- You can see the new process instance.
- You can see the process ID is the same as in the toast message in the app.
- You can see the context, which is the values sent with the API (four of them, in yellow, you entered in the input fields and the others were hardcoded in the formula for the **Create record** flow function).
- You can also see the execution log, which shows that the process stopped at the approval step (because the quantity was at least 10), and is awaiting approval. If you expand the approval step, you can see more information, including who the approval request was sent to.

![Preview in process automation](./Images/launch-preview-SPA.png)


