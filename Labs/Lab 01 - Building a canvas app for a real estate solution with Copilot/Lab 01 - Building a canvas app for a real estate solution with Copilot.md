# 實驗 1：在 Power Apps 中使用 Copilot 為房地產解決方案構建畫布應用

在本實驗中，您將使用 Power Apps 中的 Copilot
創建移動應用程序。現場代理將使用此應用瀏覽房地產庫存並管理看房預約，數據將存儲在
Dataverse 中。

\*\*注意：\*\*在本實驗中，您的數據結果可能與屏幕截圖和圖像中顯示的結果不同。這是因為
Power Apps 使用 OpenAI 為實驗室生成數據，並且數據每天都在變化。

1.  使用您的 Office 365 租戶憑據登錄 Power Apps
     [**https://make.powerapps.com/**](urn:gd:lg:a:send-vm-keys)。

2.  確保您位於開發人員環境 - **Dev One**
    中。如果沒有，請單擊環境選擇器，然後選擇 **Dev One**。

![](./media/image1.png)

3.  在 Power Apps 的主頁上，在中心文本字段中，輸入以下提示以搜索 AI
    生成的表：

構建一個應用程序來管理房地產看房

選擇 **Send** （發送） 按鈕。

![](./media/image2.png)

4.  在 Copilot AI 根據您的提示生成表後，查看表以查看為表的開頭創建的列。

![](./media/image3.png)

5.  要查看更多信息，請單擊表格上方的三個點。

![](./media/image3.png)

下一步是修改並添加到已生成的表中。

6.  現在單擊 **Showings 表**，然後在文本框中，在屏幕右側的 Copilot
    窗格下部，輸入以下文本：

添加列以跟蹤客戶端全名

這將在看房表中增加一列。選擇 **Send** （發送） 按鈕。

![](./media/image4.png)

7.  Copilot
    通知您表已更新，新列應顯示為已添加到顯示表中。（將滑動條向右移動）。要查看添加到表中的新列，請單擊
    **View data** from upper horizontal pane。 

![A screenshot of a computer Description automatically
generated](./media/image5.png)

![A screenshot of a computer Description automatically
generated](./media/image6.png)

8.  在聊天中輸入以下文本：

添加一列以跟蹤客戶電子郵件

選擇 **Send** （發送） 按鈕。

新列將添加到表中，並顯示客戶的電子郵件。

![A screenshot of a computer Description automatically
generated](./media/image7.png)

**注意：**表中生成的數據可能與本實驗屏幕截圖中表中顯示的數據不同。

9.  在聊天中輸入以下文本：

添加列以跟蹤客戶端地址和代理名稱

選擇 **Send** （發送） 按鈕。

新列將添加到表中，並顯示客戶的電子郵件。

![A screenshot of a computer Description automatically
generated](./media/image8.png)

10. 在聊天中輸入下面給定的文本，然後選擇 發送 按鈕。新列 Status （狀態）
    將添加到表中，並顯示客戶的電子郵件。

添加列狀態，列的數據類型為 choice （Pending， Completed， Confirmed，
Cancelled）

![A screenshot of a computer Description automatically
generated](./media/image9.png)

11. 選擇 **Status** column name 下拉菜單，然後選擇 **Edit column**。

![](./media/image10.png)

12. 您可以查看列的屬性以及當前狀態詳細信息和數據。選擇此窗格右上角的
    **X** 以將其關閉。 

![A screenshot of a computer Description automatically
generated](./media/image11.png)

13. 您可以看到現在已添加新選項。選擇窗格右上角的 **X** 以將其關閉。

![A screenshot of a computer Description automatically
generated](./media/image12.png)

14. 您可以看到現在已添加新選項。 ![](./media/image13.png)

15. 使用 Copilot 窗格右上角的 \*\*X\*\* 圖標關閉 \*\*Copilot 窗格\*\*。 

![A screenshot of a computer Description automatically
generated](./media/image14.png)

11. 您的表應包含多個列。但是，要繼續學習此學習路徑中的模塊，請嘗試刪除一些您不會使用的列。

您需要的列列表是：

- 展示

- 地址

- 日期

- 地位

- 代理名稱

- 客戶端全名

- 客戶電子郵件

使用您在 **Copilot Chat**
窗口中學到的知識來調整您的表以匹配前面的列表。如果需要刪除列、更改列名稱或添加列，請務必參閱
**Suggestions** 部分。

![Screenshot](./media/image15.png)

16. 要創建應用程序，請選擇屏幕右上角的 **\*\*Save and Open App\*\***
    按鈕。再次單擊 **\*\*Done working？\*\*** 彈出窗口中的 **\*\*Save
    and Open App\*\***。 

![](./media/image16.png)

![](./media/image17.png)

17. 首次加載應用時，可能會出現一個對話框，指出 **Welcome to Power Apps
    Studio**。如果是這樣，請選擇 **Skip** （跳過） 按鈕。

![](./media/image18.png)

18. 為您構建的應用程序應顯示在 **Edit** 模式下。

![](./media/image19.png)

19. 為了獲得更好的視圖，請關閉 Copliot 窗格。

![](./media/image20.png)

20. 從左側導航欄中選擇 **Data** 圖標。Copilot 創建了一個 **Dataverse**
    表，該表現在顯示在 “**Environments**” 部分中。

![](./media/image21.png)

\*\*注意： \*\*目前，只有 Dataverse 支持
Copilot。目前，您不能使用任何其他數據訪問點。

接下來，您將編輯表，因為應用程序已創建。

21. . 在 \*\***Data**\*\* 窗格中，將鼠標光標懸停在 \*\*Showing\*\*
    表上。在表的右側，選擇省略號 （...），然後從菜單中選擇 \*\***Edit
    data**\*\*。 

![](./media/image22.png)

**注：** 在 **Edit table** （編輯表）
對話框中，您可以將自己的列添加到表中或修改現有列。

22. 從表中選擇 \*\*Showing\*\* 列標題。從下拉菜單中，選擇 \*\***Edit
    column**\*\* 選項。

![](./media/image23.png)

23. 在此示例中，您不希望 **Data type** （數據類型） 為 **Single line of
    text** （單行文本）。要更改該值，請轉到 **Edit column** 窗格，然後從
    **Date type** 下拉菜單中選擇 **\# Autonumber**。選擇 **Save**
    （保存）。

![](./media/image24.png)

24. 選擇 **Edit table** 對話框右下角的 **Close** 按鈕。

![A screenshot of a computer Description automatically
generated](./media/image25.png)

25. 該表現在應在 **Data** （數據） 窗格中顯示為 **Refreshed** （刷新）。

![](./media/image26.png)

26. 修改應用程序中的庫，使其顯示相關數據。選擇 **Tree view**
    圖標以返回到 Tree 視圖。

![](./media/image27.png)

27. 在應用程序的主屏幕上，選擇 **RecordsGallery2** 以顯示
    Showings。要選擇 RecirdsGallery2，請遵循以下給定的層次結構。

> (Select Showings Screen \> ScreenContainer3 \> BodyContainer3 \>
> SidebarContainer3 \> RecordsGallery3).

![](./media/image28.png)

28. 現在選擇 **RecordsGallery3 的編輯按鈕**，將庫置於編輯模式。

![A screenshot of a computer Description automatically
generated](./media/image29.png)

29. 單擊 RecordGallery3 上的向下箭頭，選擇
    Title3，然後輸入下面給定的公式。

!!ThisItem.’Client Address’!!

![A screenshot of a computer Description automatically
generated](./media/image30.png)

30. 選擇 **Subtitle3**，然後將 **Text** 值設置為以下公式：

ThisItem.'Client Email'

![A screenshot of a computer Description automatically
generated](./media/image31.png)

31. 選擇 **Body3**，然後將 **Text** 值設置為以下公式： 

ThisItem.Status ，然後從建議中選擇 

ThisItem.'Status (cra55_status)' 

如果上述公式顯示錯誤，請使用以下公式 

ThisItem.'Location' 

![A screenshot of a computer Description automatically
generated](./media/image32.png)

庫中的單個記錄現在應類似於下圖。

![A screenshot of a computer Description automatically
generated](./media/image33.png)

32. 在 **ScreenContainer3** 中選擇 **Form3**，在畫布中選擇
    **Fields**，然後刪除 **Showing**。

![A screenshot of a computer Description automatically
generated](./media/image34.png)

由於您之前將 **ID** 字段更改為
**Autonumber**（自動編號），因此您不希望用戶輸入自己的編號; Dataverse
會自動為您輸入數字。

33. 通過選擇屏幕上方的 **Play** （播放）
    按鈕，為應用程序中顯示的屬性發出新請求。

![A screenshot of a computer Description automatically
generated](./media/image35.png)

34. 在左側窗格中，選擇 **+New** 按鈕。

![Screenshot](./media/image36.png)

35. 雖然您可以修改表單以自動填寫字段，但對於本實驗，您將手動完成此步驟以觀察應用程序的工作原理。

在字段中填寫以下信息：

- 日期：輸入任何將來的日期

- 時間： 15:00

- 經紀人姓名： [**Sarah Connor**](urn:gd:lg:a:send-vm-keys)

- 反饋： [**The property is impressive, but the kitchen needs minor
  upgrades.**](urn:gd:lg:a:send-vm-keys)

- 客戶全名： [**John Almeda**](urn:gd:lg:a:send-vm-keys)

- 客戶郵箱：[**john.almeda@example.com**](urn:gd:lg:a:send-vm-keys)

- 客戶地址：[**210 Pine Road, Portland, OR
  97204**](urn:gd:lg:a:send-vm-keys)

- 狀態：Pending

- 屬性： Luxury Villa

![A screenshot of a computer Description automatically
generated](./media/image37.png)

36. 選擇屏幕右上角的複選標記。

![A screenshot of a computer Description automatically
generated](./media/image38.png)

37. 選擇右上角的 **X** 以關閉應用程序。

![A screenshot of a computer Description automatically
generated](./media/image39.png)

如果出現一個對話框，顯示 **Did you know？**，請選擇 **OK**。

![](./media/image40.png)

新請求將添加到請求列表的左側。

38. 在屏幕的上部，選擇 **Save** （保存） 按鈕以保存您創建的新應用程序。

如果系統提示，請將 App 名稱保存為 **Real Estate Showings**。

![Screenshot](./media/image41.png)

39. 退出應用以返回到 Power Apps 主頁。
