1. On your **Create Sales Order** page, go back to UI canvas by selecting **User Interface**.

    ![](./Images/view_ui.png)

    >You can close the logic pane if it interferes with your work.

2. Drag a **Dropdown field** next to the input box for the **Material**.

    ![Add dropdown](./Images/dropdown-add.png)

    - It should look like this.

    ![Result](./Images/dropdown-add-result.png)

3. Choose the dropdown box. Take note of the **Label text**, **Option list** and **Selected value** properties because you are about to change them.

    ![Dropdown properties](./Images/dropdown-properties.png)

4. Set the **Label text** property to an empty string, that is, delete `Dropdown label` value.

5. For the **Option list** property, choose the **list of values** icon **[ ]**.

   Then set the binding to a **formula**, and set the formula to the following:<div>&nbsp;</div>`MAP(data.A_ProductDescription1, {label: item.Product+ " (" + item.ProductDescription +") "  ,value: item.Product})`
   
6. Choose **Save**.

7. The **Dropdown field** properties should now look like:

    ![](./Images/dropdown-properties1.png)

8. You will have to bind the dropdown field to the **material** page variable (as we did for the input field for material).

    For the **Selected value** field, set the binding to: **Data and variables > Page variable > material**. 

    Choose **Save**

    ![](./Images/dropdown-properties2.png)

    The **Dropdown field** properties should now look like:

    ![Selected value](./Images/dropdown-selected-value.png)

9. Choose **Save** (upper right).


## Next step

Click here to start the next step: [Preview](../ex3-SAP_Build_Apps/3_SAP-Build_E2E_BuildApps-Populate-Data/4_BuildApps-Populate-Data.md)