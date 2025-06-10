# **실습 2: Copilot을 사용하여 부동산 Showing 승인 프로세스 자동화**

이 실습에서는 Power Automate에서 Copilot을 사용하여 부동산 Showing 승인
프로세스를 자동화하는 자동화를 만들어 보겠습니다. Copilot을 사용하여
새로운 Showing 요청 시 부동산 중개인에게 이메일을 전송하는 흐름을 만들어
보겠습니다. 그러면 중개인은 이메일 내에서 Showing 요청을 승인하거나
거부할 수 있습니다.

Copilot을 사용하여 흐름을 만들려면 다음 단계를 따릅니다:

1.  Office 365 테넌트 자격 증명을 사용하여
    [**https://make.powerautomate.com/**](urn:gd:lg:a:send-vm-keys)에
    로그인합니다.

2.  국가/지역으로 **United States** 를 선택한 후 **Get started**를
    클릭합니다.

![](./media/image1.png)

3.  **environment selector** 를 클릭하고 **Dev One** 환경을 선택하세요.

![](./media/image2.png)

4.  Power Automate **Homepage** 중앙의 **Lets automate something. What
    should it do?**  텍스트 필드에 다음 프롬프트를 입력합니다:

[**Start an approval process for a new microsoft dataverse record and
update the record based on the outcome**](urn:gd:lg:a:send-vm-keys)

**Generate** 버튼을 선택합니다.

![](./media/image3.png)

5.  제안된 흐름에 두 단계만 있는 경우(예: 행이 추가, 수정 또는 삭제될
    때와 시작 및 승인을 기다리는 경우) **Show a different suggestion**를
    클릭합니다.

![](./media/image4.png)

6.  프롬프트에서 Copilot은 검토할 수 있는 제안된 흐름의 개요를
    제공합니다. 흐름을 수락하려면 **Next**를 선택합니다.

![A screenshot of a computer Description automatically
generated](./media/image5.png)

7.  연결된 앱과 서비스를 검토합니다. 연결이 설정되지 않은 경우,
    편집하거나 수정한 후 **Create flow**를 선택하세요.

![](./media/image6.png)

Copilot으로 편집 디자이너가 열리면 오른쪽에 Copilot 채팅 창과 함께
흐름이 표시됩니다.

![](./media/image7.png)

8.  **When a row is added, modified or deleted** 트리거를 선택하여
    매개변수를 설정합니다.

화면 왼쪽 패널에 트리거 세부 정보가 표시되며, 여기에는 필수인 빈 **Table
Name**매개변수도 포함됩니다.

![](./media/image8.png)

9.  \*\* **Table Name** \*\* 드롭다운 메뉴에서 \*\* **Showings** \*\*을
    검색하여 선택합니다.

> \*\*참고: lab1에서 생성된 테이블을 선택합니다. 

![](./media/image9.png)

10. 패널 오른쪽 상단에 있는 축소 아이콘을 사용하여 When a row is added,
    modified or deleted panel을 축소합니다.

![A screenshot of a computer Description automatically
generated](./media/image10.png)

11. 흐름에서 **Start and wait for an approval**  작업을 선택합니다.

**Approval Type**  매개변수가 누락된 것을 확인합니다.

![](./media/image11.png)

12. **Approval Type** 드롭다운 메뉴에서 **Approve/Reject - First to
    respond**을 선택합니다.

**Approval Type**을 선택하면 더 많은 매개변수를 사용할 수 있습니다.

![](./media/image12.png)

13. Copilot 채팅 창에 다음 프롬프트를 입력합니다.

> 시작에 대한 제목 매개변수로 " New Request for Showing "을 추가하고
> 승인 작업을 기다립니다.
>
> \*\*참고:\*\* 데이터를 수집하는 테이블 이름을 사용하세요. 실습 1에서
> 다른 테이블을 생성한 경우 해당 테이블 이름을 사용하세요.

Copilot에서 프롬프트를 처리하는 데 몇 초가 걸립니다. 처리가 완료되면
**Title** 매개변수에 프롬프트 텍스트가 입력됩니다.

![](./media/image13.png)

14. **Assigned To**  매개변수에 이 랩에 사용할 Office 365 테넌트 자격
    증명을 입력합니다. 이 이메일이 승인 요청을 수신하는 이메일입니다.

![](./media/image14.png)

15. **Details**매개변수에 다음 텍스트를 입력합니다:

> 부동산 방문 요청이 새로 생성되었습니다. 아래 세부 정보를 검토하시고
> 요청을 승인 또는 거부해 주세요:
>
> \*\*Property:\*\* \*\*Client:\*\* \*\*Client Email:\*\* \*\*Date:\*\* 

![](./media/image15.png)

16. **Details**매개변수에서 **Property** 옆에 커서를 놓고 번개 아이콘을
    선택하여 **Dynamic content** 창을 엽니다.

![](./media/image16.png)

17. **Dynamic content** 창에서 '행이 추가, 수정 또는 삭제될 때' 단계의
    **See More** 를 선택하여 사용 가능한 동적 콘텐츠 목록을 확장합니다.

![](./media/image17.png)

18. **Client** **Address**  필드를 찾을 때까지 아래로 스크롤한 다음
    **Add**를 선택합니다.

![](./media/image18.png)

**Address** dynamic content 필드가 이제 **Details** 매개변수에
추가되었습니다.

![](./media/image19.png)

19. **Client**, **Client Email** 및 **Date** 필드에 대해서도 동일한
    단계를 완료합니다.

나머지 필드의 입력을 완료하면 값은 다음 이미지와 비슷해야 합니다.

![](./media/image20.png)

20. **Details**매개변수가 완료되면 이중 화살표 아이콘을 선택하여 **Start
    and wait for an approval**작업을 접을 수 있습니다.

![](./media/image21.png)

21. **Condition**  작업을 선택합니다.

![](./media/image22.png)

22. **Choose a value** 상자를 선택한 다음 **Dynamic content** 창에서
    **Outcome**를 선택합니다.

![](./media/image23.png)

23. 조건에 대해 **is equal to** 를 선택한 다음 **Value**에 **Approve**를
    입력합니다.

![](./media/image24.png)

24. **Condition** 동작을 축소합니다.

![](./media/image25.png)

25. 조건의 **True** 브랜치에서 **Update a row**작업을 선택합니다.

![](./media/image26.png)

26. **Table Name**  드롭다운 메뉴에서 **Showings**를 검색하여
    선택합니다.

![](./media/image27.png)

27. **Row ID** 필드를 선택하고 **Dynamic content**를 선택한 다음, 행이
    추가, 수정 또는 삭제될 때 앞에 있는 **see more**를 선택합니다.

28. 이제 **Dynamic content** 창에서 **Showings** 고유 식별자 필드를
    선택하고 **Add**를 클릭합니다.

![](./media/image27.png)

Microsoft Dataverse에서 테이블을 만들 때마다 테이블과 동일한 이름의 열이
자동으로 생성됩니다. 이 열은 생성된 레코드(또는 행)의 고유 lookup ID
역할을 합니다.

29. **Advanced parameters**에서 **Show all** 를 선택합니다.

![](./media/image28.png)

30. **Status** 드롭다운 메뉴에서 **Confirmed**를 선택합니다.

![](./media/image29.png)

Showing가 승인되면 **Real Estate Showings**  테이블의 **Status**필드가
**Confirmed**으로 업데이트됩니다.

31. **Update a row** 작업을 접습니다.

![](./media/image30.png)

32. 조건의 **False** 브랜치에서 **Update a row**  작업을 선택합니다.

![](./media/image31.png)

33. **Table Name** 드롭다운 메뉴에서 **Showings**를 검색하여 선택합니다.

34. **Row ID** 필드를 선택한 다음, **Dynamic content** 
    창에서**Showings** 고유 식별자 필드를 선택합니다.

![](./media/image32.png)

35. **Advanced parameters**에서 **Show all** 을 선택합니다.

![Screenshot](./media/image33.png)

36. **Status** 드롭다운 메뉴에서 **Cancelled**를 선택합니다.

![](./media/image34.png)

Showing가 거부되면 **Real Estate Showings** 테이블의 **Status**필드가
**Cancelled**으로 업데이트됩니다.

37. **Update a row** 작업을 접습니다.

![](./media/image35.png)

38. Copilot 채팅 창에 다음 프롬프트를 입력한 후 제출합니다:

[**Under the "Update a row" action for both branches in the condition,
add a new "Send an email (V2)" action**](urn:gd:lg:a:send-vm-keys)

![](./media/image36.png)

몇 초 후에 Copilot은 다음 이미지에서 볼 수 있듯이 자신이 한 일을
설명해야 합니다.

![](./media/image37.png)

39. 조건의 **True** 브랜치에서 **Send an email** 작업을 선택합니다.

![](./media/image38.png)

40. \*\* To \*\* 필드 줄에서 \*\* Switch to advanced mode\*\*을
    선택하고, **Enter custom value** 입력을 선택한 다음, **Dynamic
    content** 창에서 **Client Email** 필드를 선택합니다. (행이 추가,
    수정 또는 삭제될 때 앞의 **see more** 를 선택합니다.)

![](./media/image39.png)

41. **Subject** 필드에 다음 텍스트를 Copilot 채팅 창에 입력한 다음
    키보드의 **Enter**키를 누릅니다:

**이메일 보내기 작업의 제목 매개변수로 "Your request for a real estate
showing has been approved"를 추가합니다.**

**Subject** 필드에는 프롬프트 텍스트가 입력되어야 합니다.

![](./media/image40.png)

42. **Body** 필드에 다음 텍스트를 Copilot 채팅 창에 입력한 다음 키보드의
    **Enter**키를 누릅니다:

**이메일 보내기 작업의 본문 매개변수에 "Good day - Your request for a
real estate showing has been approved. Please see below for details."를
추가합니다.**

**Body** 필드에는 프롬프트 텍스트가 입력되어야 합니다.

![](./media/image41.png)

43. **Body**텍스트 뒤에 다음 내용을 입력합니다:

**Property:**

**Agent Name:**

**Showing Date:**

**Dynamic content** 창에서 **Client** **Address**, **Agent Name** 및
**Showing** **Date** 필드를 **Body**  텍스트의 적절한 줄에 추가합니다.

![](./media/image42.png)

44. **Dynamic content** 창에서 **Response summary**  필드를 **Body**
    텍스트 끝에 추가합니다.

![](./media/image43.png)

45. **Send an email** 작업을 접습니다.

![](./media/image44.png)

46. ​​조건의 **False** 브랜치에서 **Send an email** 작업을 선택합니다.
    **To**필드를 선택하고 example@example.com 이메일 주소를 제거한 후,
    **Dynamic content** 창에서 **Client Email** 필드를 선택합니다.

![](./media/image45.png)

47. **Subject** 필드에 다음 내용을 Copilot 채팅 창에 입력한 다음
    키보드의 **Enter**키를 누릅니다.

**이메일 보내기 작업의 제목 매개변수로 Your request for a real estate
showing has been rejected를 추가합니다.**

![](./media/image46.png)

48. **Body**필드에 다음 텍스트를 Copilot 채팅 창에 입력한 다음 키보드의
    **Enter** 키를 누릅니다.

**이메일 보내기 작업의 본문 매개변수에 "** **Good day - Your request for
a real estate showing has been rejected. Please see below for
details.”를 추가합니다.**

![](./media/image47.png)

49. **Body**  텍스트 뒤에 다음 내용을 입력합니다.

**Property:**

**Agent Name:**

**Showing Date:**

**Dynamic content** 창에서 **Address**, **Agent Name** 및
**Showing** **Date** 필드를 **Body** 텍스트의 적절한 줄에 추가합니다.

![](./media/image48.png)

50. **Dynamic content** 창에서 **Response summary** 필드를 **Body**
    텍스트 끝에 추가합니다.

![](./media/image49.png)

51. **Send an email**  작업을 접습니다.

52. 화면 왼쪽 상단에서**request approval when a Dataverse record is
    created** 텍스트를 선택하여 흐름 이름을 **Request Approval for Real
    Estate Showing** 으로 변경합니다.

![Screenshot](./media/image50.png)

53. 화면 오른쪽 상단에 있는 **Save** 버튼을 선택하여 흐름을 저장합니다.

![](./media/image51.png)

54. 흐름 이름 앞에 있는 **back arrow** 를 선택합니다.

![Screenshot](./media/image52.png)

55. **OK**를 선택합니다.

![](./media/image53.png)

56. Real estate showing요청을 제출하려면 Power Apps의 Real Estate
    Showings
    앱([**https://make.powerapps.com/**](urn:gd:lg:a:send-vm-keys) )으로
    이동합니다.

57. 왼쪽 탐색 메뉴에서 **Apps**을 선택하고 **Showings**앱을 선택한 다음,
    **Play**를 선택합니다.

![](./media/image54.png)

58. **+New**  만들기를 선택하여 새로운 상영 요청을 만듭니다.

![](./media/image55.png)

59. 다음 정보를 필드에 입력합니다:

    - **Agent Name** - \< random name \>

    - **Client Full Name** - \< Your name \>

    - **Client Email** - \< Your email \> (the email that you're using
      for this lab)

    - **Date** - \< Any future date \>

    - **Time** - \< Any future time \>

    - **Status** - Pending

    - **Address** - 210 Pine Road, Portland, OR 97204

**참고**: 이 주소는 모듈 1의 Microsoft Excel 파일에 있는 주소 중
하나이며, **Real Estate Properties**에 업로드하여 변환한 파일과
동일합니다.

일반적으로 **Real Estate Properties**에는 조회 필드가 있지만, 이
실습에서는 간편하게 하기 위해 조회 필드를 사용하지 않습니다.

![](./media/image56.png)

60. 화면 오른쪽 상단에 있는 체크 표시를 선택합니다.

![](./media/image57.png)

흐름이 실행되고, 작성한 흐름에 입력한 이메일 주소로 승인 이메일이
전송됩니다.

61. 이 실습에 사용하는 이메일 계정에 로그인하고 이메일이 도착할 때까지
    기다립니다.

**참고**: 흐름이 즉시 실행되지 않으면 잠시 기다려 주세요. 특히 첫 번째
시도에서는 흐름이 트리거되는 데 최대 10분까지 걸릴 수 있습니다.

승인 결과는 다음 이미지와 유사합니다.

![](./media/image58.png)

62. **Approve**을 선택합니다.

![](./media/image59.png)

63. 댓글을 추가한 후 **Submit**을 선택합니다.

![](./media/image60.png)

흐름은 계속 실행되며, 행을 업데이트하고 요청자에게 이메일을 전송합니다.
요청자에게 전송된 이메일은 다음 이미지와 유사합니다.

![Screenshot](./media/image61.png)

64. 흐름을 확인하고 실행 기록에서 흐름이 이제 **Succeeded** 로
    표시되었는지 확인합니다.

![](./media/image62.png)

![](./media/image63.png)
