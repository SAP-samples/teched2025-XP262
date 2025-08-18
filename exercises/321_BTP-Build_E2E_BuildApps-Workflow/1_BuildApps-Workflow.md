### Create an App Project

>Note that there are 2 different approaches for this tutorial step. 
>
> You can do the first approach, **Basic steps**, which will teach you about UI components, stylizing them, and organizing them on the page.
>
> Alternatively, to save time, you can do the second approach, **(Optional) Start with Template Project**, which will bypass the details of adding and stylizing components, and instead teach you how to copy an existing SAP Build Apps template project which has some of the UI components for this tutorial already built. 
>



### Basic Steps - Create New Project

First, we need to create a brand new project from the build lobby.

1. Select **[Lobby](https://xp262-tg0x69xc.eu10.build.cloud.sap/lobby)** to access the entry page of **SAP Build**.

2. In the **Lobby**, choose **Create** and **Create**.

    ![Create project](./Images/321-1_new-project-create.png)

3. Select **Application** and **Next**.

    ![Build an application](./Images/321-1_new-project-build-app.png)

4. Select **Frontend** and **Next**

    ![Build an application](./Images/321-1_new-project-build-apps.png)

5. Select **Web & Mobile Application**.

6. Select **Next**

    ![Select project type](./Images/321-1_new-project-web-project.png)

7. On the next screen, enter the following:

    | Input Field | Input Value    |
    | ----------- | -------------- |
    | Project Name   | **Create Sales Order {placeholder\|userid}**|
    | Description    | **SAP Build Apps Sales Order Project {placeholder\|userid}**|

8. Select **Review**.

    ![Name project](./Images/321-1_new-project-name.png)

- You can see the Summary.

9. Select **Create**

    ![Review](./Images/321-1_new-Review-Create.png)


>By default your new application contains a page with title and text fields. In this step, you will focus on turning this page into your app – by adding components like input boxes and buttons, and then styling them. 
This is known as creating the user interface, also known as the UI.

### Basic steps - Create UI

1. Change from **FullScreen** to **Mobile**.

    ![](./Images/UI-mobile.png)


2. Select the **text field**, and Choose the **Bin** to delete it.

    ![Delete text](./Images/UI-delete-text.png)



3. In the **Properties** tab, change the **Page name** to **Create Sales Order**.

    ![Page name](./Images/UI-page-name.png)

4. Select the title field, and in the **Properties** tab, change the **Content** text to **Sales Order Workflow**.

    ![Title](./Images/UI-title.png)

5. Drag a **Container** component from the left hand panel to your canvas. Container components let you group components and configure the collection of the components as a single unit.

    ![](./Images/dragcontainer.png)


6. With the container selected, in the **Properties** tab, change the **Component display name** to **Form**.

    ![Container](./Images/UI-container.png)

7. Still with the container selected, open the **Style** tab, Choose the dropdown icon for the **Layout Container**, and Choose **Edit**. 

    ![Container style](./Images/UI-container-style.png)

8. For background color.
    
   Select **TRANSPARENT**  and open **UNIVERSAL BACKGROUND COLORS**.
   
   Select **Level 4 background**.

    ![](./Images/level4background.png)

9. Expand the **padding** section

    ![](./Images/padding1.png)

10. Choose each rectangle **Opx**. Go to **Theme**, and select the **L** size.

    ![Padding](./Images/UI-padding.png)

11. This is what you should see.

![Opx-L](./Images/UI-Opx.png)


12. Let's save the style by scrolling up in the **Style** tab, and choose **New Style**.

    ![New style](./Images/newstyle.png)

13. Enter **Layout Form Container** Choose **OK** and **Save**

    ![](./Images/savestyle.png)

14. Drag in another container into the outer container  (Form). It may be easier to drag it into the **Tree** view on the lower right, so you can put it precisely where you want. The **Tree** makes it easier to select specific components and to create a hierarchy of components on the page.

     ![](./Images/dragcontainer2.png)

    <!--Drag two container components more from the left hand panel:-->

15. Inside the new container (Container 1), add a **text**  and an **input field**. 
    
    ![Inside container](./Images/UI-container2.png)

16. Select the new, inner container (Container1 from the Tree view)

17. Go to the **Layout** tab, and under **Layout**, set the container to **Horizontal**. 

18. Set **Align components** to the middle (*Align children vertically to the middle*).

    ![Container layout](./Images/UI-container-layout.png)

19. Select the **text** field, go to the **Layout** tab, then **Width and Height**, and set the width to exactly 75px.

    ![Text width](./Images/UI-text-width.png)

20. Select the **input field**, and in the **Properties** tab, set the **Label** property to an empty string, that is, delete the `Label` property value). 

    ![](./Images/UI-input-field.png)

21. From the **Tree** view, select the inside container ( **Container1** ).

    ![Copy](./Images/copy1.png)

22. Duplicate the container by Choosing on the **Duplicate** icon.

    ![Duplicate](./Images/copy2.1.png)

- Repeat this 2 more times, until you have 4 fields.

23. Select **Save**.

    ![Multiple fields](./Images/UI-multiple-fields.1.png)

24. Choose on each field label and change it to the following field names, in this order

    | Fields    |
    | --------- |
    | Customer  |
    | Material  |
    | Quantity  |
    | Delivery Date |

25. **Save** your work

    ![Name fields](./Images/UI-name-fields.png)

26. At the bottom of the page (outside container 4), add a button.

    ![](./Images/addbutton.png)

27. In the **Properties** tab, set the **Label** to **Get Approval**

    ![Add button](./Images/UI-button.png)

28. In the **Style** tab, next to **Primary Button**, Choose the dropdown button and select **Edit**.

    ![](./Images/buttonstyle.png)

29. For **Background color** in **SAP MORNING HORIZON CONTENT PALETTES**, select the color **Emphasized**.

    ![](./Images/buttonstyle2.png)

27. Select **Save** (upper right).

    ![](./Images/saveui.png)
