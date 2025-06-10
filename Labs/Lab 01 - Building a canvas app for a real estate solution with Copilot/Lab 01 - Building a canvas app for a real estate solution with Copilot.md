# 实验 1：在 Power Apps 中使用 Copilot 为房地产解决方案构建画布应用

在本实验中，您将使用 Power Apps 中的 Copilot
创建移动应用程序。现场代理将使用此应用浏览房地产库存并管理看房预约，数据将存储在
Dataverse 中。

\*\*注意：\*\*在本实验中，您的数据结果可能与屏幕截图和图像中显示的结果不同。这是因为
Power Apps 使用 OpenAI 为实验室生成数据，并且数据每天都在变化。

1.  使用您的 Office 365 租户凭据登录 Power Apps
     [**https://make.powerapps.com/**](urn:gd:lg:a:send-vm-keys)。

2.  确保您位于开发人员环境 - **Dev One**
    中。如果没有，请单击环境选择器，然后选择 **Dev One**。

![](./media/image1.png)

3.  在 Power Apps 的主页上，在中心文本字段中，输入以下提示以搜索 AI
    生成的表：

构建一个应用程序来管理房地产看房

选择 **Send** （发送） 按钮。

![](./media/image2.png)

4.  在 Copilot AI 根据您的提示生成表后，查看表以查看为表的开头创建的列。

![](./media/image3.png)

5.  要查看更多信息，请单击表格上方的三个点。

![](./media/image3.png)

下一步是修改并添加到已生成的表中。

6.  现在单击 **Showings 表**，然后在文本框中，在屏幕右侧的 Copilot
    窗格下部，输入以下文本：

添加列以跟踪客户端全名

这将在看房表中增加一列。选择 **Send** （发送） 按钮。

![](./media/image4.png)

7.  Copilot
    通知您表已更新，新列应显示为已添加到显示表中。（将滑动条向右移动）。要查看添加到表中的新列，请单击
    **View data** from upper horizontal pane。 

![A screenshot of a computer Description automatically
generated](./media/image5.png)

![A screenshot of a computer Description automatically
generated](./media/image6.png)

8.  在聊天中输入以下文本：

添加一列以跟踪客户电子邮件

选择 **Send** （发送） 按钮。

新列将添加到表中，并显示客户的电子邮件。

![A screenshot of a computer Description automatically
generated](./media/image7.png)

**注意：**表中生成的数据可能与本实验屏幕截图中表中显示的数据不同。

9.  在聊天中输入以下文本：

添加列以跟踪客户端地址和代理名称

选择 **Send** （发送） 按钮。

新列将添加到表中，并显示客户的电子邮件。

![A screenshot of a computer Description automatically
generated](./media/image8.png)

10. 在聊天中输入下面给定的文本，然后选择 发送 按钮。新列 Status （状态）
    将添加到表中，并显示客户的电子邮件。

添加列状态，列的数据类型为 choice （Pending， Completed， Confirmed，
Cancelled）

![A screenshot of a computer Description automatically
generated](./media/image9.png)

11. 选择 **Status** column name 下拉菜单，然后选择 **Edit column**。

![](./media/image10.png)

12. 您可以查看列的属性以及当前状态详细信息和数据。选择此窗格右上角的
    **X** 以将其关闭。 

![A screenshot of a computer Description automatically
generated](./media/image11.png)

13. 您可以看到现在已添加新选项。选择窗格右上角的 **X** 以将其关闭。

![A screenshot of a computer Description automatically
generated](./media/image12.png)

14. 您可以看到现在已添加新选项。 ![](./media/image13.png)

15. 使用 Copilot 窗格右上角的 \*\*X\*\* 图标关闭 \*\*Copilot 窗格\*\*。 

![A screenshot of a computer Description automatically
generated](./media/image14.png)

11. 您的表应包含多个列。但是，要继续学习此学习路径中的模块，请尝试删除一些您不会使用的列。

您需要的列列表是：

- 展示

- 地址

- 日期

- 地位

- 代理名称

- 客户端全名

- 客户电子邮件

使用您在 **Copilot Chat**
窗口中学到的知识来调整您的表以匹配前面的列表。如果需要删除列、更改列名称或添加列，请务必参阅
**Suggestions** 部分。

![Screenshot](./media/image15.png)

16. 要创建应用程序，请选择屏幕右上角的 **\*\*Save and Open App\*\***
    按钮。再次单击 **\*\*Done working？\*\*** 弹出窗口中的 **\*\*Save
    and Open App\*\***。 

![](./media/image16.png)

![](./media/image17.png)

17. 首次加载应用时，可能会出现一个对话框，指出 **Welcome to Power Apps
    Studio**。如果是这样，请选择 **Skip** （跳过） 按钮。

![](./media/image18.png)

18. 为您构建的应用程序应显示在 **Edit** 模式下。

![](./media/image19.png)

19. 为了获得更好的视图，请关闭 Copliot 窗格。

![](./media/image20.png)

20. 从左侧导航栏中选择 **Data** 图标。Copilot 创建了一个 **Dataverse**
    表，该表现在显示在 “**Environments**” 部分中。

![](./media/image21.png)

\*\*注意： \*\*目前，只有 Dataverse 支持
Copilot。目前，您不能使用任何其他数据访问点。

接下来，您将编辑表，因为应用程序已创建。

21. . 在 \*\***Data**\*\* 窗格中，将鼠标光标悬停在 \*\*Showing\*\*
    表上。在表的右侧，选择省略号 （...），然后从菜单中选择 \*\***Edit
    data**\*\*。 

![](./media/image22.png)

**注：** 在 **Edit table** （编辑表）
对话框中，您可以将自己的列添加到表中或修改现有列。

22. 从表中选择 \*\*Showing\*\* 列标题。从下拉菜单中，选择 \*\***Edit
    column**\*\* 选项。

![](./media/image23.png)

23. 在此示例中，您不希望 **Data type** （数据类型） 为 **Single line of
    text** （单行文本）。要更改该值，请转到 **Edit column** 窗格，然后从
    **Date type** 下拉菜单中选择 **\# Autonumber**。选择 **Save**
    （保存）。

![](./media/image24.png)

24. 选择 **Edit table** 对话框右下角的 **Close** 按钮。

![A screenshot of a computer Description automatically
generated](./media/image25.png)

25. 该表现在应在 **Data** （数据） 窗格中显示为 **Refreshed** （刷新）。

![](./media/image26.png)

26. 修改应用程序中的库，使其显示相关数据。选择 **Tree view**
    图标以返回到 Tree 视图。

![](./media/image27.png)

27. 在应用程序的主屏幕上，选择 **RecordsGallery2** 以显示
    Showings。要选择 RecirdsGallery2，请遵循以下给定的层次结构。

> (Select Showings Screen \> ScreenContainer3 \> BodyContainer3 \>
> SidebarContainer3 \> RecordsGallery3).

![](./media/image28.png)

28. 现在选择 **RecordsGallery3 的编辑按钮**，将库置于编辑模式。

![A screenshot of a computer Description automatically
generated](./media/image29.png)

29. 单击 RecordGallery3 上的向下箭头，选择
    Title3，然后输入下面给定的公式。

!!ThisItem.’Client Address’!!

![A screenshot of a computer Description automatically
generated](./media/image30.png)

30. 选择 **Subtitle3**，然后将 **Text** 值设置为以下公式：

ThisItem.'Client Email'

![A screenshot of a computer Description automatically
generated](./media/image31.png)

31. 选择 **Body3**，然后将 **Text** 值设置为以下公式： 

ThisItem.Status ，然后从建议中选择 

ThisItem.'Status (cra55_status)' 

如果上述公式显示错误，请使用以下公式 

ThisItem.'Location' 

![A screenshot of a computer Description automatically
generated](./media/image32.png)

库中的单个记录现在应类似于下图。

![A screenshot of a computer Description automatically
generated](./media/image33.png)

32. 在 **ScreenContainer3** 中选择 **Form3**，在画布中选择
    **Fields**，然后删除 **Showing**。

![A screenshot of a computer Description automatically
generated](./media/image34.png)

由于您之前将 **ID** 字段更改为
**Autonumber**（自动编号），因此您不希望用户输入自己的编号; Dataverse
会自动为您输入数字。

33. 通过选择屏幕上方的 **Play** （播放）
    按钮，为应用程序中显示的属性发出新请求。

![A screenshot of a computer Description automatically
generated](./media/image35.png)

34. 在左侧窗格中，选择 **+New** 按钮。

![Screenshot](./media/image36.png)

35. 虽然您可以修改表单以自动填写字段，但对于本实验，您将手动完成此步骤以观察应用程序的工作原理。

在字段中填写以下信息：

- 日期：输入任何将来的日期

- 时间： 15:00

- 经纪人姓名： [**Sarah Connor**](urn:gd:lg:a:send-vm-keys)

- 反馈： [**The property is impressive, but the kitchen needs minor
  upgrades.**](urn:gd:lg:a:send-vm-keys)

- 客户全名： [**John Almeda**](urn:gd:lg:a:send-vm-keys)

- 客户邮箱：[**john.almeda@example.com**](urn:gd:lg:a:send-vm-keys)

- 客户地址：[**210 Pine Road, Portland, OR
  97204**](urn:gd:lg:a:send-vm-keys)

- 状态：Pending

- 属性： Luxury Villa

![A screenshot of a computer Description automatically
generated](./media/image37.png)

36. 选择屏幕右上角的复选标记。

![A screenshot of a computer Description automatically
generated](./media/image38.png)

37. 选择右上角的 **X** 以关闭应用程序。

![A screenshot of a computer Description automatically
generated](./media/image39.png)

如果出现一个对话框，显示 **Did you know？**，请选择 **OK**。

![](./media/image40.png)

新请求将添加到请求列表的左侧。

38. 在屏幕的上部，选择 **Save** （保存） 按钮以保存您创建的新应用程序。

如果系统提示，请将 App 名称保存为 **Real Estate Showings**。

![Screenshot](./media/image41.png)

39. 退出应用以返回到 Power Apps 主页。
