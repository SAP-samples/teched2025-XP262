We created page variables for the sales order data, but now we need to get the data entered by the user into the respective variable. We do this by binding each page variable to their respective UI elements, specifically, to the input boxes.

Whenever someone types into the input box, the value is automatically copied into the corresponding page variable.

1. Select **User Interface**.

    ![](./Images/viewcanvas.png)

2. Using the **TREE** structure, choose on the first input field (for **Customer**).

3. In the **Properties** tab, choose the **X** next to the **Value** field

    ![Binding input field](./Images/bind-input1.png)

4. Select **Data and Variables** > **Page variable** ... 

    ![Binding input field](./Images/bind-pv2.png)

5. Select **customer**.

6. Select **Save**

    ![](./Images/bind-pv3.png)

7. Using the **TREE** structure, choose on the second input field (for **Material**).

     In the **Properties** tab, choose the **X** next to the **Value** field, and select **Data and Variables > Page Variable > material**.

8. Select **Save**

     ![](./Images/bind-pv4.png)

9. Using the **TREE** structure, choose on the third input field (for **Quantity**).

    In the **Properties** tab, choose the **X** next to the **Value** field, and select **Data and Variables > Page Variable > quantity**.

10. Select **Save**

    ![](./Images/bind-pv5.png)

11. Using the **TREE** structure, choose on the fourth input field (for **Delivery Date**).

    In the **Properties** tab, choose the **X** next to the **Value** field, and select **Data and Variables > Page Variable > date**.

12. Select **Save**

    ![](./Images/bind-pv6.png)

13. Select **Save** (upper right).

## Next step

Click here to start the next step: [Logic](../ex3-SAP_Build_Apps/2_SAP-Build_E2E_BuildApps-Workflow/5_BuildApps-Workflow.md)