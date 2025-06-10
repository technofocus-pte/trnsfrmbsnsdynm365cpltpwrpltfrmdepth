# 실습6: Dynamics 365 Customer Service의 Copilot을 사용하여 고객 문제를 더욱 빠르게 해결하기

## 연습 1: 사례 요약

Copilot 사례 요약은 사례의 맥락을 빠르게 파악하고 고객 문제를 더욱
효율적으로 해결하는 데 도움이 됩니다. 사례 요약에는 사례 제목, 고객,
주제, 제품, 우선순위, 사례 유형 및 설명과 같은 주요 정보가 포함됩니다.

1.  **Customer Service workspace**으로 이동하려면 제공된 링크
    [**https://admin.powerplatform.microsoft.com**](urn:gd:lg:a:send-vm-keys)를
    사용하여 **Power Platform admin center**로 이동하세요.

2.  **Environments** 탭을 선택한 다음 **Customer Service Trial**  환경을
    선택합니다.

![](./media/image1.png)

3.  **Customer Service Trial environment**  페이지에서 **Environment
    URL**을 클릭합니다.

![](./media/image2.png)

4.  **Customer Service workspace**으로 이동합니다. 게시된 앱 페이지로
    이동하는 경우, **Customer Service workspace**을 선택합니다.

참고: URL을 클릭해도 Customer Service workspace으로 이동하지 않으면
Dynamics 365 옆의 탭을 클릭하여 페이지를 전환합니다. 참고: URL을
클릭해도 Customer Service workspace으로 이동하지 않으면 Dynamics 365
옆의 탭을 클릭하여 페이지를 전환하세요.

![A screenshot of a computer Description automatically
generated](./media/image3.png)

5.  **Customer Service Agent Dashboard**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image4.png)

6.  **Customer Service Agent Dashboard**에 나열된 사례 중 하나를
    선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image5.png)

7.  **Case summary** 는 사례 양식에 카드 형태로 표시됩니다. 사례를 열면
    **Summary** 카드는 기본적으로 접혀 있습니다.

![A screenshot of a computer Description automatically
generated](./media/image6.png)

8.  **Summary** 탭을 확장합니다.

![A screenshot of a computer Description automatically
generated](./media/image7.png)

9.  생성된 사례 요약을 볼 수 있습니다.

![A screenshot of a computer Description automatically
generated](./media/image8.png)

## 연습 2: 질문 초안 작성

1.  **Customer Service Agent Dashboard** 에서 샘플 사례 중 하나를
    선택합니다(예: **A Mineral Build Up in Water Supply**).

![A screenshot of a computer Description automatically
generated](./media/image9.png)

답을 알고 있을 동료나 상사에게 질문하는 것처럼 자유롭게 질문할 수
있습니다.

2.  화면 오른쪽에 열리는 **Copilot** 창에 type [**What is mineral built
    up in water supply?**](urn:gd:lg:a:send-vm-keys)라고 입력하고
    **Send** 아이콘을 선택합니다.

> **참고**: Copilot 설정 과정은 완료하는 데 시간이 걸릴 수 있습니다.
> 실습 세션을 최적화하려면 진행 상황을 저장하고 다음 실습 활동으로
> 넘어가세요. Copilot 설정이 완료되면 이 실습으로 돌아와 중단했던
> 부분부터 이어서 진행할 수 있습니다.

![A screenshot of a computer Description automatically
generated](./media/image10.png)

3.  이제 **Copilot**이 질문에 답변한 것을 볼 수 있습니다.

![A screenshot of a computer Description automatically
generated](./media/image11.png)

4.  what to do........ or how to fix issue of clogging in smart brew
    system 또는  [**What to do if water doesn't come consistently in
    smart brew system?**](urn:gd:lg:a:send-vm-keys)와 같은 추가 질문을
    할 수 있습니다. 그리고 **Send** 아이콘을 클릭하세요. **Copilot**에서
    답변을 드립니다.

![A screenshot of a computer Description automatically
generated](./media/image12.png)

5.  **Copilot**을 사용하면 다음과 같은 작업을 수행할 수 있습니다:

    - **직접 질문하기**: Copilot은 조직에서 제공하는 지식 소스에서 가장
      관련성 높은 답변을 보여줍니다.

    - **차례대로 후속 질문하기**: Copilot의 답변이 즉시 유용하지 않은
      경우, 후속 질문을 하고 자연스럽고 대화하는 방식으로 Copilot을
      안내할 수 있습니다.

    - **Copilot에게 더 나은 답변을 제공하도록 요청하기**: Copilot은 추가
      안내에 따라 답변을 재구성할 수도 있습니다.

예를 들어, [**Can you summarize your
response?**](urn:gd:lg:a:send-vm-keys) 또는 [**Can you attempt a
response providing details for each of the steps you
mentioned?**](urn:gd:lg:a:send-vm-keys)라고 입력합니다.

![A screenshot of a computer Description automatically
generated](./media/image13.png)

6.  Copilot에서 제공하는 답변에 만족하시면 답변 전체 또는 일부를
    사용하여 고객의 질문에 답변할 수 있습니다:

    - Copilot 답변의 일부를 채팅에 복사하거나 음성 대화 중에 읽어보세요.
      **Copy**  아이콘을 선택하면 전체 답변이 클립보드에 복사됩니다.

![A screenshot of a computer Description automatically
generated](./media/image14.png)

**참고**: 디지털 메시징 대화 중일 때 **Send to customer** 를 선택하면
편집 창이 열리고, 여기에서 답변을 수정하여 고객에게 보낼 수 있습니다.
고객 키워드를 변경하여 Copilot이 더 정확한 답변을 생성하도록 할 수도
있습니다.

7.  **Check sources** 를 선택하면 Copilot이 답변을 가져온 지식 기반 또는
    웹사이트 링크를 확인할 수 있습니다. 이 보충 정보는 참고 자료로
    사용하거나 고객과 공유할 수 있습니다.

![A screenshot of a computer screen Description automatically
generated](./media/image15.png)

8.  링크를 클릭하면 왼쪽에 콘텐츠가 표시됩니다.

![A screenshot of a computer Description automatically
generated](./media/image16.png)

9.  새로 열린 탭을 닫으세요. 이 경우 Troubleshooting Brewing Issues
    탭입니다.

![A screenshot of a computer Description automatically
generated](./media/image17.png)

10. Copilot의 답변이 얼마나 유용한지 평가하려면 thumbs-up 또는
    thumbs-down 아이콘을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image18.png)

11. 고객 대화가 종료된 후 또는 Copilot에서 지금까지의 대화를 무시하도록
    하려면 **Copilot** 창 상단에서 **Clear chat** 를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image19.png)

## 연습 3: 이메일 초안 작성

1.  **Copilot** 창에서 **Write an email**탭을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image20.png)

2.  사례 개요 페이지에서 **Related**탭을 선택한 다음 **Activities**를
    선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image21.png)

3.  **+New Activity \> Email**을 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image22.png)

4.  이메일 작성을 시작하면 오른쪽 패널에 Copilot이 열리고 미리 정의된
    프롬프트 5개와 사용자 지정 프롬프트 1개가 표시됩니다:

    - **Suggest a call**: 오늘이나 내일 고객과 통화하자는 내용의 답장을
      작성합니다.

    - **Request more information**: 문제 해결에 도움이 되도록 고객에게
      더 자세한 내용을 요청하는 답장을 작성합니다.

    - **Empathize with feedback**: 불만을 표명한 고객에게 공감적인
      답변을 제공하는 답변을 초안합니다.

    - **Provide product/service details**: 특정 제품이나 서비스에 대한
      세부 정보를 제공하거나 고객의 질문에 답변하는 답변을 초안합니다.

    - **Resolve the customer's problem**: 고객의 문제에 대한 해결책과
      해당되는 경우 해결 단계를 제공하는 답변을 초안합니다.

    - **Custom**: 답변을 위한 프롬프트를 직접 제공할 수 있습니다.

![A screenshot of a computer Description automatically
generated](./media/image23.png)

5.  미리 정의된 프롬프트 목록에서 **Resolve the customer's problem**을
    선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image24.png)

6.  보시다시피 Copilot이 제안을 생성했습니다.

![A screenshot of a computer Description automatically
generated](./media/image25.png)

7.  이제 답변을 검토할 수 있습니다. 필요한 내용을 변경한 후 **Copy to
    email** 을 선택하여 전체 답변을 임시 보관함에 복사합니다. 또는
    답변의 일부를 선택하고 마우스 오른쪽 버튼을 클릭하여 복사하여
    붙여넣을 수도 있습니다.

![A screenshot of a phone Description automatically
generated](./media/image26.png)

8.  이제 왼쪽 본문 부분에서 응답을 확인할 수 있습니다.

![A screenshot of a computer Description automatically
generated](./media/image27.png)

9.  이제 이메일을 보내거나 저장할 수 있습니다.

![A screenshot of a computer Description automatically
generated](./media/image28.png)
