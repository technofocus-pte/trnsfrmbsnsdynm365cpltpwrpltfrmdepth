# **Lab 10: Create segments with Copilot for Customer Insights – Data**

## **Exercise 1: Add your Data**

1.  Access your **Customer Insights - Data** environment using the given
    link [**https://home.ci.ai.dynamics.com/**](urn:gd:lg:a:send-vm-keys).

**Note**: Close the pop-up – introducing Copilot in Customer Insights –
Data.

> ![](./media/image1.png)

2.  From the left navigation, select **Data** \> **Data sources**.

> ![](./media/image2.png)

2.  Select **Add a data source**.

> ![](./media/image3.png)

3.  Select **Microsoft Power Query**.

> ![](./media/image4.png)

4.  Enter [**GroceryContacts**](urn:gd:lg:a:send-vm-keys) in the **Data
    source name** for the data source and select **Next**.

> ![](./media/image5.png)

5.  On the **Choose data source** page, select **Text/CSV**.

> ![](./media/image6.png)

6.  On the **Connection settings** page, select **Upload file** and then
    select **Browse**.

> ![](./media/image7.png)

7.  Select **Grocery_Contacts.csv** from **C:\Labfiles** in your
    lab **VM**. Select **Open**.

> ![](./media/image8.png)

8.  Select **Sign in** to log in to your account.

> ![](./media/image9.png)

9.  Enter your **Office 365 admin tenant** credentials.

> ![Screenshot](./media/image10.png)

10. Select **Next**.

> ![](./media/image11.png)

11. On the **Preview file data** page, select **Transform data**.

> ![](./media/image12.png)

12. On the **Transform data** page, go to the **Transform** ribbon and
    then select the **Use first row as headers \> Use first row as
    headers** option.

> ![](./media/image13.png)

13. Right-click the **birthdate** column, go to **Change type**, and
    then select **Date**.

> ![](./media/image14.png)

14. Select the following columns by holding down the **Ctrl** key on
    your
    keyboard: **annualincome**, **msrc_creditscore**, **msrc_customerrelationshipduration**,
    and **msrc_distancetoneareststore**.

15. When these columns are highlighted, right-click one of them, go
    to **Change type**, and then select **Decimal number**.

> ![](./media/image15.png)

16. Under **Properties** on the right side, change
    the **Name** to [**contact**](urn:gd:lg:a:send-vm-keys) and then
    press the **Enter** key on your keyboard.

> ![](./media/image16.png)

17. Select **Next**.

> ![](./media/image17.png)

18. On the **Refresh settings** page, select **Refresh manually**.
    Select **Save**.

> ![](./media/image18.png)

19. Wait till the Data source is added successfully.

> ![](./media/image19.png)

20. On the **Data sources** page, select **Add a data source**.

> ![](./media/image20.png)

21. Select **Microsoft Power Query**.

> ![](./media/image21.png)

22. Enter [**GroceryTransactions**](urn:gd:lg:a:send-vm-keys) in
    the **Data source Name** for the data source and select **Next**.

> ![](./media/image22.png)

23. On the **Choose data source** page, select **Text/CSV**.

> ![](./media/image23.png)

24. On the **Connection settings** page, select **Upload file** and then
    select **Browse**.

> ![](./media/image24.png)

25. Select **Grocery_transaction.csv** from **C:\Labfiles** in your
    lab **VM**. Click **Open**.

> ![](./media/image25.png)

26. Once the file is uploaded, select **Next**.

> ![](./media/image26.png)

27. On the **Preview file data** page, select **Transform data**.

> ![](./media/image27.png)

28. As before, go to **Transform** and select **Use first row as headers
    \> Use first row as headers**.

> ![](./media/image28.png)

29. Scroll to and select the **msrc_transactiontimestamp** column.
    Right-click the column, select **Change type**, and then
    select **Date/Time**.

> ![](./media/image29.png)

30. Press and hold the **Ctrl** key on your keyboard to select
    the **msrc_transactionamount** and **msrc_discountappliedamount** columns.
    Right-click one of the columns, go to **Change type**, and then
    select **Decimal number**.

> ![](./media/image30.png)

31. Select **Next**.

> ![](./media/image31.png)

32. On the **Refresh settings** page, select **Refresh manually**.
    Select **Save**.

> ![](./media/image32.png)

33. Wait till the Data source is added successfully.

> ![](./media/image33.png)

## **Exercise 2: Unify your data**

1.  In **Customer Insights - Data**, expand **Data** in the left
    navigation pane and then select **Unify**.

> ![](./media/image34.png)

2.  Select **Get started** on the **Customer data** area.

> ![](./media/image35.png)

3.  On the **Describe the customer data to be unified** page, select
    the **Select tables and columns** button.

> **Note**: Select (…) 3 dots in the top bar if you don’t see the given
> option due to screen resolution.
>
> ![](./media/image36.png)
>
> ![](./media/image37.png)

4.  Select the **contact** and **Grocery_transaction** tables and then
    select **Apply**.

> ![](./media/image38.png)

5.  Select the **contact** table and then select **contactid** as the
    primary key.

> ![](./media/image39.png)

6.  Select the **Grocery_transaction** table and then
    select **msrc_transactionid** as the primary key. Select **Next**.

> ![](./media/image40.png)

7.  On the **Define deduplication rules** page, click **Next**.

> ![](./media/image41.png)

8.  On the **Define matching rules** page, set up the tables in the
    following order: **contact** and **Grocery_transaction**.

9.  Ensure that the **Include all records** checkbox is selected for all
    tables.

> ![](./media/image42.png)

10. Select **+ Add rule** next to the **Grocery_transaction** table.

> ![](./media/image43.png)

11. Select **contactid** and **msrc_customerid**, and then name the
    rule [**contacttransactions**](urn:gd:lg:a:send-vm-keys).
    Select **Done**.

> ![](./media/image44.png)

12. Select **Next**.

> ![](./media/image45.png)

13. Review and edit how source data is combined into unified customer
    fields on the **Unified data view** page. Click **Next**.

> ![](./media/image46.png)

14. On the **Review and create customer profiles** page, select **Create
    customer profiles**.

> ![](./media/image47.png)

15. This process will take several minutes to complete.

16. Review the **Customer data**, **Deduplication rules**, **Matching
    rules**, and **Unified data view** fields on the **Unify** page.

> ![](./media/image48.png)

## **Exercise 3: Create segments with Copilot for Customer Insights - Data (preview)**

1.  In **Customer Insights - Data**, go to **Insights** \> **Segments**.

> ![](./media/image49.png)

2.  Select + **New segment** to create a segment.

> ![](./media/image50.png)

3.  Select the Copilot icon to open the **Copilot** pane.

> ![](./media/image51.png)

4.  Enter a description of your segment or choose one of the suggested
    prompts. For example, select **Customers who have a loyalty
    membership**.

> **Note**: If Copilot gives a message that ‘Sorry, I’m having trouble
> generating insights for this segment’, then close the Copilot pane. Go
> to **Step 6**, enter the rule as shown in the image of Step 5, and
> select **Run**.
>
> ![Screenshot](./media/image52.png)

5.  Select **Use** to apply the result to a rule.

> ![Screenshot](./media/image53.png)

6.  Select **Run**.

> ![Screenshot](./media/image54.png)

7.  On the **Review details** page, enter [**Loyalty
    membership**](urn:gd:lg:a:send-vm-keys) in the **Name** field and
    then select **Run**.

> ![Screenshot](./media/image55.png)

8.  The **Loyalty membership** segment is now created.

> ![Screenshot](./media/image56.png)
>
> **Note**: If the resulting segment contains multiple [***relationship
> paths***](https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/relationships),
> it uses the shortest path by default. **Edit** the segment to change
> the relationship path.
