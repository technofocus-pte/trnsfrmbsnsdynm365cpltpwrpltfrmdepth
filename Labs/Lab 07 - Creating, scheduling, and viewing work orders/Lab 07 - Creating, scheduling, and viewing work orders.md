# 實驗 7：在 Field Service 中使用 Copilot 在 Outlook 中創建、安排和查看工作訂單

**注：** Outlook 加載項不支持在 Outlook Web 中切換到其他主題。

## 練習 1：打開 Field Service Outlook 加載項

1.  在新選項卡中，使用鏈接打開
    **Outlook** [**http://www.outlook.com/**](urn:gd:lg:a:send-vm-keys)。

![](./media/image1.png)

2.  使用 **Office 365 管理員租戶**憑據登錄。

![](./media/image2.png)

3.  打開任何電子郵件。在電子郵件中，選擇 **Apps** 圖標。如果您沒有看到
    Apps 圖標，請選擇更多選項 （...），然後選擇 Apps。

![A screenshot of a computer Description automatically
generated](./media/image3.png)

4.  選擇 **Dynamics 365 Field Service for Outlook** 應用程序。

![A screenshot of a computer Description automatically
generated](./media/image4.png)

5.  選擇 **Sign in to get started**。

![A screenshot of a computer Description automatically
generated](./media/image5.png)

6.  選擇 **Sign-in to Dynamics 365**。

![](./media/image6.png)

7.  選擇您的 **Dynamics 365 environment**。對於此實驗室，請選擇 **Field
    Service Trial** 環境。

**注意：**如果您看到“此環境對 Field Service
無效”的警告，請暫時跳過此實驗室，並在該功能可用於此試用環境後稍後嘗試。

![A screenshot of a computer Description automatically
generated](./media/image7.png)

8.  選擇 **Get started**（開始）。

![A screenshot of a computer Description automatically
generated](./media/image8.png)

## 練習 2：在 Field Service 中使用 Copilot 在 Outlook 中創建工作訂單

1.  在電子郵件中，打開 **Field Service add-in**。

2.  在 **Home** 選項卡上，選擇 **Create a work order from email**。

![A screenshot of a computer Description automatically
generated](./media/image9.png)

3.  在 **Create work order** 頁面上，使用下表輸入要求的信息，然後選擇
    **Create**。

[TABLE]

> **注：** 對於工作訂單上的任何字段，如果下拉列表中沒有值，請選擇
> **+**。Field Service
> 應用將打開，以便您可以輸入新值及其詳細信息。保存並關閉 Field Service
> 應用。鍵入新值或選擇 **Refresh** 將新值添加到下拉列表中。
>
> ![A screenshot of a computer Description automatically
> generated](./media/image10.png)

4.  創建工作訂單後，工作訂單編號將顯示在 **Field Service**
    窗格的頂部。**System Status** （系統狀態） 默認為 **Unscheduled**
    （未計劃）。

![A screenshot of a computer Description automatically
generated](./media/image11.png)

**提示：**如果要在 Dynamics 365 Field Service
應用中打開工作訂單，請選擇彈出圖標。

![](./media/image12.png)

## 練習 3：獲取日程幫助

在 Outlook 中，計劃輔助功能可幫助您計劃、重新計劃或移動工作訂單的預訂。

### 任務 1：在 Outlook 中安排工作訂單

計劃基於資源可用性、技能、客戶承諾的時間窗口、客戶位置接近度和業務部門。

1.  在 **Field Service Add-in** 頁面上，導航到 **Work orders**
    選項卡，然後打開一個未計劃的工作訂單。

![A screenshot of a computer Description automatically
generated](./media/image13.png)

2.  在 **Work order** 頁面上，選擇 **Suggested actions** 下的
    **Schedule**。系統根據工作訂單要求搜索可用的技術人員，然後顯示建議。

![A screenshot of a computer screen Description automatically
generated](./media/image14.png)

3.  如果系統找不到建議，或者您沒有找到合適的技術人員，請改用 **Go to
    schedule board**。

![A screenshot of a computer Description automatically
generated](./media/image15.png)

4.  您將導航到 **Dynamics 365 Field Service Schedule Board**。

5.  確保您處於 **Initial public view** （初始公共視圖） 模式。選擇 Book
    預訂工作訂單。

![A screenshot of a computer Description automatically
generated](./media/image16.png)

6.  為 **Requirement** 字段選擇您的工作訂單，然後選擇 **Resource**。

7.  選擇 **Start date** （開始日期）、**Start time** （開始時間） 和
    **End date** （結束日期） 和 **End time** （結束時間）。

8.  選擇 **Book**（預訂）。工作訂單現已預訂。

![A screenshot of a computer Description automatically
generated](./media/image17.png)

9.  導航到 **Outlook** 選項卡。技術人員已預訂，工作訂單的狀態將更改為
    **Scheduled**。0

![](./media/image18.png)

10. 選擇 **View schedule** 瞭解工作訂單計劃的更多詳細信息。

![A screenshot of a computer Description automatically
generated](./media/image19.png)

### 任務 2：在 Outlook 中重新安排工作訂單

將計劃的工作訂單重新安排到其他資源、日期或時間。使用計劃輔助根據資源可用性、技能、客戶承諾的時間窗口、客戶位置接近度和業務部門提供計劃。

1.  在 **Work orders** 頁面中，打開一個計劃的工作訂單。

![](./media/image20.png)

2.  在 **Suggested actions** （建議的作） 下選擇 **View schedule**
    （查看計劃）。

![A screenshot of a phone Description automatically
generated](./media/image21.png)

3.  在計劃詳細信息頁面上，選擇 **Reschedule**（重新計劃）。

![A screenshot of a contact us Description automatically
generated](./media/image22.png)

4.  選擇 **Go to schedule board** 重新安排工作訂單。

![A screenshot of a computer Description automatically
generated](./media/image23.png)

5.  查看技術人員及其可用性。您可以按姓名搜索技術員，按日期篩選，或者按開始時間或行程時間對技術員進行排序。如果尚未在資源要求中設置
    **Estimated Duration** （估計持續時間），則默認使用 30 分鐘。

6.  重新計劃工作訂單後，**Field Service** 窗格頂部將顯示確認。

![A screenshot of a computer Description automatically
generated](./media/image24.png)

### 任務 3：在 Outlook 中移動預訂

1.  在 **Field Service Add-in** 頁面上，導航到 **Work orders**
    選項卡，然後打開計劃的工作訂單。

![](./media/image25.png)

2.  在 **Suggested actions** （建議的作） 下選擇 **View schedule**
    （查看計劃）。

![A screenshot of a computer screen Description automatically
generated](./media/image26.png)

3.  在計劃詳細信息頁面上，選擇 **Move booking**。

![A screenshot of a contact us Description automatically
generated](./media/image27.png)

4.  您可以更改當前資源。

5.  選擇日期和時間，然後選擇 **Update** （更新）。

![A screenshot of a computer Description automatically
generated](./media/image28.png)

6.  技術人員已預訂。確認將顯示在 **Field Service** 窗格的頂部。

![](./media/image29.png)

## 練習 4：在 Outlook 中查看工作訂單

1.  在電子郵件中，打開 **Field Service add-in**。

2.  在 **Work orders** 選項卡上，將顯示最多 50
    個工作訂單的列表。首先顯示最近的工作訂單。

**提示：**要在 Field Service 應用中查看更多工作訂單，請選擇列表底部的
**See more**。

![](./media/image30.png)

3.  要查找特定工作訂單，請在 **Find by ID** 框中輸入工作訂單
    ID，然後選擇 Search。

![](./media/image31.png)

4.  To filter the work orders by status or priority, select **Filter**

![A screenshot of a computer Description automatically
generated](./media/image32.png)

5.  進行選擇，例如，選擇狀態為 **Scheduled** 的工作訂單，然後選擇
    **Apply**。

![A screenshot of a login screen Description automatically
generated](./media/image33.png)

![A screenshot of a computer Description automatically
generated](./media/image34.png)

6.  要刪除篩選條件，請選擇 **Filter**（篩選），清除每個選擇，然後選擇
    **Apply**（應用）。

![A screenshot of a login form Description automatically
generated](./media/image35.png)

## 練習 5：在 Outlook 中編輯工作訂單

1.  在電子郵件中，在 **Field Service Add-in** 頁面上，導航到 **Work
    orders** 選項卡，然後打開任何工作訂單。

![A screenshot of a computer Description automatically
generated](./media/image36.png)

**提示：** 如有必要，請使用 **Find by ID** 或 **Filter** 來查找工單。

2.  進行必要的更改，例如，更改工作訂單的 **Substatus** 並選擇 **Save**
    。

![A screenshot of a phone Description automatically
generated](./media/image37.png)

3.  工作訂單已更新。確認將顯示在 **Field Service** 窗格的頂部。

![A screenshot of a phone Description automatically
generated](./media/image38.png)
