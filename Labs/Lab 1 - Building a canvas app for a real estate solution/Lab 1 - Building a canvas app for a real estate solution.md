Lab 1: Building a canvas app for a real estate solution with Copilot in
Power Apps

In this lab, you'll create a mobile application by using Copilot in
Power Apps. Field agents will use this app to browse real estate
inventory and manage appointments for showings, and the data will be
stored in Dataverse.

\*\*Note: \*\*In this lab, your results for data might vary from those
shown in the screenshots and images. The reason is because Power Apps
uses OpenAI to generate data for the lab and the data changes daily.

1.  Sign into Power
    Apps [***https://make.powerapps.com/***](urn:gd:lg:a:send-vm-keys) using
    your Office 365 tenant credentials.

2.  Ensure that you are in your developer environment - **Dev One**. If
    not, click on environment selector and select **Dev One**.

> ![Screenshot](./media/image1.png)

3.  **Disable** the **Try the new Power Apps experience** toggle switch.
    On the **Home** page in **Power Apps**, in the center text field,
    enter the following prompt to search for an AI-generated table:

> [***build an app to manage real estate
> showings***](urn:gd:lg:a:send-vm-keys)
>
> Select the **Send** button.
>
> ![Screenshot](./media/image2.png)
>
> ![Screenshot](./media/image3.png)
>
> **Note**: If pop-p appears which states that **Good data makes great
> apps** then select **Got it**.
>
> ![Screenshot](./media/image4.png)

4.  After Copilot AI generates a tables based on your prompt, look
    through the tables to view the columns that are created for the
    start of your tables.

> ![Screenshot](./media/image5.png)

5.  To see more information, click on 3 dots in front of the table name.

> ![Screenshot](./media/image5.png)
>
> Your next steps are to modify and add to the already generated table.

6.  Now click on the **Showings table** and then in the text box, in the
    lower part of the Copilot pane to the right of the screen, enter the
    following text:

> [***Add column to track client full
> name***](urn:gd:lg:a:send-vm-keys),
>
> this will add a column in the showings table. Select the Send button.
>
> ![Screenshot](./media/image6.png)

7.  Copilot notifies you that the table is updated, and the new column
    should show as being added to the showing table. (Move the slide bar
    towards right). To see the new column added to the table, click
    on **View data** from upper horizontal pane.

> ![Screenshot](./media/image7.png)
>
> ![Screenshot](./media/image8.png)

8.  Enter the following text into the chat:

> [***add a column to track client email***](urn:gd:lg:a:send-vm-keys)
>
> Select the **Send** button.
>
> A new column is added to the table and displays the client's email.
>
> ![Screenshot](./media/image9.png)
>
> **Note:** The data that's generated in your table might vary from the
> data that's shown in the table in the screenshots for this lab.

9.  Enter the below given text into the chat and select the Send button.
    A new column is added to the table and displays the client's email.

> [***Add columns to track Client Address and Agent
> Name***](urn:gd:lg:a:send-vm-keys)
>
> ![Screenshot](./media/image10.png)

10. Enter the below given text into the chat and select the Send button.
    A new column Status is added to the table and displays the client's
    email.

> [***Add a column status, data type of the column is choice (Pending,
> Completed, Confirmed, Cancelled)***](urn:gd:lg:a:send-vm-keys)
>
> ![Screenshot](./media/image11.png)

11. Select the **Status** column name dropdown menu and then
    select **Edit column**.

> ![Screenshot](./media/image12.png)

12. You can view the columns' properties and the current status details
    and data. Select the **X** in the upper-right corner of this pane to
    close it.

> ![Screenshot](./media/image13.png)

13. Close the **Copilot pane** by using **X** icon on top right corner
    of the Copilot pane.

> ![Screenshot](./media/image14.png)

14. To create the app, select the **Save and Open App** button on the
    top-right corner of the screen. Again click on **Save and Open
    App** on **Done working?** pop-up.

> ![Screenshot](./media/image15.png)
>
> ![Screenshot](./media/image16.png)

15. When the app first loads, a dialog might appear stating **Welcome to
    Power Apps Studio**. If so, select the **Skip** button.

> ![Screenshot](./media/image17.png)

16. The app that has been built for you should show in **Edit** mode.

> ![Screenshot](./media/image18.png)

17. For the better view, close the **Copliot** pane.

> ![Screenshot](./media/image19.png)

18. Select the **Data** icon from the left navigation bar. Copilot has
    created a **Dataverse** table that's now displaying in
    the **Environments** section.

> ![Screenshot](./media/image20.png)
>
> **Note:** Currently, Copilot is only supported for Dataverse. You
> can't use any other data access point at this time.
>
> Next, you'll edit the table now that the app has been created.

19. Within the **Data** pane, hover your mouse cursor over
    the **Showing** table. To the right of the table, select the
    ellipsis (...) and from the menu, select **Edit data**.

> ![Screenshot](./media/image21.png)
>
> **Note**: In the **Edit table** dialog, you can add your own columns
> to the table or modify existing columns.

20. If the **Showing** column is available in your table then select
    the **Showing** column header from the table. From the dropdown
    menu, select the **Edit column** option. If the **Showing** column
    is not available, then ignore this step and directly go to Step 22.

> ![Screenshot](./media/image22.png)

21. In this example, you don't want the **Data type** to be a **Single
    line of text**. To change that value, go to the **Edit
    column** pane, and then from the **Date type** dropdown menu,
    select **\# Autonumber**. Select **Save**.

> ![Screenshot](./media/image23.png)

22. Select the **Close** button in the lower-right corner of the **Edit
    table** dialog.

> ![Screenshot](./media/image24.png)

23. The table should now show as **Refreshed** in the **Data** pane, if
    you make changes in **Showing** column.

> ![Screenshot](./media/image25.png)

24. Modify the gallery in the application so that it displays the
    relevant data. Select the **Tree view** icon to return to the **Tree
    view**.

> ![Screenshot](./media/image26.png)

25. Under **Showings screen**, select **RecordsGallery3** to display
    Showings. To select **RecordsGallery3** follow the below given
    hierarchy. Note that, the Gallery, Title & Body may not be the same
    number as on the instructions.

> (Select **Showings
> Screen** \> **ScreenContainer3** \> **BodyContainer3** \> **SidebarContainer3** \> **RecordsGallery3**).
>
> ![Screenshot](./media/image27.png)

26. Now select the **edit** button of the **RecordsGallery3** to put the
    gallery in edit mode.

> ![Screenshot](./media/image28.png)

27. In the **Tree view**, expand **RecordGallery3**, select
    the **Title3** and then set the Text value to the following formula:

> [***ThisItem.'Client Address'***](urn:gd:lg:a:send-vm-keys)
>
> ![Screenshot](./media/image29.png)

28. Select the **Subtitle3** and then set the **Text** value to the
    following formula:

> [***ThisItem.'Client Email'***](urn:gd:lg:a:send-vm-keys)
>
> ![Screenshot](./media/image30.png)

29. Select the **Body2** and then set the **Text** value to the given
    formula. Enter **ThisItem.Status** and then from the suggestions
    select, **ThisItem.'Status (cr56c_status)'** in this case.

> **Note:** In the above formula, cra55 value can be different in your
> case
>
> ![Screenshot](./media/image31.png)
>
> A single record in the gallery should now resemble the following
> image.
>
> ![Screenshot](./media/image32.png)

30. From the **Tree view**, select
    the **Form3** from **RightContainer3** \> **MainContainer3** \> **Form
    3**. Hover the mouse over **Form3** on the canvas and then
    select **Fields**. Click on (...) next to **Showing** column and
    select **Remove**.

> **Note:** If you don’t see Showing ID or Showings field then ignore
> this step.
>
> ![Screenshot](./media/image33.png)
>
> Because you previously changed the **ID** field to **Autonumber**, you
> don't want users entering their own number; Dataverse automatically
> enters the numbers for you.

31. Make a new request for a property that shows in the app by selecting
    the **Play** button from the upper part of the screen.

> ![Screenshot](./media/image34.png)

32. In the left pane, select the **+ New** button.

> ![Screenshot](./media/image35.png)

33. Fill in the fields with the following information.Ignore the extra
    information.

    - Client Name: [***John***](urn:gd:lg:a:send-vm-keys)

    - Client Full Name: [***John Almeda***](urn:gd:lg:a:send-vm-keys)

    - Date: December 5, 2024

    - Time: 15:00

    - Agent Name: [***Sarah Connor***](urn:gd:lg:a:send-vm-keys)

    - Feedback: [***The property is impressive, but the kitchen needs
      minor upgrades.***](urn:gd:lg:a:send-vm-keys)

    - Client
      Email: [***john.almeda@example.com***](urn:gd:lg:a:send-vm-keys)

    - Client Address: [***210 Pine Road, Portland, OR
      97204***](urn:gd:lg:a:send-vm-keys)

    - Status: Pending

    - Property: Luxury Villa

> ![Screenshot](./media/image36.png)

34. Select the check mark in the upper-right corner of the screen.

> ![Screenshot](./media/image37.png)

35. Select the **X** in the upper-right corner to close out of the app.

> ![Screenshot](./media/image38.png)
>
> If a dialog appears saying **Did you know?**, select **OK**.
>
> ![Screenshot](./media/image39.png)
>
> The new request is added to the left of the list of requests.

36. From the upper part of your screen, select the **Save** button to
    save the new app that you created. If the system prompts you, save
    the app name as [***Real Estate
    Showings***](urn:gd:lg:a:send-vm-keys).

> ![Screenshot](./media/image40.png)

37. Exit the app to return to the Power Apps home page.
