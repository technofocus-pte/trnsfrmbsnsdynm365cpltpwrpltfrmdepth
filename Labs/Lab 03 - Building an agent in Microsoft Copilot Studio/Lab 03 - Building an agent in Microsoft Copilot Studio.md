# 實驗 3：使用新的 AI 功能在 Microsoft Copilot Studio 中構建機器人

在本實驗中，您將使用 Microsoft Copilot Studio 中的 Copilot
創建機器人。此外，您還將學習如何使用 Conversation Booster
功能來改進機器人的響應。

1.  使用 [**https://copilotstudio.microsoft.com/**](urn:gd:lg:a:send-vm-keys)
    使用您的 **Office 365 管理員租戶**憑據登錄 **Microsoft Copilot
    Studio**

[**admin@M365x15683240.onmicrosoft.com**](urn:gd:lg:a:send-vm-keys)

[**Cn~R2y15%7Pju3lrGdR;(HO9Y+%^70p~**](urn:gd:lg:a:send-vm-keys)

2.  如果詢問，請選擇 **United States**
    作為您的國家/地區，然後選擇**Start free trial/Get started。**

![](./media/image1.png)

3.  從環境選擇器中選擇 **Dev One** 環境。

![A screenshot of a computer Description automatically
generated](./media/image2.png)

4.  在 “**Welcome to Copilot Studio**” 彈出窗口中，選擇 “**Skip**” 

![A screenshot of a computer Description automatically
generated](./media/image3.png)

5.  從左側導航菜單中選擇 **+Create**，然後選擇 **New agent**。

> ![A screenshot of a computer Description automatically
> generated](./media/image4.png)

此時將打開 Create a bot
嚮導。此嚮導通過命名、選擇語言以及選擇是否要使用生成式答案來促進對話，從而幫助您設置機器人。

6.  選擇 **Skip to configure**。

> ![A screenshot of a computer Description automatically
> generated](./media/image5.png)

7.  將您的機器人命名為 **Real Estate Booking Service**，然後單擊 **+Add
    knowledge**。

![A screenshot of a computer Description automatically
generated](./media/image6.png)

8.  選擇 **Public website** （公共網站）。

> ![](./media/image7.png)

![A screenshot of a computer Description automatically
generated](./media/image8.png)

**注意：**選擇 **Create** （創建） 後，在新環境中創建第一個 bot
的過程最多可能需要 15 分鐘。後續機器人的創建速度要快得多。

9.  在網頁鏈接下，輸入 [**https://powerplatform.microsoft.com/**](urn:gd:lg:a:send-vm-keys) 然後選擇
    “**Add**” 。

> ![A screenshot of a computer Description automatically
> generated](./media/image9.png)

![A screenshot of a computer Description automatically
generated](./media/image10.png)

10. 您可以在 Webpage link 字段下看到添加的鏈接，現在再次選擇 **Add**。

> ![A screenshot of a computer Description automatically
> generated](./media/image11.png)

![A screenshot of a computer Description automatically
generated](./media/image12.png)

11. 選擇 **Create**。

![A screenshot of a computer Description automatically
generated](./media/image13.png)

12. 創建代理後，從上面的水平模塊中選擇 **Topics** ，然後選擇 **+ Add a
    topic** 下拉菜單。選擇 **Create from description with Copilot**。

> ![A screenshot of a computer Description automatically
> generated](./media/image14.png)

![A screenshot of a computer Description automatically
generated](./media/image15.png)

**注意：**如果未顯示**Create with
Copilot**選項，則可能需要啟用智能創作支持：

a\. 選擇上方菜單中的 **Settings** 圖標，然後選擇 **General settings**。

b\. 將 **Intelligent authoring support with Copilot** 開關設置為
**On**。

13. 此時將出現一個新窗口，要求您為 **Name your topic** ，並在 **Create a
    topic to ...**空間。

14. 在 **Name your topic** （命名您的主題） 字段中，輸入以下文本：

[**Book a Real Estate Showing**](urn:gd:lg:a:send-vm-keys)

15. 在 **Create a topic to...**字段中，輸入以下文本：

collect a user's full name, email, address of the property, and date and
time of the showing

選擇 **Create**。

![A screenshot of a computer Description automatically
generated](./media/image16.png)

![](./media/image17.png)

此時將顯示一個新主題，其中包含生成的觸發短語。

![](./media/image18.png)

![A screenshot of a computer Description automatically
generated](./media/image19.png)

**注意：**請記住，您生成的內容可能與本實驗中顯示的內容不同。

還應顯示多個問題節點、實體選擇和變量命名。

![](./media/image20.png)

![A screenshot of a computer Description automatically
generated](./media/image21.png)

16. 查找並選擇 **What is your email address？**question 節點。

> ![](./media/image22.png)

![A screenshot of a computer Description automatically
generated](./media/image23.png)

17. 選擇創作畫布上部的 **Edit with Copilot** 圖標。

![A screenshot of a computer Description automatically
generated](./media/image24.png)

18. 選擇 “**What is your email address**（您的電子郵件地址是什麼）”
    問題節點，選擇 **+Add**（+添加），然後選擇 **Message
    variation**（消息變體）。

![A screenshot of a computer Description automatically
generated](./media/image25.png)

在消息框中輸入 **Thank you**，然後選擇 {X} 圖標以插入變量。選擇 **Name**
variable（名稱變量）。

![A screenshot of a computer Description automatically
generated](./media/image26.png)

19. 在最後一個節點後選擇 **+ sign** 以再添加一個問題節點。

![A screenshot of a computer Description automatically
generated](./media/image27.png)

輸入 **Do you want to visit again？**，選擇 **Identity** 下的 **Multiple
choice option** ，單擊 **+New option**，然後選擇 **+New option**
兩次，分別輸入 **Yes** 和 **No**。

![A screenshot of a computer Description automatically
generated](./media/image28.png)

20. 選擇 **Save** （保存） 以保存更改。

![A screenshot of a computer Description automatically
generated](./media/image29.png)

21. 在屏幕右側，您可以看到 “測試您的 Copilot” 窗格已打開。

![A screenshot of a computer Description automatically
generated](./media/image30.png)

22. 當 **Conversation Start** （對話開始）
    消息出現時，您的機器人將開始對話。作為響應，輸入您創建的主題的觸發短語：

[**I want to book a real estate showing**](urn:gd:lg:a:send-vm-keys)

[**The bot responds with the "What is your full name?" question, as
shown in the following image.**](urn:gd:lg:a:send-vm-keys)

![A screenshot of a chat Description automatically
generated](./media/image31.png)

23. 輸入其餘信息：

> 複製
>
> 全名：\<您的姓名\>
>
> 電子郵件地址：\<您的電子郵件地址\>
>
> 聯繫地址： 555 Oak Lane, Denver, CO 80203
>
> 日期和時間： 10/10/2023 10:00 AM

![A screenshot of a chat Description automatically
generated](./media/image32.png)

24. 選擇 Yes （是） 或 No （否）。

![A screenshot of a chat Description automatically
generated](./media/image33.png)

25. 要測試增強的機器人，請輸入 What is Microsoft Power
    Platform？機器人從我們在創建機器人時提供的網站中檢索信息並返回響應。

![A screenshot of a computer Description automatically
generated](./media/image34.png)
