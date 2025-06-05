Lab 8: Creating and deploying an agent-facing copilot with Microsoft
Copilot for Service

Exercise 1: Create an Agent copilot

You can create an Agent copilot in a few easy steps.

1.  Go to the sign-up page
    using [***https://go.microsoft.com/fwlink/?linkid=2252259***](urn:gd:lg:a:send-vm-keys).

2.  Select **Continue**.

> ![Screenshot](./media/image1.png)

3.  Select **United States** as Country/region, enter your **phone
    number**, job title (if asked) and select **Get started**.

> ![Screenshot](./media/image2.png)
>
> **Note**: If the get you’ve selected DO NOT USE Microsoft Copilot for
> Service Preview, continue and click on Get started.

4.  Select **Get started**.

> ![Screenshot](./media/image3.png)

5.  From the environment selector, select **Contoso
    (default)** environment and if the screen appears and asks to start
    with Microsoft Copilot or create a custom copilot then click
    on **Create a custom copilot** and then select **Get started**.

> ![Screenshot](./media/image4.png)

6.  Give the name as **Agent Copilot**, select **Choose an
    environment**, select **Customer Service trial** and then
    select **Next**. If you dont see to choose an environment then keep
    the default entries as is and select **Next**.

> ![Screenshot](./media/image5.png)

7.  Under **Choose a customer engagement service**, select **I don’t
    want to set this up right now** and then select **Create**.

> **Note**: Ignore the error that says "Failed to create an
> environment".
>
> ![Screenshot](./media/image6.png)

8.  Navigate to the **Content sources** page.

> ![Screenshot](./media/image7.png)

9.  Under **Websites**, paste the given website
    - [***https://www.microsoft.com/en-in/power-platform***](urn:gd:lg:a:send-vm-keys) and
    then select **Add**.

> ![Screenshot](./media/image8.png)

10. Select **Save** at the top.

> ![Screenshot](./media/image9.png)

11. In the **Test Copilot** section, type [***What is Power
    Platform***](urn:gd:lg:a:send-vm-keys). Then, select **Send** icon.

> ![Screenshot](./media/image10.png)

12. You can see the response given by **Copilot**.

> ![Screenshot](./media/image11.png)

Exercise 2: Publish in Copilot for Service

1.  Navigate to the main **Overview** page of **Copilot for Service**.

> ![Screenshot](./media/image12.png)

2.  In the **Publish your changes** card on the **Overview** page,
    select **Publish**.

> ![Screenshot](./media/image13.png)

It may take a few minutes for the copilot to publish. Once published
successfully, the status indicator shows the last published timestamp.

Exercise 3: Connect your bot to the Microsoft Teams channel

1.  In the **Give access to customer service representatives** card,
    select **Connect to Teams**.

> ![Screenshot](./media/image14.png)

2.  You will be navigated to **Microsoft Copilot Studio**. If asked,
    sign in with your **Office 365 Admin Tenant** credentials.
    Select **United States** as **country/region** and then select **Get
    Started**. If you are navigated to Agent page as shown in the second
    image then select **Create**. Skip this step, if you see your
    A**gent Copilot** is already created.

> ![Screenshot](./media/image15.png)
>
> ![Screenshot](./media/image16.png)

3.  On Microsoft Copilot Studio portal, select **Channels** tab,
    select **Microsoft Teams** and then select **Add Channel**.

> ![Screenshot](./media/image17.png)
>
> ![Screenshot](./media/image18.png)
>
> **Note:** If you do not see this option, then the Microsoft Teams
> channel may already be enabled.

4.  Select **Edit details** to change the bot's icon, color, and
    descriptions.

> These will be shown in the **Microsoft Teams app store** and the
> app's **About** tab after the user installs the agent.
>
> ![Screenshot](./media/image19.png)

5.  Change the short description to **Test bot** then select **Save**.

> ![Screenshot](./media/image20.png)

6.  Select **See agent in Teams** to have the installation prompt launch
    in Microsoft Teams.

> ![Screenshot](./media/image21.png)

7.  Select **Cancel on Open Microsoft Teams (work or school)?** Pop-up
    window.

> ![Screenshot](./media/image22.png)

8.  Select **Use the web app instead**.

> ![Screenshot](./media/image23.png)

9.  Select **Add** to have it added as an app in Teams. This only
    installs the agent for you. select Open on the screen which appears
    after adding copilot to teams as shown in the second image below.

> ![Screenshot](./media/image24.png)
>
> ![Screenshot](./media/image25.png)

10. Enter [***What is Power Platform***](urn:gd:lg:a:send-vm-keys) in
    the Type a message box and click on **Send** icon.

> ![Screenshot](./media/image26.png)

11. You can see the given response from **Agent copilot**.

> ![Screenshot](./media/image27.png)
