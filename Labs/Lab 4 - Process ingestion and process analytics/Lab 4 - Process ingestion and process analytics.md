Lab 4: Process ingestion and process analytics with Copilot in Process
Mining (preview)

## Exercise 1 - Process ingestion with Copilot in Process Mining

1.  Navigate to the **Power Automate** portal
    using [***https://make.powerautomate.com/***](urn:gd:lg:a:send-vm-keys).
    Click on environment selector and select **Dev One** environment.

> ![Screenshot](./media/image1.png)

2.  From the left navigation, select **Process mining** and then
    select **Start here** under **Create new process**.

> ![Screenshot](./media/image2.png)

3.  In the **Process name** field, enter a name [***Process
    contacts***](urn:gd:lg:a:send-vm-keys) for your process.

4.  Select **Import Data** under **Data source**.

5.  Select **Dataflow**.

6.  Select **Continue**.

> ![Screenshot](./media/image3.png)

7.  Under **Connect to your data**, choose **Text/CSV**.

> ![Screenshot](./media/image4.png)

8.  Under **Connection settings** area, select **Upload file** and then
    click **Browse.**

> ![Screenshot](./media/image5.png)

9.  Open the **Grocery_Contacts.csv** file from **C:\LabFiles** in your
    lab VM. After uploading file, if you see that connection is created
    automatically as shown in first screenshot below then go to the next
    step. If connection is not created, then scroll down and
    select **Sign in** as shown in second screenshot below and sign in
    with your admin tenant credentials.

> **Note:** Ensure that you don’t select ‘Ask a chatbot’ while selecting
> ‘Next’ button.
>
> ![Screenshot](./media/image6.png)
>
> ![Screenshot](./media/image7.png)

10. Once the file is uploaded, select **Next**.

> ![Screenshot](./media/image8.png)

11. Select **Next** on the **Preview file data** page.

> ![Screenshot](./media/image9.png)

12. Select **Next** on the **Transform your data** page.

> ![Screenshot](./media/image10.png)

13. On the **Map your data** page, for below attributes, map the column
    of attribute type correctly to set up your process map. Then,
    select **Save and analyze**.

> **contactid**: CaseID
>
> **genderCode**: Activity
>
> **birthdate**: Event Start
>
> **Note**: Case ID, Activity, and Event start are required.
>
> ![Screenshot](./media/image11.png)

14. Wait for the report to be prepared.

> ![Screenshot](./media/image12.png)

15. Once the report is prepared, you would be able to explore the
    report. Navigate through the **Summary**, **Map** and **Variant
    DNA** tabs.

> ![Screenshot](./media/image13.png)
>
> ![Screenshot](./media/image14.png)
>
> ![Screenshot](./media/image15.png)
>
> ![Screenshot](./media/image16.png)

Exercise 2 - Process analytics with Copilot in Process Mining

1.  In process map view, select **Copilot** on the command bar to the
    right. The Copilot pane opens.

2.  Copilot offers several prepared suggestions to easily get you
    started on engaging with your data.

> ![Screenshot](./media/image17.png)

3.  From the provided suggestions, select **Summarize my process**.

> ![Screenshot](./media/image18.png)

4.  Copilot provides the response to your query.

> ![Screenshot](./media/image19.png)

5.  If available, it also provides subsequent prepared suggestions.

> ![Screenshot](./media/image20.png)

6.  (Optional) You can continue in conversation with Copilot by
    selecting subsequent suggestions. Alternatively, you can ask your
    own questions at any time using the text field in bottom part of the
    Copilot pane.
