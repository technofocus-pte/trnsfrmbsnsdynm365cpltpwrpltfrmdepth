# 실습 10: Microsoft Teams에서 Microsoft Copilot for Sales 앱 사용 및 conversation intelligence대시보드 사용(미리 보기)

**참고**: 제품 이용이 불가능한 경우 실습 11으로 전환할 수 있습니다. 제품
이용 가능 여부에 따라 나중에 이 랩을 수행할 수 있습니다.

## 연습 1: Teams에 Sales용Microsoft Copilot 설치 및 고정

### 작업 1: 사용자 지정 Teams 앱 설정 정책 만들기

1.  **Microsoft Teams admin center**
    (https://admin.teams.microsoft.com/dashboard)에 로그인합니다.

2.  왼쪽 창에서 **Teams apps \> Setup policies**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image1.png)

3.  **Manage policies** 탭에서 **Add**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image2.png)

1.  **Name** [**Assign Copilot
    permissions**](urn:gd:lg:a:send-vm-keys)을 입력합니다.

2.  **User pinning**을 켭니다.

![A screenshot of a computer Description automatically
generated](./media/image3.png)

3.  **Installed apps**에서 **Add apps**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image4.png)

4.  **Add installed apps** 패널에서 **Copilot for Sales** 앱을
    검색하세요. 앱 권한 정책으로 앱을 필터링할 수도 있습니다.

5.  **Copilot for Sales** 위에 마우스를 올리고 Select를 클릭합니다.

![A screenshot of a computer Description automatically
generated](./media/image5.png)

6.  다시 **Add**를 선택하여 나열된 앱을 설치합니다.

![A screenshot of a phone Description automatically
generated](./media/image6.png)

7.  **Pinned apps**에서 **Add apps**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image7.png)

8.  **Add pinned** 패널에서 **Copilot for Sales** 앱을 검색합니다. 앱
    권한 정책별로 앱을 필터링할 수도 있습니다.

![A screenshot of a computer Description automatically
generated](./media/image8.png)

9.  **Copilot for Sales** 위에 마우스를 올려놓고 **Select**를
    클릭합니다.

![A screenshot of a phone Description automatically
generated](./media/image9.png)

10. 다시 **Add** 를 선택하여 나열된 앱을 고정합니다.

![A screenshot of a phone Description automatically
generated](./media/image10.png)

11. **App bar**  또는 **Messaging extensions**에서 Teams에 표시할
    순서대로 앱을 정렬합니다.

12. **Save**을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image11.png)

13. 브라우저에서 새 탭을 열고 제공된
    링크[**https://teams.microsoft.com/\_#/apps/c92c289e-ceb4-4755-819d-0d1dffdab6fa/sections/homeTab**](urn:gd:lg:a:send-vm-keys)를
    사용하여 Microsoft Teams 웹앱으로 이동합니다.

14. **Office 365 admin tenant** 자격 증명으로 로그인합니다.

15. **Teams**에 **Microsoft Copilot for Sales** 앱이 고정되어 있는 것을
    확인할 수 있습니다.

![A screenshot of a computer Description automatically
generated](./media/image12.png)

16. 고정된 앱이 보이지 않으면 왼쪽 창에서 앱을 선택하고 Copilot for
    Sales를 검색한 후 Add를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image13.png)

1.  Add를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image14.png)

## 작업 2: Outlook에서 Microsoft Teams 모임 예약하기

1.  **App launcher**로 이동합니다.

![A screenshot of a calendar Description automatically
generated](./media/image15.png)

2.  Outlook을 선택합니다.

![A screenshot of a phone Description automatically
generated](./media/image16.png)

3.  왼쪽 탐색 창에서 **Calendar**를 선택하세요. **New event \> Event**를
    선택합니다.

![A screenshot of a calendar Description automatically
generated](./media/image17.png)

4.  회의 이름을 [**Sales Copilot Test
    Meeting**](urn:gd:lg:a:send-vm-keys)로 지정하고, 현재 날짜를
    선택하고 시간을 선택합니다(현재 시간보다 10분 후로 설정).

![A screenshot of a calendar Description automatically
generated](./media/image18.png)

5.  **Invite attendees**필드에 **email id**를 입력합니다. Search for a
    room or location 필드에서 **Teams meeting** 토글 버튼이 **On**인지
    확인합니다. **Send**를 선택합니다.

![](./media/image19.png)

6.  이제 **Teams**앱으로 이동하여 **Calendar**를 선택하세요. 새로 예약된
    화의가이 표시됩니다. Meeting을 클릭합니다.

![A screenshot of a calendar Description automatically
generated](./media/image20.png)

7.  **Edit**을 선택합니다.

![A screenshot of a calendar Description automatically
generated](./media/image21.png)

8.  상단 메뉴바에서 **+** 아이콘을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image22.png)

9.  **Copilot for Sales**을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image23.png)

10. **Save**를 선택합니다.

![A screenshot of a screenshot of a video conference Description
automatically generated](./media/image24.png)

11. 회의에 참여하려면 **Join**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image25.png)

12. 다시 **Join** 을 선택합니다

![A screenshot of a computer Description automatically
generated](./media/image26.png)

13. Teams 앱에서 회의에 참여하면 MOD 관리자로부터 알림을 받게 됩니다.
    **Join** 을 선택합니다.

![A screenshot of a video conference Description automatically
generated](./media/image27.png)

14. 오디오를 음소거하고 **Join now**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image28.png)

15. 관리자 팀 웹 앱에서 **Waiting in the lobby** 알림이 표시됩니다.
    **Admit**을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image29.png)

16. **More \> Record**  및 **Transcribe \> Start recording**을
    선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image30.png)

17. MOD 관리자로서 대화 내용을 작성하여 대본을 생성할 수 있습니다. (예:
    You can explain what is Sales Copilot.)

![A screenshot of a computer Description automatically
generated](./media/image31.png)

18. Teams web 앱과 사용자의 Teams 앱에서 회의를 나갑니다.

19. 왼쪽 탐색 창에서 **Chat**를 선택한 후 **Copilot for Sales**을
    선택합니다.

![A screenshot of a chat Description automatically
generated](./media/image32.png)

20. **Open summary**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image33.png)

21. 이제 Copilot for Sales에서 생성된 요약을 볼 수 있습니다.

![A screenshot of a computer Description automatically
generated](./media/image34.png)

## 연습 2: Teams에서 CRM record 공유

1.  관리자의 **Outlook** 계정으로 이동하여 이메일이나 예약된 회의를
    엽니다.

2.  **Copilot for Sales** 창을 엽니다. **Save email to Dynamics 365**을
    클릭합니다.

![A screenshot of a computer Description automatically
generated](./media/image35.png)

3.  **First, turn on server-side sync**  대화 상자에서 **Turn on**을
    선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image36.png)

4.  **Connect to a record** 페이지에서 검색 상자를 사용하여 연락처
    Alex를 검색합니다.

![A screenshot of a phone Description automatically
generated](./media/image37.png)

5.  연락처를 선택하고 **Save**를 클릭합니다.

![A screenshot of a phone Description automatically
generated](./media/image38.png)

6.  선택한 연락처의 기록에 이메일이 저장되면 **Copilot for Sales** 창에
    메시지가 표시됩니다.

![A screenshot of a computer Description automatically
generated](./media/image39.png)

7.  연락처를 선택합니다. **Contact details**  페이지로 이동합니다.

![A screenshot of a phone Description automatically
generated](./media/image40.png)

8.  **Contact details**  페이지에서 **Opportunities**  영역으로 이동하여
    기회 중 하나(예: 50 Café A-100 Automatic) 위에 마우스를 올려놓고
    추가 옵션(... 3개의 점)을 클릭한 다음 **Teams**을 선택하고 **+ Set
    up deal room**을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image41.png)

9.  **Use an existing team**.을 선택합니다.

![A screenshot of a computer program Description automatically
generated](./media/image42.png)

10. **Test Team** 을 선택한 후 **Next**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image43.png)

11. 채널을 그대로 두고, 개인정보보호를 **Standard**으로 선택하고,
    **Include shared channel** 확인란을 선택한 다음 **Set up team**을
    선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image44.png)

12. Teams 앱으로 이동합니다. **Test Team** 에서 **50 Café A-100
    Automatic**채널을 선택합니다. 다음 스크린샷은 50 Café A-100
    Automatic의 deal room 팀 예시를 보여줍니다.

![A screenshot of a computer Description automatically
generated](./media/image45.png)

13. Copilot for Sales 메시지 아래에 있는 **Reply**를 클릭한 다음 **+**
    아이콘을 선택하여 작업과 앱을 엽니다.

![A screenshot of a computer Description automatically
generated](./media/image46.png)

14. Select **Copilot for Sales** app.

![A screenshot of a computer Description automatically
generated](./media/image47.png)

15. 검색창에 alex를 입력한 후 **Alex Baker** 연락처를 선택합니다.

![A screenshot of a search engine Description automatically
generated](./media/image48.png)

16. 이제 **send icon**을 클릭하여 레코드를 보냅니다.

![A screenshot of a computer Description automatically
generated](./media/image49.png)

17. View record를 클릭하면 연락처 세부 정보가 표시됩니다.

![A screenshot of a computer Description automatically
generated](./media/image50.png)

## 연습 3: Power BI를 사용하여 판매자 대화 데이터 분석(미리 보기)

### 작업 1: Copilot for Sales 대시보드 앱 다운로드

1.  Copilot for Sales 대화 인텔리전스 대시보드를 다운로드하려면
    [**https://go.microsoft.com/fwlink/p/?linkid=2259835**](https://go.microsoft.com/fwlink/p/?linkid=2259835)로
    이동하세요. **Get it now**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image51.png)

2.  Power BI 앱으로 이동합니다. Install this Power BI app창에서
    **Install** 를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image52.png)

3.  앱 목록에서 Copilot for Sales - 대시보드를 확인할 수 있습니다.
    **Copilot for Sales - Dashboard**를 클릭하여 엽니다.

![A screenshot of a search engine Description automatically
generated](./media/image53.png)

4.  보고서에서 다음 페이지를 사용할 수 있습니다:

- Coaching opportunities

- Customer insights

- Call recordings

![A screenshot of a computer Description automatically
generated](./media/image54.png)

5.  **Time period filter**와 **Data filters**를 사용할 수 있습니다.

![](./media/image55.png)

6.  왼쪽 탐색 창에서 **Coaching opportunities page** 를 선택합니다.
    선택한 기간의 대화 KPI와 요약 차트가 표시됩니다.

![](./media/image56.png)

7.  왼쪽 탐색 창에서 **Customer insights page**를 선택합니다. 고객
    감정과 고객이 가장 많이 언급하는 브랜드가 표시됩니다.

![](./media/image57.png)

8.  왼쪽 탐색 창에서 **Conversation recordings** 페이지를 선택하세요. 이
    페이지에서는 통화 녹음을 듣고 대화의 맥락을 이해하는 데 도움이
    됩니다.

![A screenshot of a computer Description automatically
generated](./media/image58.png)

### 작업 2: 대시보드를 조직 데이터에 연결하기

Microsoft AppSource에서 Copilot for Sales - 대화 인텔리전스 대시보드를
다운로드하면 샘플 데이터가 포함되어 있습니다. 이 대시보드를 Dataverse의
사용자 데이터에 연결하려면 다음 단계를 따릅니다:

1.  다운로드한 Copilot for Sales 대시보드가 ​​이미 열려 있다면 **Connect
    your data**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image59.png)

2.  다음 정보를 입력합니다:

a. **EnvironmentPath**:Sales 평가판 Dataverse 환경의 URL입니다. 입력하는
환경 경로 URL에서 https:// prefix를 제거해야 합니다. (URL을 확인하려면
Power Platform 관리 센터로 이동하세요. 왼쪽 탐색 창에서 환경을 선택하고
Sales 평가판을 클릭한 후 환경 URL을 복사하세요.)

b. **CRM type**: 사용 중인 CRM 유형(**Dynamics**)

c\. **Next**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image60.png)

3.  Select an authentication method - **OAuth2** and privacy level
    settings - **None** for your data source. Select **Sign in and
    connect**. 3. 데이터 소스에 대한 인증 방식(**OAuth2**)과 개인정보
    보호 수준 설정(**None**)을 선택합니다. **Sign in and connect**을
    선택합니다.

![A screenshot of a login page Description automatically
generated](./media/image61.png)

4.  대시보드가 ​​조직 데이터에 성공적으로 연결되면 보고서를 편집하고
    게시할 수 있습니다.

** **
