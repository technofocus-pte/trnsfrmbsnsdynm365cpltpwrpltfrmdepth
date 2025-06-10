# Laboratório 11: Criando segmentos com o Copilot para Customer Insights - Data (pré-visualização)

## Exercício 1: Adicione seus dados

1.  Acesse seu ambiente do **Customer Insights - Data** usando o link
    fornecido **https://home.ci.ai.dynamics.com/**. Na navegação à
    esquerda, selecione **Data** \>  **Data sources**.

![](./media/image1.png)

Observação: feche a janela pop-up - apresentando o Copilot in Customer
Insights - Data.

![](./media/image2.png)

2.  Selecione **Add a data source**.

![](./media/image3.png)

3.  Selecione **Microsoft Power Query**.

4.  Digite **GroceryContacts** no campo **Data source Name** para a
    fonte de dados e selecione **Next**.

![](./media/image4.png)

5.  Na página **Choose data source**, selecione **Text/CSV**.

![](./media/image5.png)

6.  Na página **Connection settings**, selecione **Upload file** e, em
    seguida, selecione **Browse**.

![](./media/image6.png)

7.  Selecione **Grocery_Contacts.csv** em **C:\LabFiles** em sua **VM**
    do laboratório. Em seguida, selecione **Open**.

![](./media/image7.png)

8.  Selecione **Sign in,** para fazer login em sua conta.

![](./media/image8.png)

9.  Insira suas credenciais do **Office 365 admin tenant.**

![A screenshot of a computer error Description automatically
generated](./media/image9.png)

10. Selecione **Next**.

![A screenshot of a computer Description automatically
generated](./media/image10.png)

11. Na página **Preview file data**, selecione **Transform data**.

![](./media/image11.png)

12. Na página **Transform data**, vá até a faixa de opções **Transform**
    e selecione a opção **Use first row as headers \> Use first row as
    headers**.

![](./media/image12.png)

13. Clique com o botão direito do mouse na coluna **birthdate**, vá até
    **Change type** e selecione **Date** .

![](./media/image13.png)

14. Selecione as seguintes colunas mantendo pressionada a tecla **Ctrl**
    no seu teclado:
    **annualincome**, **msrc_creditscore**, **msrc_customerrelationshipduration**
    e **msrc_distancetoneareststore**.

15. Quando essas colunas estiverem destacadas, clique com o botão
    direito do mouse em uma delas, vá até **Change type** e selecione
    **Decimal number**.

![](./media/image14.png)

16. Em **Properties**, no lado direito, altere o **Name** para
    **contact** e, em seguida, pressione a tecla **Enter** no seu
    teclado.

![](./media/image15.png)

17. Selecione **Next**.

![](./media/image16.png)

18. Na página **Refresh settings**, selecione **Refresh manually**. Em
    seguida, selecione **Save**.

![A screenshot of a computer Description automatically
generated](./media/image17.png)

19. Aguarde até que a fonte de dados seja adicionada com com sucesso.

![A screenshot of a computer Description automatically
generated](./media/image18.png)

20. Na página **Data sources**, selecione **Add a data source**.

![A screenshot of a computer Description automatically
generated](./media/image19.png)

21. Selecione **Microsoft Power Query**.

22. Digite **GroceryTransactions** no campo **Data source Name** para a
    fonte de dados e selecione **Next** .

![A screenshot of a computer Description automatically
generated](./media/image20.png)

23. Na página **Choose data source**, selecione **Text/CSV**.

![A screenshot of a computer Description automatically
generated](./media/image21.png)

24. Na página **Connection settings**, selecione **Upload file** e, em
    seguida, selecione **Browse**.

![A screenshot of a computer Description automatically
generated](./media/image22.png)

25. Selecione **Grocery_transaction.csv** em **C:\LabFiles** em sua
    **VM** do laboratório. Clique em **Open**.

![](./media/image23.png)

26. Depois que o arquivo for carregado, selecione **Next**.

![A screenshot of a computer Description automatically
generated](./media/image24.png)

27. Na página **Preview file data**, selecione **Transform data**.

![A screenshot of a computer Description automatically
generated](./media/image25.png)

28. Como antes, vá até **Transform** e selecione **Use first row as
    headers \> Use first row as headers**.

![A screenshot of a computer Description automatically
generated](./media/image26.png)

29. Role até a coluna **msrc_transactiontimestamp** e selecione-a.
    Clique com o botão direito do mouse na coluna, selecione **Change
    type** e, em seguida, selecione **Date/Time**.

![A screenshot of a computer Description automatically
generated](./media/image27.png)

30. Pressione e mantenha pressionada a tecla **Ctrl** no teclado para
    selecionar as colunas **msrc_transactionamount** e
    **msrc_discountappliedamount**. Clique com o botão direito do mouse
    em uma das colunas, vá para **Change type** e selecione **Decimal
    number**.

![](./media/image28.png)

31. Selecione **Next**.

![](./media/image29.png)

32. Na página **Refresh settings**, selecione **Refresh manually**. Em
    seguida, selecione **Save**.

![A screenshot of a computer Description automatically
generated](./media/image30.png)

33. Aguarde até que a fonte de dados seja adicionada com sucesso.

![A screenshot of a computer Description automatically
generated](./media/image31.png)

# Exercício 2: Unifique seus dados

1.  Em **Customer Insights - Data**, expanda **Dados** no painel de
    navegação esquerdo e selecione **Unify**.

2.  Selecione **Get started** na área de **Customer data**.

![A screenshot of a computer Description automatically
generated](./media/image32.png)

3.  Na página **Describe the customer data to be unified**, selecione o
    botão **Select tables and columns**.

![A screenshot of a computer Description automatically
generated](./media/image33.png)

4.  Selecione as tabelas **Contact** e **Grocery_transaction** e, em
    seguida, selecione **Apply**.

![A screenshot of a computer Description automatically
generated](./media/image34.png)

5.  Selecione a tabela **contact** e, em seguida, selecione
    **contactid** como a chave primária.

![A screenshot of a computer screen Description automatically
generated](./media/image35.png)

6.  Selecione a tabela **Grocery_transaction** e, em seguida, selecione
    **msrc_transactionid** como chave primária. Selecione **Next**.

![A screenshot of a computer Description automatically
generated](./media/image36.png)

7.  Na página **Define deduplication rules**, clique em **Next**.

![A screenshot of a computer Description automatically
generated](./media/image37.png)

8.  Na página **Define matching rules**, configure as tabelas na
    seguinte ordem: **contact** e **Grocery_transaction**.

9.  Certifique-se de que a caixa de seleção **Include all records**
    esteja marcada para todas as tabelas.

![A screenshot of a computer Description automatically
generated](./media/image38.png)

10. Selecione **+ Add rule** ao lado da tabela **Grocery_transaction**.

![A screenshot of a computer Description automatically
generated](./media/image39.png)

11. Selecione **contacttid** e **msrc_customerid** e, em seguida, nomeie
    a regra como **contacttransactions**. Selecione **Done**.

![A screenshot of a computer Description automatically
generated](./media/image40.png)

12. Selecione **Next**.

![A screenshot of a computer Description automatically
generated](./media/image41.png)

13. Revise e edite como os dados de origem são combinados nos campos de
    cliente unificados na página **Unified data view**. Clique em
    **Next**.

![A screenshot of a computer Description automatically
generated](./media/image42.png)

14. Na página **Review and create customer profiles**, selecione
    **Create customer profiles**.

![A screenshot of a computer Description automatically
generated](./media/image43.png)

15. Esse processo levará alguns minutos para ser concluído.

16. Revise os campos **Customer data**, **Deduplication
    rules**, **Matching rules**, and **Unified data view** na página
    **Unify**.

![A screenshot of a computer Description automatically
generated](./media/image44.png)

## Exercício 3: Criar segmentos com o Copilot para Customer Insights - Data (pré-visualização)

1.  Em **Customer Insights - Data,** acesse **Insights** \> 
    **Segments** e selecione + **New segment** para criar um segmento.

![A screenshot of a computer Description automatically
generated](./media/image45.png)

2.  Selecione o ícone do Copilot para abrir o painel do **Copilot**.

![A screenshot of a computer Description automatically
generated](./media/image46.png)

3.  Digite uma descrição de seu segmento ou escolha um dos prompts
    sugeridos. Por exemplo, selecione **Customers who have a loyalty
    membership.**![A screenshot of a chat Description automatically
    generated](./media/image47.png)

4.  Selecione **Use** para aplicar o resultado a uma regra.

![A screenshot of a chat Description automatically
generated](./media/image48.png)

5.  Selecione **Run**.

![A screenshot of a computer Description automatically
generated](./media/image49.png)

6.  Na página **Review details**, digite **Loyalty membership** no campo
    **Name** e, em seguida, selecione **Run**.

![A screenshot of a computer Description automatically
generated](./media/image50.png)

7.  O segmento **Loyalty membership** foi criado.

![A screenshot of a computer Description automatically
generated](./media/image51.png)

**Observação**: Se o segmento resultante contiver múltiplos
[***relationship
paths***](https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/relationships),
ele usará por padrão o caminho mais curto. **Edit** o segmento para
alterar o o caminho da relação.
