# Laboratório 3: Criando um bot no Microsoft Copilot Studio com os novos recursos de AI

Neste laboratório, você criará um bot usando o Copilot no Microsoft
Copilot Studio. Além disso, aprenderá a usar o recurso Conversation
Booster para melhorar as respostas do seu bot.

1.  Faça login no **Microsoft Copilot Studio** com suas credenciais do
    **Office 365 admin tenant** usando
    [**https://copilotstudio.microsoft.com/**](https://copilotstudio.microsoft.com/)

[**admin@M365x15683240.onmicrosoft.com**](urn:gd:lg:a:send-vm-keys)

[**Cn~R2y15%7Pju3lrGdR;(HO9Y+%^70p~**](urn:gd:lg:a:send-vm-keys)

2.  Se solicitado, selecione **United States** como seu country/region
    e, em seguida, selecione **Start free trial/Get started.**

![](./media/image1.png)

3.  Selecione o ambiente **Dev One** no seletor de ambientes.

![A screenshot of a computer Description automatically
generated](./media/image2.png)

4.  Na janela pop-up **Welcome to Copilot Studio**, selecione **Skip**.

![A screenshot of a computer Description automatically
generated](./media/image3.png)

5.  Selecione **+Create** no menu de navegação à esquerda e, em seguida,
    selecione **New agent.**

> ![A screenshot of a computer Description automatically
> generated](./media/image4.png)

O assistente Create a bot será aberto. Esse assistente ajuda você a
configurar seu bot definindo um nome, selecionando o idioma e,
opcionalmente, escolhendo se deseja potencializar suas conversas com
respostas geradas por AI.

6.  Selecione **Skip to** **configure**.

> ![A screenshot of a computer Description automatically
> generated](./media/image5.png)

7.  Dê ao seu bot o nome **Real Estate Booking Service**  e clique em
    **+Add knowledge**.

![A screenshot of a computer Description automatically
generated](./media/image6.png)

8.  Selecione **Public website**.

> ![](./media/image7.png)

![A screenshot of a computer Description automatically
generated](./media/image8.png)**Observação:** Após selecionar
**Create**, o processo de criação do primeiro bot em um novo ambiente
pode levar até 15 minutos. Bots subsequentes são criados muito mais
rapidamente.

9.  No link da página da web, insira    e, em seguida, selecione
    **Add**.

> ![A screenshot of a computer Description automatically
> generated](./media/image9.png)

![A screenshot of a computer Description automatically
generated](./media/image10.png)

10. Você verá o link adicionado no campo Webpage link. Agora, selecione
    **Add** novamente.

> ![A screenshot of a computer Description automatically
> generated](./media/image11.png)

![A screenshot of a computer Description automatically
generated](./media/image12.png)

11. Selecione **Create**.

![A screenshot of a computer Description automatically
generated](./media/image13.png)

12. Com o seu agente criado, selecione **Topics** na paleta horizontal
    superior e, em seguida, selecione o menu suspenso **+ Add a topic**.
    Escolha a opção **Create from description with Copilot**.

> ![A screenshot of a computer Description automatically
> generated](./media/image14.png)

![A screenshot of a computer Description automatically
generated](./media/image15.png)

**Observação:** Se a opção **Create with Copilot** não for exibida,
talvez seja necessário habilitar o suporte à criação inteligente:

a\. Selecione o ícone de **Settings** no menu superior e, em seguida,
selecione **General settings**.

b\. Defina a opção **Intelligent authoring support with Copilot** como
**On**.

13. Uma nova janela aparecerá solicitando que você **Name your topic** e
    forneça uma descrição em **Create a topic to...**

14. No campo **Name your topic**, insira o seguinte texto:

[**Book a Real Estate Showing**](urn:gd:lg:a:send-vm-keys)

15. No campo **Create a topic to...**, insira o seguinte texto:

collect a user's full name, email, address of the property, and date and
time of the showing

Selecione **Create**.

![A screenshot of a computer Description automatically
generated](./media/image16.png)

![](./media/image17.png)

Um novo tópico é exibido com as frases de acionamento geradas.

![](./media/image18.png)

![A screenshot of a computer Description automatically
generated](./media/image19.png)

**Observação:** Lembre-se de que o conteúdo gerado pode aparecer
diferente do que é mostrado neste laboratório.

Vários nós de perguntas, seleção de entidades e nomenclatura de
variáveis também devem ser exibidos.

![](./media/image20.png)

![A screenshot of a computer Description automatically
generated](./media/image21.png)

16. Procure e selecione o nó da pergunta **What is your email address?**

> ![](./media/image22.png)

![A screenshot of a computer Description automatically
generated](./media/image23.png)

17. Selecione o ícone **Edit with Copilot** na parte superior da tela de
    criação.

![A screenshot of a computer Description automatically
generated](./media/image24.png)

18. Selecione o nó de pergunta **‘What is your email address?’**, clique
    em **+Add** e, em seguida, selecione **Message variation**.

![A screenshot of a computer Description automatically
generated](./media/image25.png)

Digite **Thank you** na caixa de mensagem e, em seguida, selecione o
ícone {X} para inserir a variável. Selecione a variável **Name**.

![A screenshot of a computer Description automatically
generated](./media/image26.png)

19. Selecione o **sinal +** após o último nó para adicionar mais um nó
    de pergunta.

![A screenshot of a computer Description automatically
generated](./media/image27.png)

Digite **Do you want to visit again?** selecione a opção **Multiple
choice** sob **Identity**, clique em **+New option** e insira **Yes** e
**No** separadamente, selecionando **+New option** duas vezes.

![A screenshot of a computer Description automatically
generated](./media/image28.png)

20. Selecione **Save** para salvar suas alterações.

![A screenshot of a computer Description automatically
generated](./media/image29.png)

21. No lado direito da tela, você verá que o painel Test your Copilot já
    está aberto.

![A screenshot of a computer Description automatically
generated](./media/image30.png)

22. Quando a mensagem **Conversation Start** aparecer, seu bot iniciará
    uma conversa. Em resposta, insira uma frase de acionamento para o
    tópico que você criou:

[**I want to book a real estate showing**](urn:gd:lg:a:send-vm-keys)

[**The bot responds with the "What is your full name?" question, as
shown in the following image.**](urn:gd:lg:a:send-vm-keys)

![A screenshot of a chat Description automatically
generated](./media/image31.png)

23. Insira as demais informações:

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

24. Selecione Yes ou No.

![A screenshot of a chat Description automatically
generated](./media/image33.png)

25. Para testar o bot otimizado, digite What is Microsoft Power
    Platform? O bot recupera as informações do site que fornecemos ao
    criar um bot e retorna uma resposta.

![A screenshot of a computer Description automatically
generated](./media/image34.png)
