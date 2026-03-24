**Lab 2 - Create an Inventory Management Solution with Automated
Restocking flow**

**Objective:** In this lab, you will learn to use Copilot in Microsoft
Power Apps and Power Automate to design and implement an end-to-end
inventory management solution. You will learn to create a
Dataverse-backed canvas app for managing inventory data and to automate
inventory restocking using an approval-based workflow.

**Exercise 1: Build an Inventory Management App**

**Task 1: Create an inventory management app using Copilot.**

1.  Open a browser and go to +++\*\* sign in with Office 365 admin
    tenant credentials.

2.  Ensure that you are in **your developer** environment – **Dev One**.

> ![](./media/image1.png)

3.  Select **Apps** from the left navigation pane.

> ![](./media/image2.png)

4.  Select **+New app** \> **Start with Copilot**.

> ![](./media/image3.png)

5.  Enter the prompt below and click on the **Generate** button.

> +++**Build a candy inventory management app**+++
>
> ![](./media/image4.png)

6.  Copilot generates the tables as shown in the image below.

> ![](./media/image5.png)

7.  Select the **Inventory** table and then select **View data.**
    Observe the available columns.

> ![](./media/image6.png)

8.  Enter the given prompt in the text box and click the **send** icon.
    This column is required to notify when the quantity falls below the
    reorder point.

> +++**Add reorder point column to Inventory table**+++
>
> ![](./media/image7.png)

9.  Check if the new column has been added to the table by Copilot.

> ![](./media/image8.png)

10. Add a **candyInStock** column with the data type set to **Number**.
    If the quantity is less than the reorder point, the **Quantity**
    column will automatically be updated using **candyInStock**.

> +++ Add a candyInStock column to the Inventory table with the number
> data type+++
>
> ![](./media/image9.png)
>
> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image10.png)

11. After executing the above prompt, Copilot has generated the
    candyInStock column, but it has also changed the data type of the
    Reorder point column, stating data validation errors were found.

![](./media/image11.png)

12. Click the **drop-down** menu of the **Reorder Point** column and
    then select **Edit column**.

> ![](./media/image12.png)

13. Reselect the **Whole number** as the data type of the column and
    then click **Update**.

> ![](./media/image13.png)

14. Edit the numbers manually in the **Reorder Point** column.

> ![](./media/image14.png)

15. Close the **Copilot** pane.

![](./media/image15.png)

16. Click on the **Save and open app** button.

> ![](./media/image16.png)

17. In the **Done working?** window, click **Save and open app**, then
    wait for the app to be created.

> ![](./media/image17.png)

18. In the **welcome** window, select **Skip**.

> ![](./media/image18.png)

19. The app gets created and should look like the image below.

> ![](./media/image19.png)

20. Click the **Save** button, enter the name **Candy Inventory
    Management App**, and then click **Save** again.

> ![](./media/image20.png)

**Exercise 2: Create a Power Automate flow to restock the inventory.**

**Task 1: Create an automated flow to trigger restock email**

1.  Log in to **Power Automate** using <https://make.powerautomate.com/>
    with your Office 365 Tenant credentials. Select the **Dev One**
    environment from the environment selector.

> ![](./media/image21.png)

2.  Copy the following prompt and paste it in the Copilot field, and
    then select **Generate**.

> **Prompt:** Create a candy restock flow when a row is added or
> modified in the Dataverse table. Add a condition to check if the
> quantity is less than the reorder points. If it is less then take an
> approval to update the row
>
> ![](./media/image22.png)

3.  Based on the description, Copilot begins to create a
    suggested trigger and actions for your flow. Select **Keep it and
    continue**.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image23.png)

4.  Review your connected apps and services to X and Outlook. A green
    checkmark indicates that the connection is valid. Select **Create
    flow**.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image24.png)

5.  Select the **When a row is added or modified** step.

> ![](./media/image25.png)

6.  Select the **Change Type** as **Added or Modified** from the
    drop-down menu.

> ![](./media/image26.png)

7.  From the **Table Name** dropdown menu, search for and
    select **Inventories**.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image27.png)

8.  Remove the default selection in the **Scope** field and select
    **Organization** from the drop-down menu.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image28.png)

9.  Collapse the **When a row is added, modified or deleted** panel
    using the collapse icon on top right corner of the panel.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image29.png)

10. Select the **Condition** step.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image30.png)

11. Observe that Copilot has already added values.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image31.png)

12. But we don’t want these values, i.e., body/quantity. To correct
    that, follow the upcoming steps.

13. Select the **Choose a value** box, remove the default selection, and
    select the dynamic content icon. 

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image32.png)

14. Search for the +++Quantity+++ column and select it. 

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image33.png)

15. Similarly, remove the second default value and select the dynamic
    content icon.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image34.png)

16. Search for the +++**Reorder points**+++ column and select it. 

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image35.png)

17. Close the **Condition** pane.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image36.png)

18. Expand the **Condition** node.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image37.png)

19. Select the** Start and wait for an approval **action from the flow.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image38.png)

20. From the **Approval Type** dropdown menu, select **Approve/Reject -
    First to respond**.

> After you select the **Approval Type**, more parameters are now
> available.
>
> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image39.png)

21. Under the **Title** field, enter +++**Approve to Restock**+++ - and
    click on the dynamic content icon.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image40.png)

22. Search for +++**Candy**+++ and select **Candy (Type)**. 

> ![](./media/image41.png)

23. In the **Assigned to** field, enter MOD and select MOD Administrator
    credentials from the suggestion.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image42.png)

24. In the **Details** field, enter the given text: Select
    Candy(Type)\>from the dynamic content.

> Hi Sir,
>
> \<Candy(Type)\> is out of stock - for customers to place an order.
> Please approve to restock.
>
> Thanks
>
> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image43.png)

25. Close the **Start and wait for an approval **pane.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image44.png)

26. Select the **Condition** step.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image45.png)

27. Select the **Choose a value** box, select the dynamic content icon. 

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image46.png)

28. Select **Outcome** listed under the **Start and wait for an
    Approval** action.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image47.png)

29. Select the condition as **is equal to** and enter the value
    as **Approve**. Close the **Condition** pane.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image48.png)

30. Expand another **Condition** step and select the **Update a row**
    step under the **True** branch.

> ![](./media/image49.png)

31. Remove the default selection (if any) for the **Table name** field.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image50.png)

32. Select the **Inventories** table from the drop-down menu.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image51.png)

33. Select the **Row Id** field, remove the default selection (if any),
    and then select the dynamic content icon. 

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image52.png)

34. Search for a unique identifier column from the Inventories table and
    select it. In this case, it is **Inventory**.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image53.png)

35. Click the **Advanced Parameters** drop down and select
    the **Quantity** column. 

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image54.png)

36. Click inside the **Quantity** field and select the **Function**
    icon.

> ![](./media/image55.png)

37. Enter the below function (you type in your app) and collapse the
    action.

+++add(triggerBody()?\['cr6cd_Quantity'\],triggerBody()?\['cr6cd_candyInStock'\])+++

> **Note:** The below function does not work for you as your column
> schema name will be different. Navigate to the **Power Apps** portal,
> select **Tables** from the left pane, reach out to the Inventory table
> in the list, and note down the schema.
>
> ![](./media/image56.png)
>
> ![](./media/image57.png)

38. Close the **Update a row** pane.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image58.png)

39. Rename the flow - **Candy Restock Flow**.

> ![A screenshot of a search box AI-generated content may be
> incorrect.](./media/image59.png)

40. Save the flow by selecting the **Save** button in the upper-right
    corner of the screen.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image60.png)

41. Note that you may get an error while saving the flow. Do not
    navigate from this window till you see the message that your follow
    is saved.

42. If you get an error regarding the subscription request in the When a
    row is added, modified or deleted step, then you open the step,
    scroll down, and remove the subscription request parameter by
    selecting the X sign next to the step. Collapse the pane and again
    click save.

> ![](./media/image61.png)

43. If you still came across the error as shown in the image below, then
    try creating a new connection using the upcoming steps.

> ![](./media/image62.png)

44. Select When a row is added, modified or deleted step, scroll down
    and select Change connection reference.

> ![](./media/image63.png)

45. Select **Add new**.

> ![](./media/image64.png)

46. Enter the **Office 365 tenant credentials** for the **Connection
    name**, keep the **Authentication type** as **Oauth,** and select
    **Sign in**.

> ![](./media/image65.png)

47. Similarly, add the new connection for Start an stop approval step
    and the update a row step. Then save the flow.

> ![](./media/image66.png)

**Task 2: Test the restock flow**

1.  Switch back to the **Power Apps** tab or open it
    using **https://make.powerapps.com/**. From the left pane, select
    Apps and then open the **Candy Inventory Management App**.

> ![](./media/image67.png)

2.  Select the **Inventories** screen.

> ![](./media/image68.png)

3.  Select **+New.**

> ![](./media/image69.png)

4.  Enter the **Quantity** value **less than the reorder
    points** and **commit** changes. Enter **Inventory 3** as an
    **Inventory**.

> ![](./media/image70.png)

5.  Switch back to the **Power Automate** tab. Select the **App
    launcher** from the top-left corner.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image71.png)

6.  You should have received an email to
    restock. **Approve** and **Submit**. 

> ![](./media/image72.png)

7.  Switch back to the **Power Automate** tab. From the left pane,
    select **My flows** \> **Candy Restock Flow**.

> ![A screenshot of a computer AI-generated content may be
> incorrect.](./media/image73.png)

8.  The flow is successful now. 

> ![](./media/image74.png)

9.  Turn off the flow.

> ![](./media/image75.png)

**Summary**: In this lab, you have learnt to build an inventory
management solution using Microsoft Power Platform with Copilot
assistance. You learnt to generate a canvas app using Copilot, which
creates the required Dataverse tables for managing inventory data, and
enhanced the data model by adding and correcting columns such as Reorder
Point and candyInStock. You created an automated Power Automate flow
that monitors inventory changes and triggers a restocking approval
process when stock levels fall below the defined reorder point. The flow
sends an approval request, updates inventory quantities upon approval,
and ensures proper automation using Dataverse triggers and conditions.
