# Laboratório 7: Criando, agendando e exibindo ordens de serviço no Outlook usando o Copilot no Field Service

**Observação**: Alternar para um tema diferente no **Outlook Web** não é
compatível com os **complementos do Outlook**.

## Exercício 1: Abrir o complemento Field Service Outlook

1.  Em uma nova guia, abra o **Outlook** usando o link  ..

![](./media/image1.png)

2.  Faça login com suas credenciais de **Office 365 admin tenant**.

![](./media/image2.png)

3.  Abra qualquer um dos e-mails. Enquanto estiver com o e-mail aberto,
    selecione o ícone **Apps**. Se não visualizar o ícone Apps,
    selecione mais opções (…) e, em seguida, Apps.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image3.png)

4.  Selecione **Dynamics 365 Field Service for Outlook** .

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image4.png)

5.  Selecione **Sign in to get started**.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image5.png)

6.  Selecione **Sign-in to Dynamics 365**.

![](./media/image6.png)

7.  Em Select your **Dynamics 365 environment**. Selecione o ambiente
    **Field Service Trial**, nesse laboratório.

**Observação:** se aparecer um aviso dizendo "This environment is not
valid for Field service", pule este laboratório por enquanto e tente
novamente mais tarde, quando o recurso estiver disponível nesse ambiente
de teste.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image7.png)

8.  Selecione **Get started**.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image8.png)

## Exercício 2: Criar uma ordem de serviço no Outlook usando o Copilot no Field Service

1.  Enquanto estiver em um email, abra o **complemento Field Service**.

2.  Na aba **Página Inicial**, selecione **Create a work order from
    email**.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image9.png)

3.  Na página **Create work order**, use a tabela a seguir para inserir
    as informações solicitadas e selecione **Create**.

[TABLE]

> **Observação**: Para qualquer campo na ordem de serviço, se um valor
> não estiver disponível na lista suspensa, selecione **+**. O
> aplicativo Field Service será aberto para que você possa inserir um
> novo valor e seus detalhes. Salve e feche o aplicativo Field Service.
> Digite o novo valor ou selecione **Refresh** para adicionar o novo
> valor à lista suspensa.
>
> ![Uma captura de tela de um computador Descrição gerada
> automaticamente](./media/image10.png)

4.  Após a criação da ordem de serviço, o número da ordem de serviço
    será exibido na parte superior do painel do **Field Service**. O
    **System Status** padrão será **Unscheduled**.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image11.png)

**Dica**: Se você quiser abrir a ordem de serviço no aplicativo Dynamics
365 Field Service, selecione o ícone de pop-up.

![](./media/image12.png)

## Exercício 3: Obter assistência de agendamento

No Outlook, a funcionalidade de **schedule assist** ajuda você a
agendar, reagendar ou mover um agendamento para uma ordem de serviço.

### Tarefa 1: Agendar uma ordem de serviço no Outlook

O agendamento é baseado na disponibilidade de recursos, habilidades,
janelas de tempo prometidas pelo cliente, proximidade da localização do
cliente e unidade de negócios.

1.  Na página do **Field Service Add-in**, navegue até a guia **Work
    orders** e abra uma ordem de serviço que esteja com o status de
    Unscheduled.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image13.png)

2.  Na página **Worker order**, selecione **Schedule** em **Suggested
    actions**. O sistema procura por técnicos disponíveis com base nas
    necessidades da ordem de serviço e, em seguida, exibe sugestões.

![Uma captura de tela de uma tela de computador Descrição gerada
automaticamente](./media/image14.png)

3.  Se o sistema não encontrar sugestões ou você não encontrar o técnico
    ideal, utilize a opção **Go to schedule board**.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image15.png)

4.  Você será direcionado para o **Schedule Board** do **Dynamics 365
    Field Service**.

5.  Certifique-se de que está no modo **Initial public view**. Selecione
    **Book** para agendar uma ordem de serviço.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image16.png)

6.  Selecione sua ordem de serviço no campo **Requirement** e escolha o
    **Resource**.

7.  Selecione a **Start date, Start time, End date e End time**.

8.  Selecione **Book**. A ordem de serviço está reservada agora.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image17.png)

9.  Navegue até a guia **Outlook**. O técnico foi agendado e o status da
    ordem de serviço é alterado para **Scheduled.**

![](./media/image18.png)

10. Selecione **View schedule** para ver mais detalhes sobre o
    agendamento da ordem de serviço.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image19.png)

### Tarefa 2: Reagendar uma ordem de serviço no Outlook

Reagendar uma ordem de serviço agendada para um recurso, data ou hora
diferente. Use o assistente de agendamento para fornecer agendamentos
com base na disponibilidade de recursos, habilidades, janelas de tempo
prometidas pelo cliente, proximidade da localização do cliente e unidade
de negócios.

1.  Na página de **Work orders**, abra uma ordem de serviço que já
    esteja agendada.

![](./media/image20.png)

2.  Selecione **View schedule** em **Suggested actions**.

![Uma captura de tela de um telefone Descrição gerada
automaticamente](./media/image21.png)

3.  Na página de detalhes do agendamento, selecione **Reschedule**.

![Uma captura de tela de um contato Descrição gerada
automaticamente](./media/image22.png)

4.  Selecione **Go to schedule board** para reagendar a ordem de
    serviço.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image23.png)

5.  Revise os técnicos e sua disponibilidade. Você pode procurar um
    técnico pelo nome, filtrar por datas ou classificar os técnicos por
    horário de início ou tempo de viagem. Se a **Estimated Duration**
    não tiver sido configurada nos requisitos do recurso, 30 minutos
    será usado como valor padrão.

6.  Assim que a ordem de serviço for reagendada, uma confirmação será
    exibida na parte superior do painel do **Field Service**.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image24.png)

### Tarefa 3: Mover um agendamento no Outlook

1.  Na página **Field Service Add-in**, navegue até a guia **Work
    orders** e abra uma ordem de serviço agendada.

![](./media/image25.png)

2.  Selecione **View schedule** em **Suggested actions**.

![Uma captura de tela de uma tela de computador Descrição gerada
automaticamente](./media/image26.png)

3.  Na página de detalhes do agendamento, selecione **Move booking**.

![Uma captura de tela de um contato Descrição gerada
automaticamente](./media/image27.png)

4.  Você pode alterar o recurso atual.

5.  Selecione a data e a hora e selecione **Update**.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image28.png)

6.  O técnico foi agendado. Uma confirmação será exibida na parte
    superior do painel do **Field Service**.

![](./media/image29.png)

## Exercício 4: Exibir ordens de serviço no Outlook

1.  Enquanto estiver em um e-mail, abra o **Field Service add-in**.

2.  Na guia **Work orders**, será exibida uma lista de até 50 ordens de
    serviço. A ordem de serviço mais recente aparecerá primeiro.

**Dica**: Para visualizar mais ordens de serviço no aplicativo Field
Service, selecione **See more** na parte inferior da lista.

![](./media/image30.png)

3.  Para encontar uma ordem de serviço específica, digite a ID da ordem
    de serviço na na caixa **Find by ID** e selecione **Search**.

![](./media/image31.png)

4.  Para filtrar as ordens de serviço por status ou prioridade,
    selecione **Filter.**

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image32.png)

5.  Faça sua escolha, por exemplo, selecione as ordens de serviço com
    status o status **Scheduled** e, em seguida, selecione **Apply**.

![Uma captura de tela de uma tela de login Descrição gerada
automaticamente](./media/image33.png)

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image34.png)

6.  Para remover um filtro, selecione **Filter**, desmarque cada seleção
    e, em seguida, selecione **Apply**.

![Uma captura de tela de um formulário de login Descrição gerada
automaticamente](./media/image35.png)

## Exercício 5: Editar uma ordem de serviço no Outlook

1.  Enquanto estiver em um e-mail, na página do **Field Service
    Add-in**, navegue até a guia **Work orders** e depois abra qualquer
    uma das ordens de serviço.

![Uma captura de tela de um computador Descrição gerada
automaticamente](./media/image36.png)

**Dica**: Use **Find by ID** ou **Filter** para encontrar a ordem de
serviço, se necessário.

2.  Faça as alterações necessárias, por exemplo, altere o **Substatus**
    da ordem de serviço e selecione **Save**.

![Uma captura de tela de um telefone Descrição gerada
automaticamente](./media/image37.png)

3.  A ordem de serviço foi atualizada. Uma confirmação será exibida no
    topo do painel do **Field Service**.

![Uma captura de tela de um telefone Descrição gerada
automaticamente](./media/image38.png)
