# 실습 11: Copilot을 사용하여 고객 인사이트를 위한 세그먼트 만들기 - 데이터(미리 보기)

## 연습 1: 데이터 추가하기

1.  제공된
    링크([**https://home.ci.ai.dynamics.com/**](https://home.ci.ai.dynamics.com/))를
    사용하여 **Customer Insights - Data** **environment**에 접속합니다.
    왼쪽 탐색 메뉴에서 **Data** \> **Data sources**를 선택합니다.

![](./media/image1.png)

참고: introducing Copilot in Customer Insights – Data팝업을 닫으세요

![](./media/image2.png)

2.  **Add a data source**를 선택합니다.

![](./media/image3.png)

3.  **Microsoft Power Query**를 선택합니다.

4.  데이터 소스의 **Data source** **Name** 에 **GroceryContacts**를
    입력하고 **Next**를 선택합니다.

![](./media/image4.png)

5.  **Choose data source**  페이지에서 **Text/CSV**를 선택합니다.

![](./media/image5.png)

6.  **Connection settings** 페이지에서 **Upload file** 를 선택한 다음
    **Browse**를 선택합니다.

![](./media/image6.png)

7.  실습 **VM**의 **C:\LabFiles**에서 **Grocery_Contacts.csv** 파일을
    선택합니다. **Open**를 선택합니다.

![](./media/image7.png)

8.  **Sign in**을 선택하여 계정에 로그인합니다.

![](./media/image8.png)

9.  **Office 365 admin tenant** 자격 증명을 입력합니다.

![A screenshot of a computer error Description automatically
generated](./media/image9.png)

10. **Next**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image10.png)

11. **Preview file data** 에서 **Transform data**를 선택합니다.

![](./media/image11.png)

12. **Transform data** 페이지에서 **Transform** 리본으로 이동한 다음
    **Use first row as headers \> Use first row as headers** 옵션을
    선택합니다.

![](./media/image12.png)

13. **birthdate** 열을 마우스 오른쪽 버튼으로 클릭하고 **Change
    type**으로 이동한 다음 **Date**를 선택합니다.

![](./media/image13.png)

14. 키보드의 **Ctrl** 키를 누른 상태에서 다음 열을 선택합니다:
    **annualincome**, **msrc_creditscore**, **msrc_customerrelationshipduration**,
    및 **msrc_distancetoneareststore**.

15. 이러한 열이 강조 표시되면 그 중 하나를 마우스 오른쪽 버튼으로
    클릭하고 **Change type**으로 이동한 다음 **Decimal number**를
    선택합니다.

![](./media/image14.png)

16. 오른쪽의 **Properties**에서 **Name**을
    [**contact**](urn:gd:lg:a:send-vm-keys)로 변경한 다음 키보드의
    **Enter** 키를 누릅니다.

![](./media/image15.png)

17. **Next**를 선택합니다.

![](./media/image16.png)

18. **Refresh settings**  페이지에서 **Refresh manually** 를 선택합니다.
    **Refresh manually**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image17.png)

19. 데이터 소스가 성공적으로 추가될 때까지 기다립니다.

![A screenshot of a computer Description automatically
generated](./media/image18.png)

20. **Data sources**페이지에서 **Add a data source**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image19.png)

21. **Microsoft Power Query**를 선택합니다.

22. 데이터 원본의 **Data source Name** 에
    [**GroceryTransactions**](urn:gd:lg:a:send-vm-keys)를 입력하고
    **Next**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image20.png)

23. **Choose data source** 페이지에서 **Text/CSV**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image21.png)

24. **Connection settings** 페이지에서 **Upload file** 를 선택한 다음
    **Browse**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image22.png)

25. 실습 **VM**의 **C:\LabFiles**에서 **Grocery_transaction.csv** 파일을
    선택하고 **Open**를 클릭합니다.

![](./media/image23.png)

26. 파일이 업로드되면 **Next**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image24.png)

27. **Preview file data**  페이지에서 **Transform data**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image25.png)

28. 이전과 마찬가지로 **Transform** 으로 가서 **Use first row as headers
    \> Use first row as headers**로 사용을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image26.png)

29. **msrc_transactiontimestamp** 열로 스크롤하여 선택합니다. 열을
    마우스 오른쪽 버튼으로 클릭하고 **Change type**를 선택한 다음
    **Date/Time**을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image27.png)

30. 키보드의 **Ctrl** 키를 길게 눌러
    **msrc_transactionamount** 및 **msrc_discountappliedamount**  열을
    선택합니다. 열 중 하나를 마우스 오른쪽 버튼으로 클릭하고 **Change
    type**으로 이동한 다음 **Decimal number**를 선택합니다.

![](./media/image28.png)

31. **Next**를 선택합니다.

![](./media/image29.png)

32. **Refresh settings** 페이지에서 **Refresh manually**를 선택합니다.
    **Save**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image30.png)

33. 데이터 소스가 성공적으로 추가될 때까지 기다립니다.

![A screenshot of a computer Description automatically
generated](./media/image31.png)

# 연습 2: 데이터 통합

1.  **Customer Insights - Data**에서 왼쪽 탐색 창의 **Data**를 확장한
    다음 **Unify**를 선택합니다.

2.  **Customer data**영역에서 **Get started**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image32.png)

3.  **Describe the customer data to be unified** 페이지에서 **Select
    tables and columns** 를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image33.png)

4.  **contact** 및 **Grocery_transaction** 테이블을 선택한 다음
    **Apply**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image34.png)

5.  **contact** 테이블을 선택한 다음 **contactid**를 기본 키로
    선택합니다.

![A screenshot of a computer screen Description automatically
generated](./media/image35.png)

6.  **Grocery_transaction** 테이블을 선택한 후 **msrc_transactionid** 를
    기본 키로 선택하고 **Next**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image36.png)

7.  **Define deduplication rules** 페이지에서 **Next**를 클릭합니다.

![A screenshot of a computer Description automatically
generated](./media/image37.png)

8.  **Define matching rules** 페이지에서 다음 순서로 테이블을
    설정합니다: **contact** 및 **Grocery_transaction**.

9.  모든 테이블에 대해 **Include all records** 체크박스가 선택되어
    있는지 확인합니다.

![A screenshot of a computer Description automatically
generated](./media/image38.png)

10. **Grocery_transaction** 테이블 옆에 있는 **+ Add rule** 를
    선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image39.png)

11. **contactid**와 **msrc_customerid**를 선택한 후 규칙 이름을
    [**contacttransactions**](urn:gd:lg:a:send-vm-keys)로 지정합니다.
    **Done**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image40.png)

12. **Next**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image41.png)

13. **Unified data view** 페이지에서 소스 데이터가 통합 고객 필드에
    결합되는 방식을 검토하고 편집합니다. **Next**를 클릭합니다.

![A screenshot of a computer Description automatically
generated](./media/image42.png)

14. **Review and create customer profiles** 페이지에서 **Create customer
    profiles**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image43.png)

15. 이 프로세스를 완료하는 데 몇 분 정도 걸립니다.

16. **Unify** 페이지에서 **Customer data**, **Deduplication
    rules**, **Matching rules** 및 **Unified data view**  필드를
    검토합니다.

![A screenshot of a computer Description automatically
generated](./media/image44.png)

## 연습 3: 고객 인사이트를 위한 Copilot - 데이터(미리 보기)를 사용하여 세그먼트 만들기

1.  **Customer Insights - Data**에서 **Insights** \> **Segments** 로
    이동한 다음 **New segment** 를 선택하여 세그먼트를 만듭니다.

![A screenshot of a computer Description automatically
generated](./media/image45.png)

2.  Copilot 아이콘을 선택하여 **Copilot** 창을 엽니다.

![A screenshot of a computer Description automatically
generated](./media/image46.png)

3.  Enter a description of your segment or choose one of the suggested
    prompts. For example, select **Customers who have a loyalty
    membership**.  
    세그먼트에 대한 설명을 입력하거나 제안된 프롬프트 중 하나를
    선택합니다. 예를 들어, **Customers who have a loyalty membership**을
    선택합니다.

![A screenshot of a chat Description automatically
generated](./media/image47.png)

4.  결과를 규칙에 적용하려면 **Use** 를 선택합니다.

![A screenshot of a chat Description automatically
generated](./media/image48.png)

5.  **Run**을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image49.png)

6.  **Review details** 페이지에서 **Name** 필드에 **Loyalty
    membership** 을 입력한 다음 **Run**을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image50.png)

7.  **Loyalty membership** 세그먼트가 생성되었습니다.

![A screenshot of a computer Description automatically
generated](./media/image51.png)

참고: 결과 세그먼트에 여러 [***relationship
paths***](https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/relationships)가
포함된 경우 기본적으로 가장 짧은 경로가 사용됩니다. 관계 경로를
변경하려면 세그먼트를 **편집합니다**.
