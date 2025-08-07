In this lesson, you’ll configure **filtering**, **ordering** and **paging** for both the **Get Record Collection** logic node and the **A_SalesOrder** data variable. This improves performance and ensures only the most relevant data is retrieved.

>Note: Since this is a live SAP S/4HANA OData service, it may return a large volume of Sales Orders.
To ensure optimal performance and relevant results, you will retrieve only the latest entries.

## Get Record Collection Logic Node

1. In the logic flow, select the **Get Record Collection** node to open its properties.

   ![](./Images/Add_Filter1.png)

### Filtering

2. Under **Filter condition**, select the **X** icon, then choose **Object with properties**.

   ![](./Images/Add_Filter2.png)

3. Select **ADD CONDITION**: 
  * **Property:** **SalesOrganization**
  * **Condition Type: equal**
  * **Compared value: 1710** 
  
  
4. Select **ADD CONDITION**: 
  * **Property:** **SalesOrderType**
  * **Condition Type: equal**
  * **Compared value: OR** 

 Click **SAVE**.

   ![](./Images/Add_Filter3.png)

### Ordering

5. Under **Ordering**, select the **X** icon, then choose **List of values**.

   ![](./Images/Add_Filter4.png)

6. Select **ADD SORT OPTION**:

  * **Property: SalesOrder**
  * **Order: descending**
  This ensures the most recent Sales Orders appear first.

Click **SAVE**. 

   ![](./Images/Add_Filter5.png)

### Paging

7. Under **Paging**, select the **X** icon, then choose **Object with properties**.

   ![](./Images/Add_Filter6.png)

8. Here we will set two mandatory values: 

* **Page size**
* **Include total count**

   ![](./Images/Add_Filter7.png)

9. Under **Page size**, select the **X** icon, then choose **Static Number**.

   ![](./Images/Add_Filter8.png)

10. Enter **10** as the page size. This will fetch only 10 records at a time.

   ![](./Images/Add_Filter9.png)

11. Under **Include total count**, select the **X** icon, then choose **Static true/false**.

   ![](./Images/Add_Filter10.png)

12. Set the value to **false**, then click **SAVE** to confirm both paging settings.

   ![](./Images/Add_Filter11.png)

13. **Save** your work. Now close the logic screen by clicking on downward arrow.

   ![](./Images/Add_Filter12.png)

## A_SalesOrder Data Variable

1. Go to **Variables > DATA VARIABLES > A_SalesOrder**. To the right of the screen are the properties for this data variable.

   ![](./Images/Add_Filter13.png)

### Filtering

2. Under **Filter condition**, select the **X** icon, then choose **Object with properties**.

   ![](./Images/Add_Filter2b.png)

3. Select **ADD CONDITION**: 
  * **Property:** **SalesOrganization**
  * **Condition Type: equal**
  * **Compared value: 1710** 
  
  
4. Select **ADD CONDITION**: 
  * **Property:** **SalesOrderType**
  * **Condition Type: equal**
  * **Compared value: OR** 

 Click **SAVE**.

   ![](./Images/Add_Filter3b.png)   

### Ordering

5. Under **Ordering**, select the **X** icon, then choose **List of values**.

   ![](./Images/Add_Filter14.png)

6. Select **ADD SORT OPTION**:

  * **Property: SalesOrder**
  * **Order: descending**
  This ensures the most recent Sales Orders appear first.

Click **SAVE**. 

   ![](./Images/Add_Filter15.png)

### Paging

7. Under **Paging**, select the **X** icon, then choose **Object with properties**.

   ![](./Images/Add_Filter16.png)

8. Here we will set two mandatory values: 

* **Page size**
* **Include total count**

   ![](./Images/Add_Filter17.png)

9. Under **Page size**, select the **X** icon, then choose **Static Number**.

   ![](./Images/Add_Filter18.png)

10. Enter **10** to limit the results to 10 records per query

   ![](./Images/Add_Filter19.png)

11. For **Include total count**, select the **X** icon, then choose **Static true/false**.

   ![](./Images/Add_Filter20.png)

12. Set the value to **false**, then click **SAVE** to confirm both paging settings.

   ![](./Images/Add_Filter21.png)

13. **Save** your work. Select the **User Interface** tab..

   ![](./Images/Add_Filter22.png)

