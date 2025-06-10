# Lab 11: Creazione di segmenti con Copilot for Customer Insights - Data (anteprima)

## Esercizio 1: Aggiungere i data

1.  Accedi all'ambiente **Customer Insights - Data** utilizzando il link
    indicato **https://home.ci.ai.dynamics.com/**. Nel riquadro di
    spostamento a sinistra, seleziona **Data** \> **Data sources**.

![](./media/image1.png)

Nota: Chiudi il pop-up **– Introducing Copilot in Customer Insights -
Data**.

![](./media/image2.png)

2.  Seleziona **Add a data source**.

![](./media/image3.png)

3.  Selezionare **Microsoft Power Query**.

4.  Immettere **GroceryContacts** nel **Data source Name** per l'origine
    data e selezionare **Next**.

![](./media/image4.png)

5.  Nella pagina **Choose data source** selezionare **Text/CSV**.

![](./media/image5.png)

6.  Nella pagina **Connection settings** selezionare **Upload file** e
    quindi selezionare **Browse**.

![](./media/image6.png)

7.  Selezionare **Grocery_Contacts.csv** da **C:\LabFiles** nella **VM**
    del lab. Seleziona **Open**.

![](./media/image7.png)

8.  Seleziona **Sign in,** per accedere al suoi account.

![](./media/image8.png)

9.  Immettere le credenziali del **Office 365 admin tenant**.

![Uno screenshot di un errore del computer Descrizione generata
automaticamente](./media/image9.png)

10. Seleziona **Next**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image10.png)

11. Nella pagina **Preview file data,** selezionare **Transform data**.

![](./media/image11.png)

12. Nella pagina **Transform data** passare alla barra multifunzione
    **Transform** e quindi selezionare l'opzione **Use first row as
    headers \> Use first row as headers.**

![](./media/image12.png)

13. Fare clic con il pulsante destro del mouse sulla colonna
    **birthdate**, passare a **Change type** e quindi selezionare
    **Date**.

![](./media/image13.png)

14. Seleziona le seguenti colonne tenendo premuto il tasto **Ctrl**
    sulla tastiera:
    **annualincome**, **msrc_creditscore**, **msrc_customerrelationshipduration**,
    and **msrc_distancetoneareststore**.

15. Quando queste colonne sono evidenziate, fai clic con il pulsante
    destro del mouse su una di esse, vai su **Change type**, quindi
    seleziona **Decimal number**.

![](./media/image14.png)

16. In **Properties** sul lato destro, cambia il **Name** in
    [**contact**](urn:gd:lg:a:send-vm-keys) e quindi premi il tasto
    **Enter** sulla tastiera.

![](./media/image15.png)

17. Seleziona **Next**.

![](./media/image16.png)

18. Nella pagina **Refresh settings,** selezionare **Refresh manually**.
    Seleziona **Save**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image17.png)

19. Attendi che l'origine data venga aggiunta correttamente.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image18.png)

20. Nella pagina **Data sources,** selezionare **Add a data source**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image19.png)

21. Selezionare **Microsoft Power Query**.

22. Entrare [**Grocery Transactions**](urn:gd:lg:a:send-vm-keys) Nel
    **Data source Name** per l'origine data e selezionare **Next**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image20.png)

23. Nella pagina **Choose data source** selezionare **Text/CSV**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image21.png)

24. Nella pagina **Connection settings** selezionare **Upload file** e
    quindi selezionare **Browse**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image22.png)

25. Selezionare **Grocery_transaction.csv** da **C:\LabFiles** nella
    **VM** del lab. Fare clic su **Open**.

![](./media/image23.png)

26. Una volta caricato il file, selezionare **Next**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image24.png)

27. Nella pagina **Preview file data** selezionare **Transform data**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image25.png)

28. Come prima, vai su **Transform** e seleziona **Use first row as
    headers \> Use first row as headers**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image26.png)

29. Scorrere fino a e selezionare la colonna
    **msrc_transactiontimestamp**. Fare clic con il pulsante destro del
    mouse sulla colonna, scegliere **Change Type** e quindi selezionare
    **Date/Time**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image27.png)

30. Tieni premuto il tasto **Ctrl** sulla tastiera per selezionare le
    colonne **msrc_transactionamount** e **msrc_discountappliedamount**.
    Fare clic con il pulsante destro del mouse su una delle colonne,
    andare su **Change Type**, quindi selezionare **Decimal number**.

![](./media/image28.png)

31. Seleziona **Next**.

![](./media/image29.png)

32. Nella pagina **Refresh settings,** selezionare **Refresh manually**.
    Seleziona **Save**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image30.png)

33. Attendi che l'origine data venga aggiunta correttamente.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image31.png)

# Esercizio 2: Unificare i data

1.  In **Customer Insights - Data**, espandi **Data** nel riquadro di
    navigazione a sinistra, quindi seleziona **Unify**.

2.  Seleziona **Get started** nell'area **Customer data.**

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image32.png)

3.  Nella pagina **Describe the customer data to be unified**
    selezionare il pulsante **Select Tables and Columns**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image33.png)

4.  Seleziona le tabelle dei **contact** e **Grocery_transaction**,
    quindi seleziona **Apply**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image34.png)

5.  Selezionare la tabella dei **contact**, quindi selezionare
    **contactid** come chiave primaria.

![Uno screenshot dello schermo di un computer Descrizione generata
automaticamente](./media/image35.png)

6.  Selezionare la tabella **Grocery_transaction**, quindi selezionare
    **msrc_transactionid** come chiave primaria. Seleziona **Next**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image36.png)

7.  Nella pagina **Define deduplication rules**, fare clic su **Next**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image37.png)

8.  Nella pagina **Define matching rules**, imposta le tabelle nel
    seguente ordine: **contact** e **Grocery_transaction**.

9.  Assicurarsi che la casella di controllo **Include all records** sia
    selezionata per tutte le tabelle.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image38.png)

10. Seleziona **+ Add rule** accanto alla tabella
    **Grocery_transaction**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image39.png)

11. Selezionare **contactid** e **msrc_customerid,** e quindi assegnare
    un nome alla regola
    [**contacttransactions**](urn:gd:lg:a:send-vm-keys). Selezionare
    **Done**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image40.png)

12. Seleziona **Next**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image41.png)

13. Esaminare e modificare il modo in cui i data di origine vengono
    combinati nei campi unificati del cliente nella pagina **Unified
    data view**. Fare clic su **Next**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image42.png)

14. Nella pagina **Review and create customer profiles**, seleziona
    **Create customer profiles.**

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image43.png)

15. Il completamento di questo processo richiederà alcuni minuti.

16. Esamina i campi **Customer data**, **Deduplication
    rules**, **Matching rules**, e **Unified data view** nella pagina
    **Unify**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image44.png)

## Esercizio 3: Creare segmenti con Copilot for Customer Insights - Data (anteprima)

1.  In **Customer Insights - Data**, vai a **Insights** \> **Segments**
    e seleziona + **New segment** per creare un segmento.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image45.png)

2.  Selezionare l'icona Copilot per aprire il riquadro **Copilot**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image46.png)

3.  Inserisci una descrizione del segmento o scegli uno dei prompt
    suggeriti. Ad esempio, selezionare **Customers who have a loyalty
    membership. **.

![Uno screenshot di una chat Descrizione generata
automaticamente](./media/image47.png)

4.  Selezionare **Use** per applicare il risultato a una regola.

![Uno screenshot di una chat Descrizione generata
automaticamente](./media/image48.png)

5.  Seleziona **Run**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image49.png)

6.  Nella pagina **Review details** immettere **Loyalty membership** nel
    campo **Name** e quindi selezionare **Run**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image50.png)

7.  Il segmento **Loyalty membership** è stato creato.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image51.png)

**Nota**: se il segmento risultante contiene più [***relationship
paths***](https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/relationships),
per impostazione predefinita utilizza il percorso più breve. **Edit** il
segmento per cambiare il percorso della relazione.
