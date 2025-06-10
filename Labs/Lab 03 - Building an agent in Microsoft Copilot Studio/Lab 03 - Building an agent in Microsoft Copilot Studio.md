# Lab 3: Creazione di un bot in Microsoft Copilot Studio con le nuove funzionalità di intelligenza artificiale

In questo lab si creerà un bot usando Copilot in Microsoft Copilot
Studio. Inoltre, imparerai come utilizzare la funzione Conversation
Booster per migliorare le risposte del suoi bot.

1.  Accedere a **Microsoft Copilot Studio** con le credenziali del
    **Office 365** **admin** **tenant** utilizzando
    [**https://copilotstudio.microsoft.com/**](urn:gd:lg:a:send-vm-keys)

2.  Se richiesto, seleziona **United States** come paese/area
    geografica, quindi seleziona **Start free trial/Get started.**

![](./media/image1.png)

3.  Seleziona l'ambiente **Dev One** dal selettore dell'ambiente.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image2.png)

4.  Nella finestra popup **Welcome to Copilot Studio,** selezionare
    **Skip**

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image3.png)

5.  Seleziona **+Create** dal menu di navigazione a sinistra, quindi
    seleziona **New agent.**

> ![Uno screenshot di un computer Descrizione generata
> automaticamente](./media/image4.png)

Viene visualizzata la procedura guidata Crea un bot. Questa procedura
guidata consente di configurare il bot assegnandogli un nome,
selezionando la lingua e, facoltativamente, scegliendo se si desidera
migliorare le conversazioni con risposte generative.

6.  Selezionare **Skip to configure.**

> ![Uno screenshot di un computer Descrizione generata
> automaticamente](./media/image5.png)

7.  Assegna al suoi bot il nome **Real Estate Booking Service** se
    quindi fai clic su **+Add Knowledge.**

> ![Uno screenshot di un computer Descrizione generata
> automaticamente](./media/image6.png)

8.  Seleziona **Public website**.

> ![](./media/image7.png)

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image8.png)

**Nota:** dopo aver selezionato **Create**, il processo di creazione del
primo bot all'interno di un nuovo ambiente può richiedere fino a 15
minuti. I bot successivi vengono creati molto più velocemente.

9.  Sotto il collegamento alla pagina Web, inserisci il
    [**https://powerplatform.microsoft.com/**](urn:gd:lg:a:send-vm-keys)
    e quindi seleziona **Add**.

> ![Uno screenshot di un computer Descrizione generata
> automaticamente](./media/image9.png)

10. Puoi vedere il link aggiunto nel campo Collegamento pagina web, ora
    seleziona di nuovo **Add**.

> ![Uno screenshot di un computer Descrizione generata
> automaticamente](./media/image10.png)

11. Seleziona **Create**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image11.png)

12. Dopo aver creato l'agente, seleziona **Topics** dal pallet
    orizzontale sopra e quindi seleziona il menu a discesa **+ Add a
    topic**. Seleziona **Create from description with Copilot.**

> ![Uno screenshot di un computer Descrizione generata
> automaticamente](./media/image12.png)

**Nota:** se l' opzione **Create with Copilot** non viene visualizzata,
potrebbe essere necessario abilitare il supporto per l'authoring
intelligente:

a\. Selezionare l' icona **Settings** nel menu superiore, quindi
selezionare **General settings**.

b\. Impostare l' interruttore **Intelligent authoring support with**
**Copilot** su **On**.

13. Viene visualizzata una nuova finestra che ti chiede di assegnare un
    **Name your topic** e di fornire una descrizione nella sezione
    **Create a topic to...**spazio.

14. Nel campo **Name your topic**, inserisci il seguente testo:

[**Book a Real Estate Showing**](urn:gd:lg:a:send-vm-keys)

15. Nella casella **Create a topic to...** , inserisci il seguente
    testo:

Raccogli il nome completo di un utente, l'e-mail, l'indirizzo della
proprietà e la data e l'ora della presentazione

Seleziona **Create**.

![](./media/image13.png)

Viene visualizzato un nuovo argomento con le frasi trigger generate.

![](./media/image14.png)

**Nota:** ricorda che i contenuti generati potrebbero apparire in modo
diverso da quelli mostrati in questo laboratorio.

Dovrebbero essere visualizzati anche più nodi di domande, la selezione
di entità e la denominazione delle variabili.

![](./media/image15.png)

16. Cerca e quindi seleziona **What is your email address?** nodo della
    domanda.

> ![](./media/image16.png)

17. Selezionare l' icona **Edit with Copilot** nella parte superiore
    dell'area di disegno.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image17.png)

18. Seleziona il nodo della domanda **"What is your email address?**",
    seleziona **+Add**, quindi seleziona **Message variation**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image18.png)

Inserisci **Thank you** nella casella del messaggio, quindi seleziona
l'icona {X} per inserire la variabile. Selezionare Variabile **Name**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image19.png)

19. Selezionare **+sign** dopo l'ultimo nodo per aggiungere un altro
    nodo della domanda.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image20.png)

Entra **Do you want to visit again?**, selezionare **Multiple choice
option** in **Identity**, fare clic su **+New option** e immettere
**Yes** e **No** separatamente selezionando due volte +**New option.**

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image21.png)

20. Seleziona **Save** per salvare le modifiche.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image22.png)

21. Sul lato destro dello schermo, puoi vedere che il riquadro Verifica
    il suoi copilota è già aperto.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image23.png)

22. Quando viene visualizzato il messaggio **Conversation Start**, il
    bot avvierà una conversazione. In risposta, inserisci una frase
    trigger per l'argomento che hai creato:

[**I want to book a real estate
showing**](https://urn:gd:lg:a:send-vm-keys/)

[**The bot responds with the "What is your full name?" question, as
shown in the following image.**](https://urn:gd:lg:a:send-vm-keys/)* *

![Uno screenshot di una chat Descrizione generata
automaticamente](./media/image24.png)

23. Inserisci il resto delle informazioni:

> Copy
>
> Full name: \<Your name\>
>
> E-mail address: \<Your email address\>
>
> Address: 555 Oak Lane, Denver, CO 80203
>
> Date and Time: 10/10/2023 10:00 AM

![Uno screenshot di una chat Descrizione generata
automaticamente](./media/image25.png)

24. Selezionare **Yes** o **No**.

![Uno screenshot di una chat Descrizione generata
automaticamente](./media/image26.png)

25. Per testare il bot potenziato, inserisci **What is Microsoft Power
    Platform**? Il bot recupera dal sito Web le informazioni che abbiamo
    fornito durante la creazione di un bot e restituisce una risposta.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image27.png)
