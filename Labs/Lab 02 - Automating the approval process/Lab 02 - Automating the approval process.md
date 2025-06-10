# **Laboratório 2: Automatização do processo de aprovação para uma visita a um imóvel usando o Copilot**

Neste laboratório, você criará uma automação usando o Copilot no Power
Automate para automatizar o processo de aprovação de uma visita a um
imóvel. Você usará o Copilot para criar um fluxo que envia um e-mail ao
corretor imobiliário quando uma nova visita é solicitada. Em seguida, o
corretor pode aprovar ou rejeitar a solicitação de visita diretamente no
e-mail.

Siga estas etapas para criar um fluxo usando o Copilot.

1.  Faça login no Power Automate
    usando [**https://make.powerautomate.com/**](urn:gd:lg:a:send-vm-keys) com
    suas credenciais de locatário do Office 365.

2.  Selecione **United States** como country/region e clique em **Get
    started**.

![](./media/image1.png)

3.  Clique em **environment selector** e selecione o ambiente **Dev
    One**.

![](./media/image2.png)

4.  No centro da **página inicial** do Power Automate, no campo de texto
    em **Lets automate something. What should it do?** insira o seguinte
    prompt:

[**Inicie um processo de aprovação para um novo registro do Microsoft
Dataverse e atualize o registro com base no
resultado.**](urn:gd:lg:a:send-vm-keys)

Selecione o botão **Generate**.

![](./media/image3.png)

5.  Se o fluxo sugerido contiver apenas duas etapas, ou seja, Quando uma
    linha é adicionada, modificada ou excluída e Iniciar e aguardar
    aprovação, clique em **Show a different suggestion.**

![](./media/image4.png)

6.  No prompt, o Copilot fornece o esboço de um fluxo sugerido que você
    pode revisar. Para aceitar o fluxo, selecione **Next**.

![A screenshot of a computer Description automatically
generated](./media/image5.png)

7.  Verifique os aplicativos e serviços conectados. Se uma conexão não
    tiver sido estabelecida, edite-a ou corrija-a e selecione **Create
    flow**.

![](./media/image6.png)

O designer Editar com Copilot abre com seu fluxo e uma janela de chat do
Copilot à direita.![](./media/image7.png)

8.  Defina alguns parâmetros selecionando o acionador **When a row is
    added, modified or deleted**.

Um painel no lado esquerdo da tela mostra os detalhes do acionador,
incluindo um parâmetro **Table name** vazio que é necessário.

![](./media/image8.png)

9.  No menu suspenso \*\***Table name\*\***, pesquise e selecione
    **\*\*Showing\*\***.

> \*\*Observação:\*\* Selecione a tabela que foi gerada no lab1. 

![](./media/image9.png)

10. Reduza o painel When a row is added, modified or deleted usando o
    ícone de redução no canto superior direito do painel.

![A screenshot of a computer Description automatically
generated](./media/image10.png)

11. Selecione a ação **Start and wait for an approval** no fluxo.

Observe que o parâmetro **Approval Type** não está presente.

![](./media/image11.png)

12. No menu suspenso **Approval Type**, selecione **Approve/Reject –
    First to respond**.

Após selecionar **Approval Type**, mais parâmetros ficam disponíveis.

![](./media/image12.png)

13. Na janela de chat do Copilot, digite o seguinte comando:

> Add "New Request for Showing" as the Title parameter for the Start and
> wait for an approval action.
>
> \*\*Observação\*\*: use o nome da tabela da qual estamos ingerindo
> dados. Se o laboratório 1 tiver gerado alguma outra tabela, use o nome
> dessa tabela. 

O Copilot leva alguns segundos para processar o prompt. Quando o
processamento estiver concluído, o parâmetro **Title** será preenchido
com o texto do prompt.

![](./media/image13.png)

14. Para o parâmetro **Assigned To**, insira as credenciais do locatário
    do Office 365 que você está usando para este laboratório. Este
    endereço de e-mail é aquele que recebe a solicitação de
    aprovação.![](./media/image14.png)

15. Para o parâmetro **Details**, insira o seguinte texto:

> Foi criado um novo pedido para uma visita a um imóvel. Reveja os
> detalhes abaixo e aprove ou recuse o pedido:
>
> \*\*Property:\*\* \*\*Client:\*\* \*\*Client Email:\*\* \*\*Date:\*\* 
>
>  

![](./media/image15.png)

16. Coloque o cursor ao lado de **Property:** no parâmetro **Details**
    e, em seguida, selecione o ícone de raio para abrir o painel
    **Dynamic content**.

![](./media/image16.png)

17. No painel **Dynamic content**, selecione **See More** da etapa 'When
    a row is added, modified or deleted' para expandir a lista de
    dynamic content disponível.

![](./media/image17.png)

18. Role a página para baixo até encontrar o campo **Client Address** e,
    em seguida, selecione **Add**.

![](./media/image18.png)

O campo de conteúdo dinâmico **Address** agora foi adicionado ao
parâmetro **Details**.

![](./media/image19.png)

19. Repita os mesmos passos para os campos **Client**, **Client
    Email** e **Date** .

Quando terminar de preencher os demais campos, os valores devem ficar
semelhantes à imagem a seguir.

![](./media/image20.png)

20. Com o parâmetro **Details** preenchido, você pode reduzir a ação
    **Start and wait for an approval** selecionando o ícone de seta
    dupla.

![](./media/image21.png)

21. Selecione a ação **Condition**

![](./media/image22.png)

22. Selecione a caixa **Choose a value** e, em seguida, selecione
    **Outcome** no painel **Dynamic content**.

![](./media/image23.png)

23. Selecione **is equal to** para a condição e, em seguida, insira
    **Approve** no campo **Value**.

![](./media/image24.png)

24. Recolher a ação **Condition**.

![](./media/image25.png)

25. Selecione a ação **Update a row** sob o ramo **True** da condição.

![](./media/image26.png)

26. No menu suspenso **Table Name**, pesquise e selecione **Showings**.

![](./media/image27.png)

27. Selecione o campo **Row ID**, selecione **Dynamic content** e, em
    seguida, selecione **see more** em frente à etapa When a row is
    added, modified or deleted.

28. Agora, selecione o campo **Showings** unique identifier no painel
    **Dynamic content** e clique em **Add**.

![](./media/image27.png)

Sempre que você cria uma tabela no Microsoft Dataverse, uma coluna é
criada automaticamente com o mesmo nome da tabela. Essa coluna serve
como ID de pesquisa exclusiva para o registro (ou linha) que foi criado.

29. Selecione **Show all** em **Advanced parameters**.

![](./media/image28.png)

30. Selecione **Confirmed** no menu suspenso **Status**.

![](./media/image29.png)

Quando uma exibição é aprovada, o campo **Status** na tabela **Real
Estate Showings** é atualizado para **Confirmed**.

31. Recolher a ação **Update a row**.

![](./media/image30.png)

32. Selecione a ação **Update a row** sob o ramo **False** da condição.

![](./media/image31.png)

33. No menu suspenso **Table Name**, pesquise e selecione **Showings**.

34. Selecione o campo **Row ID** e, em seguida, selecione o campo de
    identificador exclusivo de **Showings** no painel de **Dynamic
    content**.

![](./media/image32.png)

35. Selecione **Show all** em **Advanced parameters**.

![Screenshot](./media/image33.png)

36. Selecione **Canceled** no menu suspenso **Status**.

![](./media/image34.png)

Quando uma exibição é rejeitada, o campo **Status** na **tabela Real
Estate Showings** é atualizado para **Canceled**.

37. Recolha a ação **Update a row**.

![](./media/image35.png)

38. Na janela de chat do Copilot, insira o seguinte prompt e, em
    seguida, envie:

[**Under the "Update a row" action for both branches in the condition,
add a new "Send an email (V2)" action**](urn:gd:lg:a:send-vm-keys)

![](./media/image36.png)

Após alguns segundos, o Copilot deve explicar o que foi feito, conforme
mostrado na imagem a seguir.

![](./media/image37.png)

39. Selecione a ação **Send an email** sob o ramo **True** da condição.

![](./media/image38.png)

40. Selecione \*\*Switch to advanced mode\*\* na linha do campo
    \*\*To\*\*, selecione **Enter custom value** e, em seguida,
    selecione o campo **Client Email** no painel de **Dynamic content**.
    (Selecione **see more** em frente à ação When a row is added,
    modified or deleted).

![](./media/image39.png)

41. No campo **Subject**, digite o seguinte texto na janela de chat do
    Copilot e pressione a tecla **Enter** no teclado:

**Add "Your request for a real estate showing has been approved" as the
Subject parameter for the Send an email action**

The **Subject** field should populate with the prompt text.

![](./media/image40.png)

42. Para o campo **Body**, insira o seguinte texto na janela de chat do
    Copilot e pressione a tecla **Enter** no teclado:

**Add "Good day - Your request for a real estate showing has been
approved. Please see below for details." as the Body parameter for the
Send an email action**

O campo **Body** deve ser preenchido com o texto do prompt.

![](./media/image41.png)

43. Insira o seguinte conteúdo após o texto do campo **Body**:

**Property:**

**Agent Name:**

**Showing Date:**

Em seguida, adicione os campos **Client Address**, **Agent Name** e
**Showing Date** do painel de **Dynamic content** nas linhas apropriadas
do texto do **Body**.

![](./media/image42.png)

44. Adicione o campo **Response summary** do painel de **Dynamic
    content** ao final do texto do campo **Body**.

![](./media/image43.png)

45. Recolha a ação **Send an email**.

![](./media/image44.png)

46. Selecione a ação **Send an email** sob o ramo **False** da condição.
    Selecione o campo **To**, remova o endereço de e-mail
    example@example.com e, em seguida, selecione o campo **Client
    Email** no painel de **Dynamic content**.

![](./media/image45.png)

47. No campo **Subject**, digite o seguinte texto na janela de chat do
    Copilot e pressione a tecla **Enter** no teclado:

[**Add "Your request for a real estate showing has been rejected" as the
Subject parameter for the Send an email
action**](urn:gd:lg:a:send-vm-keys)

![](./media/image46.png)

48. No campo **Body**, digite o seguinte texto na janela de chat do
    Copilot e pressione a tecla **Enter** no teclado:

[**Add "Good day - Your request for a real estate showing has been
rejected. Please see below for details." as the Body parameter for the
Send an email action**](urn:gd:lg:a:send-vm-keys)

![](./media/image47.png)

49. Insira o seguinte conteúdo após o texto do campo **Body**:

**Property:**

**Agent Name:**

**Showing Date:**

Em seguida, adicione os campos **Address**, **Agent Name** e **Showing
Date** do painel de **Dynamic content** nas linhas apropriadas do texto
do **Body**.

![](./media/image48.png)

50. Adicione o campo **Response summary** do painel de **Dynamic
    content** ao final do texto do campo **Body**.

![](./media/image49.png)

51. Recolha a ação **Send an email**.

52. Renomeie o fluxo para **Request Approval for Real Estate Showing**
    selecionando o texto **request approval when a Dataverse record is
    created** no canto superior esquerdo da tela.

![Screenshot](./media/image50.png)

53. Salve o fluxo selecionando o botão **Save** no canto superior
    direito da tela.

![](./media/image51.png)

54. Selecione a **back arrow** localizada antes do nome do fluxo.

![Screenshot](./media/image52.png)

55. Selecione **OK**.

![](./media/image53.png)

56. Para enviar uma solicitação de exibição de imóvel, acesse o
    aplicativo **Real Estate Showings** no Power Apps por meio do site
    [**https://make.powerapps.com/**](urn:gd:lg:a:send-vm-keys) .

57. Selecione **Apps** na navegação à esquerda, depois selecione o
    aplicativo **Showings** e, em seguida, clique em **Play**.

![](./media/image54.png)

58. Selecione **+New**  para criar uma nova solicitação de exibição.

![](./media/image55.png)

59. Preencha os campos com as informações a seguir:

    - **Agent Name** - \< nome aleatório \>

    - **Client Full Name** - \< Seu nome \>

    - **Client Email** - \< Seu email \> (o e-mail que você está usando
      para este laboratório)

    - **Date** - \< Qualquer data futura \>

    - **Time** - \< Qualquer data futura \>

    - **Status** - **Pending**

    - **Address - 210 Pine Road, Portland, OR 97204**

**Observação:** Este endereço é um dos endereços do arquivo Microsoft
Excel do Módulo 1; é o mesmo arquivo que você carregou e transformou na
tabela **Real Estate Properties**.

Normalmente, você teria um campo de pesquisa para a tabela **Real Estate
Properties**, mas neste laboratório isso foi simplificado.

![](./media/image56.png)

60. Selecione a marca de seleção no canto superior direito da tela.

![](./media/image57.png)

O fluxo é executado e envia um e-mail de aprovação para o endereço de
e-mail que você forneceu no fluxo que construiu.

61. Acesse a conta de e-mail que você está usando neste laboratório e
    aguarde a chegada do e-mail.

**Observação:** Se o fluxo não for executado imediatamente,
certifique-se de aguardar. Pode levar até 10 minutos para o fluxo ser
acionado, especialmente na primeira tentativa.

A solicitação de aprovação deve se assemelhar à imagem a seguir.

![](./media/image58.png)

62. Selecione **Approve**.

![](./media/image59.png)

63. Adicione um comentário e, em seguida, selecione **Submit**.

![](./media/image60.png)

O fluxo continua em execução; ele atualiza a linha e envia um e-mail
para o solicitante. O e-mail enviado ao solicitante se assemelha à
imagem a seguir.

![Screenshot](./media/image61.png)

64. Verifique o fluxo e observe que agora ele está marcado como
    **Succeded** no histórico de execução.

![](./media/image62.png)

![](./media/image63.png)
