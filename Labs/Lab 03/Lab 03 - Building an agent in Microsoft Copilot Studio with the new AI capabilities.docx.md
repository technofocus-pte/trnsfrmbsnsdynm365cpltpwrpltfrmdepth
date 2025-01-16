# Lab 3: Building an agent Microsoft Copilot Studio with the new AI capabilities

In this lab, you'll create a bot by using Copilot in Microsoft Copilot
Studio. Additionally, you'll learn how to use the Conversation Booster
feature to improve your bot's responses.

1.  Sign into **Microsoft Copilot Studio** with your **Office 365 admin
    tenant** credentials
    using [**https://copilotstudio.microsoft.com/**](urn:gd:lg:a:send-vm-keys)

[**admin@M365x15683240.onmicrosoft.com**](urn:gd:lg:a:send-vm-keys)

[**Cn~R2y15%7Pju3lrGdR;(HO9Y+%^70p~**](urn:gd:lg:a:send-vm-keys)

2.  If asked, select **United States** as your country/region and then
    select **Start free trial/Get started.**

> ![](./media/image1.png)

3.  Select **Dev One** environment from environment selector.

> ![A screenshot of a computer Description automatically
> generated](./media/image2.png)

4.  On the **Welcome to Copilot Studio** pop-up, select **Skip**

> ![A screenshot of a computer Description automatically
> generated](./media/image3.png)

5.  Select **+Create** from the left navigation menu and then
    select **New agent.**

> ![A screenshot of a computer Description automatically
> generated](./media/image4.png)

6.  Select **Skip to configure**.

> ![A screenshot of a computer Description automatically
> generated](./media/image5.png)

7.  Name your agent as **Real Estate Booking Service** and then click
    on **+Add knowledge.**

> ![A screenshot of a computer Description automatically
> generated](./media/image6.png)

8.  Select **Public website**.

> ![](./media/image7.png)

9.  Under the webpage link, enter
    the [**https://powerplatform.microsoft.com/**](urn:gd:lg:a:send-vm-keys) and
    then select **Add**.

> ![A screenshot of a computer Description automatically
> generated](./media/image8.png)

10. You can see the link added under Webpage link field, now again
    select **Add**.

> ![A screenshot of a computer Description automatically
> generated](./media/image9.png)

11. Select **Create**.

> ![A screenshot of a computer Description automatically
> generated](./media/image10.png)

12. With your agent created, select **Topics** from the above horizontal
    pallet and then select the **+ Add a topic** dropdown menu.
    Select **Create from description with Copilot**.

> ![A screenshot of a computer Description automatically
> generated](./media/image11.png)
>
> **Note:** If the **Create with Copilot** option doesn't display, you
> might need to enable Intelligent authoring support:
>
> a\. Select the **Settings** icon in the upper menu and then
> select **General settings**.
>
> b\. Set the **Intelligent authoring support with Copilot** toggle
> to **On**.

13. A new window appears asking you to **Name your topic** and provide a
    description in the **Create a topic to...** space.

14. In the **Name your topic** field, enter the following text:

> [**Book a Real Estate Showing**](urn:gd:lg:a:send-vm-keys)

15. In the **Create a topic to...** field, enter the following text:

> collect a user's full name, email, address of the property, and date
> and time of the showing
>
> Select **Create**.
>
> ![](./media/image12.png)

A new topic displays with the generated trigger phrases.

> ![](./media/image13.png)

**Note:** Remember, your generated content might appear differently than
what's shown in this lab.

Multiple question nodes, entity selection, and variable naming should
also be displayed.

![](./media/image14.png)

16. Look for and then select the **What is your email
    address?** question node.

> ![](./media/image15.png)

17. Select the **’What is your email address'** question node,
    select **+Add**, and then select **Message variation**.

> ![A screenshot of a computer Description automatically
> generated](./media/image16.png)
>
> Enter **Thank you** in the message box and then select {X} icon to
> insert variable. Select **Name** variable.
>
> ![A screenshot of a computer Description automatically
> generated](./media/image17.png)

19. Select **+ sign** after the last node and select **Ask a question**
    to add one more question node.

![A screenshot of a computer Description automatically
generated](./media/image18.png)

Enter **Do you want to visit again?**, select **Multiple choice
option** under **Identity**, click on **+New option** and
enter **Yes** and **No** separately by selecting **+New option** twice.

![A screenshot of a computer Description automatically
generated](./media/image19.png)

20. Select **Save** to save your changes.

> ![A screenshot of a computer Description automatically
> generated](./media/image20.png)

21. On right side of the screen, you can see the Test your copilot pane
    is already opened. If not, click on **Test** to test the agent.

> ![](./media/image21.png)

22. When the **Conversation Start** message appears, your bot will start
    a conversation. In response, enter a trigger phrase for the topic
    that you've created:

[**I want to book a real estate showing**](urn:gd:lg:a:send-vm-keys)

[**The bot responds with the "What is your full name?" question, as
shown in the following image.**](urn:gd:lg:a:send-vm-keys)

> ![](./media/image22.png)

23. Enter the rest of the information:

> Copy
>
> Full name: \<Your name\>
>
> Email address: \<Your email address\>
>
> Address: 555 Oak Lane, Denver, CO 80203
>
> Date and Time: 10/1/2025 10:00 AM
>
> ![A screenshot of a chat Description automatically
> generated](./media/image23.png)

24. Select Yes or No.

> ![A screenshot of a chat Description automatically
> generated](./media/image24.png)

25. To test the ‘add knowledge’ property, enter What is Microsoft Power
    Platform? The bot retrieves information from the website which we
    have provided while creating an agent and returns a response.

> ![](./media/image25.png)
