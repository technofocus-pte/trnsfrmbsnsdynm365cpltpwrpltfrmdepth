# 실습3: 새로운 AI 기능을 사용하여 Microsoft Copilot Studio에서 봇 구축

이 실습에서는 Microsoft Copilot Studio의 Copilot을 사용하여 봇을 만들어
보겠습니다. 또한, Conversation Booster 기능을 사용하여 봇의 응답을
개선하는 방법도 알아봅니다.

1.  [**https://copilotstudio.microsoft.com/**](urn:gd:lg:a:send-vm-keys)을
    사용하여 **Office 365 admin tenant** 자격 증명으로 **Microsoft
    Copilot Studio**에 로그인합니다.

[**admin@M365x15683240.onmicrosoft.com**](urn:gd:lg:a:send-vm-keys)

[**Cn~R2y15%7Pju3lrGdR;(HO9Y+%^70p~**](urn:gd:lg:a:send-vm-keys)

2.  요청이 있으면 country/region으로 **United States** 를 선택한 다음
    **Start free trial/Get started**을 선택합니다.

![](./media/image1.png)

3.  환경 선택기에서 **Dev One** 환경을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image2.png)

4.  **Welcome to Copilot Studio**  팝업에서 **Skip**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image3.png)

5.  왼쪽 탐색 메뉴에서 **+Create** 를 선택한 다음 **New** **agent**를
    선택합니다.

> ![A screenshot of a computer Description automatically
> generated](./media/image4.png)

Create a bot wizard가 열립니다. 이 마법사는 봇의 이름을 지정하고, 언어를
선택하고, 생성 답변으로 대화를 강화할지 여부를 선택하는 등 봇을 설정하는
데 도움을 줍니다.

6.  **Skip to** **configure**를 선택합니다.

> ![A screenshot of a computer Description automatically
> generated](./media/image5.png)

7.  봇의 이름을 **Real Estate Booking Service** 로 지정한 다음 **+Add
    knowledge**를 클릭합니다.

![A screenshot of a computer Description automatically
generated](./media/image6.png)

8.  **Public website**를 선택합니다.

> ![](./media/image7.png)

![A screenshot of a computer Description automatically
generated](./media/image8.png)

**참고**: **Create**를 선택한 후 새 환경에서 첫 번째 봇을 만드는 데 최대
15분이 걸릴 수 있습니다. 이후 봇은 훨씬 더 빨리 생성됩니다.

9.  웹페이지 링크 아래에
    [**https://powerplatform.microsoft.com/**](urn:gd:lg:a:send-vm-keys)을
    입력한 다음 **Add**를 선택합니다.

> ![A screenshot of a computer Description automatically
> generated](./media/image9.png)

![A screenshot of a computer Description automatically
generated](./media/image10.png)

10. Webpage link필드 아래에 링크가 추가된 것을 확인할 수 있습니다. 이제
    다시 **Add**를 선택합니다.

> ![A screenshot of a computer Description automatically
> generated](./media/image11.png)

![A screenshot of a computer Description automatically
generated](./media/image12.png)

11. **Create**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image13.png)

12. 에이전트를 생성한 후, 위의 가로 팔레트에서 **Topics**를 선택하고 **+
    Add a topic** 드롭다운 메뉴를 선택합니다. **Create from description
    with Copilot**을 선택합니다.

> ![A screenshot of a computer Description automatically
> generated](./media/image14.png)

![A screenshot of a computer Description automatically
generated](./media/image15.png)

**참고**: **Create with Copilot** 옵션이 표시되지 않으면 지능형 작성
지원을 활성화해야 할 수 있습니다:

a\. 상단 메뉴에서 **Settings** 아이콘을 선택한 다음 **General
settings**을 선택합니다.

b\. **Intelligent authoring support with Copilot** 토글을 **On**으로
설정합니다.

13. **Name your topic** 이라는 새 창이 나타나고 **Create a topic
    to...** 공간에 설명을 입력합니다.

14. **Name your topic**  필드에 다음 텍스트를 입력합니다:

[**Book a Real Estate Showing**](urn:gd:lg:a:send-vm-keys)

15. **Create a topic to...**필드에 다음 텍스트를 입력합니다.

collect a user's full name, email, address of the property, and date and
time of the showing

**Create**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image16.png)

![](./media/image17.png)

생성된 트리거 문구와 함께 새로운 주제가 표시됩니다.

![](./media/image18.png)

![A screenshot of a computer Description automatically
generated](./media/image19.png)

**참고**: 생성된 콘텐츠는 이 랩에 표시된 내용과 다르게 표시될 수
있습니다.

여러 질문 노드, 엔터티 선택 및 변수 이름도 표시되어야 합니다.

![](./media/image20.png)

![A screenshot of a computer Description automatically
generated](./media/image21.png)

16. **What is your email address?** 질문 노드를 찾아 선택합니다.

> ![](./media/image22.png)

![A screenshot of a computer Description automatically
generated](./media/image23.png)

17. Authoring canvas상단에 있는 **Edit with Copilot**  아이콘을
    선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image24.png)

18. **What is your email address** 질문 노드를 선택하고 **+Add**,를
    선택한 다음 **Message variation**을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image25.png)

메시지 상자에 **Thank you** 를 입력한 후 {X} 아이콘을 클릭하여 변수를
삽입합니다. **Name** variable을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image26.png)

19. 마지막 노드 뒤에 있는 **+ sign** 를 선택하면 질문 노드가 하나 더
    추가됩니다.

![A screenshot of a computer Description automatically
generated](./media/image27.png)

**Do you want to visit again?**를 입력하고, **Identity** 아래에서
**Multiple choice option** 을 선택하고, **+New option**을 클릭한 다음
**+New option** 을 두 번 선택하여 **Yes**와 **No**를 각각 입력합니다.

![A screenshot of a computer Description automatically
generated](./media/image28.png)

20. **Save**을 선택하여 변경 사항을 저장합니다.

![A screenshot of a computer Description automatically
generated](./media/image29.png)

21. 화면 오른쪽에 Test your copilot 창이 이미 열려 있는 것을 볼 수
    있습니다.

![A screenshot of a computer Description automatically
generated](./media/image30.png)

22. **Conversation Start**메시지가 나타나면 봇이 대화를 시작합니다.
    응답으로, 생성한 주제에 대한 트리거 문구를 입력합니다.

[**I want to book a real estate showing**](urn:gd:lg:a:send-vm-keys)

[**The bot responds with the "What is your full name?" question, as
shown in the following image.**](urn:gd:lg:a:send-vm-keys)

![A screenshot of a chat Description automatically
generated](./media/image31.png)

23. 나머지 정보를 입력합니다:

> Copy
>
> Full name: \<Your name\>
>
> Email address: \<Your email address\>
>
> Address: 555 Oak Lane, Denver, CO 80203
>
> Date and Time: 10/10/2023 10:00 AM

![A screenshot of a chat Description automatically
generated](./media/image32.png)

24. Yes 또는 No를 선택합니다.

![A screenshot of a chat Description automatically
generated](./media/image33.png)

25. 부스트된 봇을 What is Microsoft Power Platform?를 입력하세요. 봇은
    봇 생성 시 제공한 웹사이트 정보를 검색하여 응답을 반환합니다.

![A screenshot of a computer Description automatically
generated](./media/image34.png)
