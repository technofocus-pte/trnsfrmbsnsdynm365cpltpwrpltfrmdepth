Lab 2: Automating the approval process for a real estate showing using
Copilot

In this lab, you'll create an automation by using Copilot in Power
Automate to automate the approval process for a real estate showing.
You'll use Copilot to create a flow that sends an email to the real
estate agent when a new showing is requested. Then, the agent can
approve or reject the showing request from within the email.

Follow these steps to create a flow by using Copilot.

1.  Sign into Power Automate
    using [***https://make.powerautomate.com/***](urn:gd:lg:a:send-vm-keys) with
    you Office 365 tenant credentials.

2.  If asked, select **United States** as country/region and then click
    on **Get started**.

> ![Screenshot](./media/image1.png)

3.  Click on **environment selector** and select **Dev
    One** environment.

> ![Screenshot](./media/image2.png)

4.  In the center of the Home page within Power Automate, in the text
    field on Let’s automate something. What should it do? enter the
    following prompt: [***When a dataverse row is added, created,
    deleted or modified, start and wait for the approval process
    approval and update the row accordingly based on the approval
    outcome.***](urn:gd:lg:a:send-vm-keys) Select
    the **Generate** button.

> ![Screenshot](./media/image3.png)

5.  From the prompt, Copilot provides the outline for a suggested flow
    that you can review. To accept the flow, select **Keep it and
    continue**.

> ![Screenshot](./media/image4.png)

6.  Review the connected apps and services. If a connection hasn't been
    made, edit or fix it and then select **Create flow**.

> ![Screenshot](./media/image5.png)
>
> The Edit with Copilot designer opens with your flow along with a
> Copilot chat window on the right.
>
> ![Screenshot](./media/image6.png)

7.  Set up some parameters by selecting the **When a row is added,
    modified or deleted** trigger.

> A panel on the left side of the screen shows the trigger details,
> including an empty **Table Name** parameter that's required.
>
> ![Screenshot](./media/image7.png)

8.  From the **Table Name** dropdown menu, search for and
    select **Showings**.

> **Note:** Select the table that got generated in lab1.
>
> ![Screenshot](./media/image8.png)

9.  Collapse the **When a row is added, modified or deleted** panel
    using collapse icon on top right corner of the panel

> ![Screenshot](./media/image9.png)

10. Select the **Start and wait for an approval** action from the flow

> Notice that the **Approval Type** parameter is missing.
>
> **Note**: If you see an error that says ‘Failed to retrieve dynamic
> input’, then click on the cross icon to clear the **Approval
> type** field.
>
> ![Screenshot](./media/image10.png)

11. From the **Approval Type** dropdown menu, select **Approve/Reject -
    First to respond**.

> After you select the **Approval Type**, more parameters are now
> available.
>
> ![Screenshot](./media/image11.png)

12. Under the **Title** field, enter [***New Request for
    Showing***](urn:gd:lg:a:send-vm-keys).

> **Note**: Use the name of the table that we are ingesting data from.
> If lab 1 has generated some other table use the name of that table.
>
> ![Screenshot](./media/image12.png)

13. For the **Assigned To** parameter, enter the Office 365 tenant
    credentials that you're using for this lab. This email address is
    the one that receives the approval request.

> ![Screenshot](./media/image13.png)

14. For the Details parameter, enter the following text:

> [***A new request for a real estate showing has been created. Please
> review the details below and approve or reject the
> request:***](urn:gd:lg:a:send-vm-keys)
>
> [***Property:***](urn:gd:lg:a:send-vm-keys)
>
> [***Client:***](urn:gd:lg:a:send-vm-keys)
>
> [***Client Email:***](urn:gd:lg:a:send-vm-keys)
>
> [***Date:***](urn:gd:lg:a:send-vm-keys)
>
> ![Screenshot](./media/image14.png)

15. Place your curser next to **Property:** in the **Details** parameter
    and then select the lightning icon to open the **Dynamic
    content** pane.

> ![Screenshot](./media/image15.png)

16. In the **Dynamic content** pane, select **See More** of the step
    'When a row is added, modified or deleted' to expand the list of
    available dynamic content.

> ![Screenshot](./media/image16.png)

17. Scroll down until you find the **Client** **Address** field and then
    select **Add**.

> ![Screenshot](./media/image17.png)
>
> The **Address** dynamic content field is now added to
> the **Details** parameter.
>
> ![Screenshot](./media/image18.png)

18. Complete the same steps for the Client Full Name, Client Email and
    Showing Date fields.

> When you're done with the rest of the fields, the values should
> resemble the following image.
>
> ![Screenshot](./media/image19.png)

19. With the **Details** parameter completed, you can collapse
    the **Start and wait for an approval** action by selecting the
    double arrow icon.

> ![Screenshot](./media/image20.png)

20. Select the **Condition** action.

> ![Screenshot](./media/image21.png)

21. Select the **Choose a value** box and then select **Outcome** from
    the **Dynamic content** pane.

> ![Screenshot](./media/image22.png)

22. Select **is equal to** for the condition and then
    enter **Approve** for **Value**.

> ![Screenshot](./media/image23.png)

23. Collapse the **Condition** action.

> ![Screenshot](./media/image24.png)

24. Select the **Update a row** action under the **True** branch of the
    condition.

> ![Screenshot](./media/image25.png)

25. From the **Table Name** dropdown menu, search for and
    select **Showings**.

> **Note**: If you see an error - Failed to retrieve the dynamic inputs
> then select **cross icon** to clear the value under the **Table
> name** field.
>
> ![Screenshot](./media/image26.png)
>
> ![Screenshot](./media/image27.png)

26. Select the **Row ID** field, delete the exixting
    content **YourROWID** and select **Dynamic content** and then
    select **see more** infront of the **When a row is added, modified
    or deleted**.

27. Now, select the **Showings** unique identifier field from
    the **Dynamic content** pane and click on **Add**.

> ![Screenshot](./media/image28.png)
>
> Whenever you create a table in Microsoft Dataverse, a column is
> automatically created with the same name of the table. This column
> serves as the unique lookup ID for the record (or row) that was
> created.

28. Select **Show all** under **Advanced parameters**.

> ![Screenshot](./media/image29.png)

29. Select **Confirmed** from the **Status** dropdown menu.

> When a showing is approved, the **Status field** in the **Showings
> table** is updated to **Confirmed**.
>
> ![Screenshot](./media/image30.png)

30. Collapse the **Update a row** action.

> ![Screenshot](./media/image31.png)

31. Select the **Update a row** action under the **False** branch of the
    condition.

> ![Screenshot](./media/image32.png)

32. From the **Table Name** dropdown menu, search for and
    select **Showings**.

> **Note**: If you see an error - Failed to retrieve the dynamic inputs
> then select cross icon to clear the value under the **Table
> name** field.
>
> ![Screenshot](./media/image33.png)

33. Select the **Row ID** field and delete the exixting
    content **YourROWID** then select **Showings** unique identifier
    field from the **Dynamic content** pane and click on **Add**.

> ![Screenshot](./media/image34.png)

34. Select **Show all** under **Advanced parameters**.

> ![Screenshot](./media/image35.png)

35. Select **Cancelled** from the **Status** dropdown menu.

> When a showing is rejected, the **Status** field in
> the **Showings** table is updated to **Cancelled**. .
>
> ![Screenshot](./media/image36.png)

36. Collapse the **Update a row** action.

> ![Screenshot](./media/image37.png)

37. In the Copilot chat window, enter the following prompt and then
    submit:

> [***Under the "Update a row" action for both branches in the
> condition, add a new "Send an email (V2)"
> action***](urn:gd:lg:a:send-vm-keys)
>
> **Important**: Sometimes Copilot fails to create a step. In case
> Copilot fails then create a step manually by selecting **+
> icon** under **Update a row** and then in the **Add an action** pane
> which opens on left side, enter **Send an email** in the search box
> and select **Send an email (V2)** action from **Office 365 Outlook**.
> After creating this step, you will be asked to create connection.
> Select **Sign in**. In case, if you see connection error in the step
> created by Copilot then at the bottom of the **Send an
> email(V2)** action pane, select **Change connection**, select
> given **admin tenant** id to create a connection.
>
> ![Screenshot](./media/image38.png)
>
> After a few seconds, Copilot should explain what it did, as shown in
> the following image.
>
> ![Screenshot](./media/image39.png)

38. Select the **Send an email** action under the **True** branch of the
    condition.

> ![Screenshot](./media/image40.png)

39. Select **Switch to advanced** mode in the line of **To** field. In
    the **To** field, select the **Client Email** dynamic content.
    (Select see more in front of the When a row is added, modified or
    deleted)

> ![Screenshot](./media/image41.png)

40. For the **Subject** field, enter the following text:

> [***Your request for a real estate showing has been
> approved***](urn:gd:lg:a:send-vm-keys)
>
> ![Screenshot](./media/image42.png)

41. For the **Body** field, enter the following text:

> [***Good day - Your request for a real estate showing has been
> approved. Please see below for details.***](urn:gd:lg:a:send-vm-keys)
>
> ![Screenshot](./media/image43.png)

42. Enter the following content after the **Body** text:

> [***Property:***](urn:gd:lg:a:send-vm-keys)
>
> [***Agent Name:***](urn:gd:lg:a:send-vm-keys)
>
> [***Showing Date:***](urn:gd:lg:a:send-vm-keys)
>
> Add the **Client** **Address**, **Agent
> Name** and **Showing** **Date** fields from the **Dynamic
> content** pane to the appropriate lines in the **Body** text.
>
> ![Screenshot](./media/image44.png)

43. Add the **Response summary** field from the **Dynamic content** pane
    to the end of the **Body** text.

> ![Screenshot](./media/image45.png)

44. Collapse the **Send an email** action.

> ![Screenshot](./media/image46.png)

45. Select the **Send an email** action under the **False** branch of
    the condition. Select the **To** field, remove
    the example@example.com email address, and then select the **Client
    Email** field from the **Dynamic content** pane.

> ![Screenshot](./media/image47.png)

46. For the **Subject** field, enter the following text:

> [***Your request for a real estate showing has been
> rejected***](urn:gd:lg:a:send-vm-keys)
>
> ![Screenshot](./media/image48.png)

47. For the **Body** field, enter the following text:

> [***Good day - Your request for a real estate showing has been
> rejected. Please see below for details.***](urn:gd:lg:a:send-vm-keys)
>
> ![Screenshot](./media/image49.png)

48. Enter the following content after the **Body** text:

> [***Property:***](urn:gd:lg:a:send-vm-keys)
>
> [***Agent Name:***](urn:gd:lg:a:send-vm-keys)
>
> [***Showing Date:***](urn:gd:lg:a:send-vm-keys)
>
> Add the **Address**, **Agent Name** and **Showing** **Date** fields
> from the **Dynamic content** pane to the appropriate lines in
> the **Body** text.
>
> ![Screenshot](./media/image50.png)

49. Add the **Response summary** field from the **Dynamic content** pane
    to the end of the **Body** text.

> ![Screenshot](./media/image51.png)

50. Collapse the **Send an email** action.

51. Rename the flow to [***Request Approval for Real Estate
    Showing***](urn:gd:lg:a:send-vm-keys) by selecting the **request
    approval when a Dataverse record is created** text in the upper-left
    corner of the screen.

> ![Screenshot](./media/image52.png)

52. Save the flow by selecting the **Save** button in the upper-right
    corner of the screen.

> ![Screenshot](./media/image53.png)

53. Select **back arrow** before the name of the flow.

> ![Screenshot](./media/image54.png)

54. Select **OK**.

> ![Screenshot](./media/image55.png)

55. To submit a real estate showing request, go to the Real Estate
    Showings app in Power Apps
    using [***https://make.powerapps.com/***](urn:gd:lg:a:send-vm-keys) .

56. Select **Apps** from left navigation, select **Real Estate
    Showings** app and then select **Play**.

> ![Screenshot](./media/image56.png)

57. Select **Showings** screen then select **+
    New** on **Showing** screen to create a new showing request.

> ![Screenshot](./media/image57.png)

58. Fill in the fields with the following information:

    - Client Name: [***Summer***](urn:gd:lg:a:send-vm-keys)

    - Date: February 25, 2025

    - Time: 15:00

    - Agent Name: [***Bruce Banner***](urn:gd:lg:a:send-vm-keys)

    - Feedback: [***The property is impressive, but the kitchen needs
      minor upgrades.***](urn:gd:lg:a:send-vm-keys)

    - Client Full Name: [***Summer Scott***](urn:gd:lg:a:send-vm-keys)

    - Client Email: Enter the given Admin tenant id which is used for
      this lab

    - Client Address: [***350 Alps Road, Portland, OR
      97254***](urn:gd:lg:a:send-vm-keys)

    - Status: Pending

    - Property: Luxury Villa

> ![Screenshot](./media/image58.png)

59. Select the check mark in the upper-right corner of the screen.

> ![Screenshot](./media/image59.png)
>
> The flow runs and sends an approval email to the email address that
> you provided in the flow that you built.

60. Sign in to the Admin email account that you're using for this lab
    and then wait for the email to arrive. To sign in to email,
    select **App launcher** from the top left corner of the **Powers
    Apps/Power Automate** portal and then select **Outlook**.

> **Note:** If the flow doesn't run immediately, make sure that you wait
> for it. It might take up to 10 minutes for the flow to be triggered,
> especially on the first try.
>
> The approval should resemble the following image.
>
> ![Screenshot](./media/image60.png)

61. Select **Approve**.

> ![Screenshot](./media/image61.png)

62. Add a comment and then select **Submit**.

> ![Screenshot](./media/image62.png)
>
> The flow continues to run; it updates the row and sends an email to
> the requestor. The email that's sent to the requester resembles the
> following image.
>
> ![Screenshot](./media/image63.png)

63. Check the flow and notice that the flow is now marked
    as **Succeeded** in the run history.

> ![Screenshot](./media/image64.png)
>
> ![Screenshot](./media/image65.png)
