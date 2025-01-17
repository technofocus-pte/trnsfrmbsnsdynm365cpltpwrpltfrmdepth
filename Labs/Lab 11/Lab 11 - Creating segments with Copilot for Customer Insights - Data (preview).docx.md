# Lab 11: Creating segments with Copilot for Customer Insights - Data (preview)

## Exercise 1: Add your Data

1.  Access your **Customer Insights - Data** environment using the given
    link [**https://home.ci.ai.dynamics.com/**](urn:gd:lg:a:send-vm-keys).
    From the left navigation, select **Data** \> **Data sources**.

![](./media/image1.png)

Note: Close the pop up – introducing Copilot in Customer Insights –
Data.

![](./media/image2.png)

2.  Select **Add a data source**.

![](./media/image3.png)

3.  Select **Microsoft Power Query**.

4.  Enter **GroceryContacts** in the **Data source** **Name** for the
    data source and select **Next**.

![](./media/image4.png)

5.  On the **Choose data source** page select **Text/CSV**.

![](./media/image5.png)

6.  On the **Connection settings** page, select **Upload file** and then
    select **Browse**.

![](./media/image6.png)

7.  Select **Grocery_Contacts.csv** from **C:\LabFiles** in your
    lab **VM**. Select **Open**.

![](./media/image7.png)

8.  Select **Sign in**, to login to your account.

![](./media/image8.png)

9.  Enter your **Office 365 admin tenant** credentials.

![A screenshot of a computer error Description automatically
generated](./media/image9.png)

10. Select **Next**.

![A screenshot of a computer Description automatically
generated](./media/image10.png)

11. On the **Preview file data** page, select **Transform data**.

![](./media/image11.png)

12. On the **Transform data** page, go to the **Transform** ribbon and
    then select the **Use first row as headers \> Use first row as
    headers** option.

![](./media/image12.png)

13. Right-click the **birthdate** column, go to **Change type**, and
    then select **Date**.

![](./media/image13.png)

14. Select the following columns by holding down the **Ctrl** key on
    your
    keyboard: **annualincome**, **msrc_creditscore**, **msrc_customerrelationshipduration**,
    and **msrc_distancetoneareststore**.

15. When these columns are highlighted, right-click one of them, go
    to **Change type**, and then select **Decimal number**.

![](./media/image14.png)

16. Under **Properties** on the right side, change
    the **Name** to [**contact**](urn:gd:lg:a:send-vm-keys) and then
    press the **Enter** key on your keyboard.

![](./media/image15.png)

17. Select **Next**.

![](./media/image16.png)

18. On the **Refresh settings** page, select **Refresh manually**.
    Select **Save**.

![A screenshot of a computer Description automatically
generated](./media/image17.png)

19. Wait till the Data source is added successfully.

![A screenshot of a computer Description automatically
generated](./media/image18.png)

20. On the **Data sources** page, select **Add a data source**.

![A screenshot of a computer Description automatically
generated](./media/image19.png)

21. Select **Microsoft Power Query**.

22. Enter [**GroceryTransactions**](urn:gd:lg:a:send-vm-keys) in
    the **Data source Name** for the data source and select **Next**.

![A screenshot of a computer Description automatically
generated](./media/image20.png)

23. On the **Choose data source** page select **Text/CSV**.

![A screenshot of a computer Description automatically
generated](./media/image21.png)

24. On the **Connection settings** page, select **Upload file** and then
    select **Browse**.

![A screenshot of a computer Description automatically
generated](./media/image22.png)

25. Select **Grocery_transaction.csv** from **C:\LabFiles** in your
    lab **VM**. Click **Open**.

![](./media/image23.png)

26. Once the file is uploaded, select **Next**.

![A screenshot of a computer Description automatically
generated](./media/image24.png)

27. On the **Preview file data** page, select **Transform data**.

![A screenshot of a computer Description automatically
generated](./media/image25.png)

28. As before, go to **Transform** and select **Use first row as headers
    \> Use first row as headers**.

![A screenshot of a computer Description automatically
generated](./media/image26.png)

29. Scroll to and select the **msrc_transactiontimestamp** column.
    Right-click the column, select **Change type**, and then
    select **Date/Time**.

![A screenshot of a computer Description automatically
generated](./media/image27.png)

30. Press and hold the **Ctrl** key on your keyboard to select
    the **msrc_transactionamount** and **msrc_discountappliedamount** columns.
    Right-click one of the columns, go to **Change type**, and then
    select **Decimal number**.

![](./media/image28.png)

31. Select **Next**.

![](./media/image29.png)

32. On the **Refresh settings** page, select **Refresh manually**.
    Select **Save**.

![A screenshot of a computer Description automatically
generated](./media/image30.png)

33. Wait till the Data source is added successfully.

![A screenshot of a computer Description automatically
generated](./media/image31.png)

# Exercise 2: Unify your data

1.  In **Customer Insights - Data**, expand **Data** in the left
    navigation pane and then select **Unify**.

2.  Select **Get started** on the **Customer data** area.

![A screenshot of a computer Description automatically
generated](./media/image32.png)

3.  On the **Describe the customer data to be unified** page, select
    the **Select tables and columns** button.

![A screenshot of a computer Description automatically
generated](./media/image33.png)

4.  Select **contact** and **Grocery_transaction** tables and then
    select **Apply**.

![A screenshot of a computer Description automatically
generated](./media/image34.png)

5.  Select the **contact** table and then select **contactid** as the
    primary key.

![A screenshot of a computer screen Description automatically
generated](./media/image35.png)

6.  Select the **Grocery_transaction** table and then
    select **msrc_transactionid** as the primary key. Select **Next**.

![A screenshot of a computer Description automatically
generated](./media/image36.png)

7.  On the **Define deduplication rules** page, click **Next**.

![A screenshot of a computer Description automatically
generated](./media/image37.png)

8.  On the **Define matching rules** page, set up the tables in the
    following order: **contact** and **Grocery_transaction**.

9.  Ensure that the **Include all records** checkbox is selected for all
    tables.

![A screenshot of a computer Description automatically
generated](./media/image38.png)

10. Select **+ Add rule** next to the **Grocery_transaction** table.

![A screenshot of a computer Description automatically
generated](./media/image39.png)

11. Select **contactid** and **msrc_customerid**, and then name the
    rule [**contacttransactions**](urn:gd:lg:a:send-vm-keys).
    Select **Done**.

![A screenshot of a computer Description automatically
generated](./media/image40.png)

12. Select **Next**.

![A screenshot of a computer Description automatically
generated](./media/image41.png)

13. Review and edit how source data is combined into unified customer
    fields on the **Unified data view** page. Click **Next**.

![A screenshot of a computer Description automatically
generated](./media/image42.png)

14. On the **Review and create customer profiles** page, select **Create
    customer profiles**.

![A screenshot of a computer Description automatically
generated](./media/image43.png)

15. This process will take several minutes to complete.

16. Review the **Customer data**, **Deduplication rules**, **Matching
    rules**, and **Unified data view** fields on the **Unify** page.

![A screenshot of a computer Description automatically
generated](./media/image44.png)

## Exercise 3: Create segments with Copilot for Customer Insights - Data (preview)

1.  In **Customer Insights - Data**, go
    to **Insights** \> **Segments** and select + **New segment** to
    create a segment.

![A screenshot of a computer Description automatically
generated](./media/image45.png)

2.  Select the Copilot icon to open the **Copilot** pane.

![A screenshot of a computer Description automatically
generated](./media/image46.png)

3.  Enter a description of your segment or choose one of the suggested
    prompts. For example, select **Customers who have a loyalty
    membership**.

![A screenshot of a chat Description automatically
generated](./media/image47.png)

4.  Select **Use** to apply the result to a rule.

![A screenshot of a chat Description automatically
generated](./media/image48.png)

5.  Select **Run**.

![A screenshot of a computer Description automatically
generated](./media/image49.png)

6.  On the **Review details** page, enter **Loyalty membership** in
    the **Name** field and then select **Run**.

![A screenshot of a computer Description automatically
generated](./media/image50.png)

7.  The **Loyalty membership** segment is now created.

![A screenshot of a computer Description automatically
generated](./media/image51.png)

**Note**: If the resulting segment contains multiple [***relationship
paths***](https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/relationships),
it uses the shortest path by default. **Edit** the segment to change the
relationship path.
