# 實驗 11：使用 Copilot for Customer Insights 創建細分 - 數據（預覽）

## 練習 1：添加數據

1.  使用給定的鏈接 [**https://home.ci.ai.dynamics.com/**](urn:gd:lg:a:send-vm-keys)訪問您的
    **Customer Insights - Data** 環境。 從左側導航欄中，選擇 **Data \>
    Data sources**。

![](./media/image1.png)

注意：關閉彈出窗口 – 在 Customer Insights – 數據中引入 Copilot。

![](./media/image2.png)

2.  選擇 **Add a data source**（添加數據源）。

![](./media/image3.png)

3.  選擇 **Microsoft Power Query**。

4.  在數據源的 **Data source Name** 中輸入 **GroceryContacts**，然後選擇
    **Next**。

![](./media/image4.png)

5.  在 **Choose data source** 頁面上，選擇 **Text/CSV**。

![](./media/image5.png)

6.  在 **Connection settings** （連接設置） 頁面上，選擇 **Upload file**
    （上傳文件），然後選擇 **Browse** （瀏覽）。

![](./media/image6.png)

7.  從實驗室 **VM** 的 **C：\LabFiles** 中選擇
    **Grocery_Contacts.csv**。選擇 “**Open**” 。

![](./media/image7.png)

8.  選擇 **Sign in**（登錄），以登錄您的帳戶。

![](./media/image8.png)

9.  輸入您的 **Office 365 管理員租戶**憑據。

![A screenshot of a computer error Description automatically
generated](./media/image9.png)

10. 選擇 **Next**（下一步）。

![A screenshot of a computer Description automatically
generated](./media/image10.png)

11. 在 **Preview file data** （預覽文件數據） 頁面上，選擇 **Transform
    data** （轉換數據）。

![](./media/image11.png)

12. 在 **Transform data** 頁面上，轉到 **Transform** 功能區，然後選擇
    **Use first row as headers \> Use first row as headers** 選項。

![](./media/image12.png)

13. 右鍵單擊 **birthdate** 列，轉到 **Change type**
    （更改類型），然後選擇 **Date** （日期）。

![](./media/image13.png)

14. 按住鍵盤上的 **Ctrl**
    鍵選擇以下列： **annualincome**, **msrc_creditscore**, **msrc_customerrelationshipduration**,
    和**msrc_distancetoneareststore**.

15. 突出顯示這些列時，右鍵單擊其中一列，轉到 **Change type**
    （更改類型），然後選擇 **Decimal number** （十進制數）。

![](./media/image14.png)

16. 在右側的 **Properties** 下，將 **Name**
    更改為 [**contact**](urn:gd:lg:a:send-vm-keys)，然後按 **Enter**
    鍵盤上的鍵。

![](./media/image15.png)

17. 選擇 **Next**（下一步）。

![](./media/image16.png)

18. 在 **Refresh settings** （刷新設置） 頁面上，選擇 **Refresh
    manually** （手動刷新）。選擇 **Save** （保存）。

![A screenshot of a computer Description automatically
generated](./media/image17.png)

19. 等待 Data source 添加成功。

![A screenshot of a computer Description automatically
generated](./media/image18.png)

20. 在 **Data sources** （數據源） 頁面上，選擇 **Add a data source**
    （添加數據源）。

![A screenshot of a computer Description automatically
generated](./media/image19.png)

21. 選擇 **Microsoft Power Query**。

22. 在數據源的 **Data source Name**
    中輸入 **GroceryTransactions**，然後選擇**Next**。

![A screenshot of a computer Description automatically
generated](./media/image20.png)

23. 在 **Choose data source** 頁面上，選擇 **Text/CSV**。

![A screenshot of a computer Description automatically
generated](./media/image21.png)

24. 在 **Connection settings** （連接設置） 頁面上，選擇 **Upload file**
    （上傳文件），然後選擇 **Browse** （瀏覽）。

![A screenshot of a computer Description automatically
generated](./media/image22.png)

25. 從實驗室 **VM** 的 **C：\LabFiles** 中選擇
    **Grocery_transaction.csv**。單擊 **Open**。

![](./media/image23.png)

26. 上傳文件後，選擇 **Next**。

![A screenshot of a computer Description automatically
generated](./media/image24.png)

27. 在 **Preview file data** （預覽文件數據） 頁面上，選擇 **Transform
    data** （轉換數據）。

![A screenshot of a computer Description automatically
generated](./media/image25.png)

28. 與以前一樣，轉到 **Transform** 並選擇 **Use first row as headers \>
    Use first row as headers**。

![A screenshot of a computer Description automatically
generated](./media/image26.png)

29. 滾動並選擇 **msrc_transactiontimestamp** 列。右鍵單擊該列，選擇
    **Change type** （更改類型），然後選擇 **Date/Time（**日期/時間）。

![A screenshot of a computer Description automatically
generated](./media/image27.png)

30. 按住鍵盤上的 **Ctrl** 鍵以選擇 **msrc_transactionamount** 和
    **msrc_discountappliedamount** 列。右鍵單擊其中一列，轉到 **Change
    type** （更改類型），然後選擇 **Decimal number** （十進制數）。

![](./media/image28.png)

31. 選擇 **Next**（下一步）。

![](./media/image29.png)

32. 在 **Refresh settings** （刷新設置） 頁面上，選擇 **Refresh
    manually** （手動刷新）。選擇 **Save** （保存）。

![A screenshot of a computer Description automatically
generated](./media/image30.png)

33. 等待 Data source 添加成功。

![A screenshot of a computer Description automatically
generated](./media/image31.png)

# 練習 2：統一數據

1.  在 **Customer Insights - Data** 中，展開左側導航窗格中的
    **Data**，然後選擇 **Unify**。

2.  在 **Customer data** （客戶數據） 區域選擇 **Get started**
    （開始）。

![A screenshot of a computer Description automatically
generated](./media/image32.png)

3.  在 **Describe the customer data to be unified** 頁面上，選擇
    **Select tables and columns** 按鈕。

![A screenshot of a computer Description automatically
generated](./media/image33.png)

4.  選擇 **contact** 和 **Grocery_transaction** 表，然後選擇 **Apply**。

![A screenshot of a computer Description automatically
generated](./media/image34.png)

5.  選擇 **contact** 表，然後選擇 **contactid** 作為主鍵。

![A screenshot of a computer screen Description automatically
generated](./media/image35.png)

6.  選擇 **Grocery_transaction** 表，然後選擇 **msrc_transactionid**
    作為主鍵。選擇 **Next**（下一步）。

![A screenshot of a computer Description automatically
generated](./media/image36.png)

7.  在 **Define deduplication rules** 頁面上，單擊 **Next**。

![A screenshot of a computer Description automatically
generated](./media/image37.png)

8.  在 **Define matching rules** 頁面上，按以下順序設置表：**contact**
    和 **Grocery_transaction**。

9.  確保為所有表選中 **Include all records** 複選框。

![A screenshot of a computer Description automatically
generated](./media/image38.png)

10. 選擇 **Grocery_transaction** 表旁邊的 **+ Add rule**。

![A screenshot of a computer Description automatically
generated](./media/image39.png)

11. 選擇 **contactid** 和
    **msrc_customerid**，然後將規則命名為 **contacttransactions**。選擇
    **Done**。

![A screenshot of a computer Description automatically
generated](./media/image40.png)

12. 選擇 **Next**（下一步）。

![A screenshot of a computer Description automatically
generated](./media/image41.png)

13. 在 **Unified data view** （統一數據視圖）
    頁面上查看和編輯如何將源數據合併到 Unified customer fields
    （統一數據視圖） 中。單擊 **Next**。

![A screenshot of a computer Description automatically
generated](./media/image42.png)

14. 在 **Review and create customer profiles**
    （查看並創建客戶配置文件） 頁面上，選擇 **Create customer profiles**
    （創建客戶配置文件）。

![A screenshot of a computer Description automatically
generated](./media/image43.png)

15. 此過程需要幾分鐘才能完成。

16. 查看 **Customer data** （客戶數據）、 **Deduplication rules**
    （重複數據刪除規則）、**Matching rules** （匹配規則） 和 **Unified
    data view** （統一數據視圖） **Unify** 頁面上的字段。

![A screenshot of a computer Description automatically
generated](./media/image44.png)

## 練習 3：使用 Copilot for Customer Insights 創建客戶細分 - 數據（預覽）

1.  在 **Customer Insights - Data** 中，轉到 **Insights \> Segments**
    ，然後選擇 **+ New segment** 以創建細分。

![A screenshot of a computer Description automatically
generated](./media/image45.png)

2.  選擇 Copilot 圖標以打開 **Copilot** 窗格。

![A screenshot of a computer Description automatically
generated](./media/image46.png)

3.  輸入區段的描述或選擇建議的提示之一。例如，選擇 **Customer who have a
    loyalty membership**（具有忠誠度會員資格的客戶）。

![A screenshot of a chat Description automatically
generated](./media/image47.png)

4.  選擇 **Use** 將結果應用於規則。

![A screenshot of a chat Description automatically
generated](./media/image48.png)

5.  選擇 **Run** （運行）。

![A screenshot of a computer Description automatically
generated](./media/image49.png)

6.  在 **Review details** （查看詳細信息） 頁面上，在 **Name** （名稱）
    字段中輸入 **Loyalty membership**，然後選擇 **Run** （運行）。

![A screenshot of a computer Description automatically
generated](./media/image50.png)

7.  現在已創建 **Loyalty membership** 段。

![A screenshot of a computer Description automatically
generated](./media/image51.png)

**注：** 如果生成的區段包含多個 [***relationship
paths***](https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/relationships)，則默認情況下會使用最短路徑。**編輯**區段以更改關係路徑。
