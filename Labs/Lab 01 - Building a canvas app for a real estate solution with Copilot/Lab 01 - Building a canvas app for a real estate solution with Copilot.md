# Lab 1: Creazione di un'app canvas per una soluzione immobiliare con Copilot in Power Apps

In questo lab creerai un'applicazione per dispositivi mobili utilizzando
Copilot in Power Apps. Gli agenti sul campo utilizzeranno questa app per
sfogliare l'inventario immobiliare e gestire gli appuntamenti per le
proiezioni, mentre i data verranno archiviati in Common Data Service.

Nota: in questo laboratorio, i risultati dei data potrebbero variare da
quelli mostrati negli screenshot e nelle immagini. Il motivo è che Power
Apps usa OpenAI per generare data per il laboratorio e i data cambiano
ogni giorno.

1.  Accedi a Power Apps
    [**https://make.powerapps.com/**](urn:gd:lg:a:send-vm-keys)
    utilizzando le credenziali del tenant di Office 365.

2.  Assicurati di essere nel suoi ambiente di sviluppo - **Dev One**. In
    caso contrario, fai clic sul selettore dell'ambiente e seleziona
    **Dev One**.

![](./media/image1.png)

3.  Nella home page di Power Apps, nel campo di testo centrale, immetti
    il seguente prompt per cercare una tabella generata
    dall'intelligenza artificiale:

**Build an app to manage real estate showings **

Seleziona il pulsante **Send**.

![](./media/image2.png)

4.  Dopo che AI di Copilot ha generato le tabelle in base al prompt,
    esaminare le tabelle per visualizzare le colonne create per l'inizio
    delle tabelle.

![](./media/image3.png)

5.  Per visualizzare ulteriori informazioni, fare clic sui tre punti
    sopra la tabella.

![](./media/image3.png)

I passaggi successivi consistono nel modificare e aggiungere alla
tabella già generata.

6.  Ora fai clic sulla **Showings table** e quindi nella casella di
    testo, nella parte inferiore del riquadro Copilot a destra dello
    schermo, inserisci il seguente testo:

**Add a column to track client full name**

In questo modo verrà aggiunta una colonna nella tabella delle
visualizzazioni. Seleziona il pulsante **Send**.

![](./media/image4.png)

7.  Copilot notifica che la tabella è stata aggiornata e che la nuova
    colonna dovrebbe essere visualizzata come aggiunta alla tabella
    visualizzata. (Spostare la barra di scorrimento verso destra). Per
    visualizzare la nuova colonna aggiunta alla tabella, fare clic su
    **View data** dal riquadro orizzontale superiore.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image5.png)

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image6.png)

8.  Inserisci il seguente testo nella chat:

**Add a column to track client email **

Seleziona il pulsante **Send**.

Viene aggiunta una nuova colonna alla tabella e viene visualizzata
l'email del cliente.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image7.png)

**Nota:** i data generati nella tabella potrebbero differire dai data
mostrati nella tabella negli screenshot di questo lab.

9.  Inserisci il seguente testo nella chat:

**Add columns to track client address and agent name **

Seleziona il pulsante **Send**.

Viene aggiunta una nuova colonna alla tabella e viene visualizzata
l'email del cliente.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image8.png)

10. Inserisci il testo indicato di seguito nella chat e seleziona il
    pulsante Invia. Una nuova colonna Stato viene aggiunta alla tabella
    e visualizza l'e-mail del cliente.

**Add a column status, data type of the column is choice (Pending,
Completed, Confirmed, Cancelled**) 

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image9.png)

11. Seleziona il menu a discesa Nome colonna **Status**, quindi
    seleziona **Edit column.**

![](./media/image10.png)

12. È possibile visualizzare le proprietà delle colonne e i dettagli e i
    data sullo stato corrente. Seleziona la **X** nell'angolo in alto a
    destra di questo riquadro per chiuderlo.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image11.png)

13. Puoi vedere che le nuove scelte sono state aggiunte. Seleziona la
    **X** nell'angolo in alto a destra del riquadro per chiuderlo.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image12.png)

14. Puoi vedere che le nuove scelte sono state aggiunte.
    ![](./media/image13.png)

15. Chiudere il \*\*Copilot pane\*\*utilizzando l'icona \*\***X**\*\*,
    nell'angolo superiore destro del riquadro CoInstrument.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image14.png)

11. La tabella deve avere diverse colonne. Tuttavia, per continuare a
    seguire i moduli di questo percorso di apprendimento, provare a
    rimuovere alcune colonne che non si utilizzeranno.

L'elenco delle colonne necessarie è:

- Risultati

- Indirizzo

- Dattero

- Stato

- Nome agente

- Nome completo del cliente

- E-mail del cliente

Utilizza ciò che hai appreso con la finestra **Copilot** **Chat** per
regolare la tabella in modo che corrisponda all'elenco precedente.
Assicurarsi di fare riferimento alla sezione **Suggestions** se è
necessario rimuovere una colonna, modificare il nome di una colonna o
aggiungere una colonna.

![Immagine dello schermo](./media/image15.png)

16. Per creare l'app, seleziona il pulsante \*\***Save and Open
    App\*\*** nell'angolo in alto a destra dello schermo. Fai nuovamente
    clic su \*\***Save and Open App\*\*** sul pop-up **\*\*Done
    working?\*\*.**

![](./media/image16.png)

![](./media/image17.png)

17. Quando l'app viene caricata per la prima volta, potrebbe essere
    visualizzata una finestra di dialogo che indica **Welcome to Power
    Apps Studio**. In tal caso, selezionare il pulsante **Skip**.

![](./media/image18.png)

18. L'app che è stata creata per te dovrebbe essere visualizzata in
    modalità **Edit**.

![](./media/image19.png)

19. Per una visione migliore, chiudere il riquadro Copliot.

![](./media/image20.png)

20. Seleziona l'icona **Data** dalla barra di navigazione a sinistra.
    Copilot ha creato una tabella **Dataverse** che ora viene
    visualizzata nella sezione **Envionments**.

![](./media/image21.png)

Nota: Attualmente, Copilot è supportato solo per Common Data Service. Al
momento non è possibile utilizzare altri punti di accesso ai data.

Successivamente, modificherai la tabella ora che l'app è stata creata.

21. . Nel riquadro \*\***Data**\*\*, passa il cursore del mouse sulla
    tabella \*\*Showing\*\*. A destra della tabella, selezionare i
    puntini di sospensione (**...**) e dal menu, selezionare \*\***Edit
    data\*\***.

![](./media/image22.png)

**Nota**: Nella finestra di dialogo **Edit table**, è possibile
aggiungere colonne personalizzate alla tabella o modificare le colonne
esistenti.

22. Selezionare l'intestazione di colonna \*\*Showing\*\* dalla tabella.
    Dal menu a discesa, seleziona l'opzione \*\***Edit column\*\***

![](./media/image23.png)

23. In questo esempio, non si desidera che il **Data type** sia una
    **Single line of text**. Per modificare tale valore, passare al
    riquadro **Edit column**, quindi dal menu a discesa **Data type**,
    selezionare **\# Autonumber**. Seleziona **Save**.

![](./media/image24.png)

24. Seleziona il pulsante **Close** nell'angolo in basso a destra della
    finestra di dialogo **Edit table**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image25.png)

25. La tabella dovrebbe ora essere visualizzata come **Refreshed** nel
    riquadro **Data**.

![](./media/image26.png)

26. Modificare la raccolta nell'applicazione in modo che visualizzi i
    data pertinenti. Selezionare l'icona **Tree view** per tornare alla
    visualizzazione Struttura.

![](./media/image27.png)

27. Nella schermata principale dell'app, seleziona **RecordsGallery2**
    per visualizzare le visualizzazioni. Per selezionare
    RecirdsGallery2, seguire la gerarchia indicata di seguito.

> (Select Showings Screen \> ScreenContainer3 \> BodyContainer3 \>
> SidebarContainer3 \> RecordsGallery3).

![](./media/image28.png)

28. Ora seleziona il **edit button** di **RecordsGallery3** per mettere
    la galleria in modalità di modifica.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image29.png)

29. Fare clic sulla freccia giù su RecordGallery3, selezionare Title3 e
    quindi inserire la formula indicata di seguito.

!! ThisItem.'Client Address'!!

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image30.png)

30. Seleziona **Subtitle3** e quindi imposta il valore **Text** sulla
    seguente formula:

ThisItem.’Client Email'

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image31.png)

31. Selezionare **Body3** e quindi impostare il valore **Text** sulla
    formula seguente:

ThisItem.Status e quindi dai suggerimenti selezionare,

ThisItem.'Status (cra55_status)'

Se la formula sopra mostra un errore, usa quella seguente

ThisItem.'Location'

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image32.png)

Un singolo record nella raccolta dovrebbe ora essere simile all'immagine
seguente.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image33.png)

32. Seleziona **Form3** in **ScreenContainer3**, nell'area di disegno
    seleziona **Fields** e quindi rimuovi **Showing**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image34.png)

Poiché in precedenza hai modificato il campo **ID** in **Autonumber**,
non vuoi che gli utenti inseriscano il proprio numero; Common Data
Service inserisce automaticamente i numeri per te.

33. Effettua una nuova richiesta per una proprietà che viene
    visualizzata nell'app selezionando il pulsante **Play** nella parte
    superiore dello schermo.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image35.png)

34. Nel riquadro sinistro selezionare il pulsante **+New**.

![Immagine dello schermo](./media/image36.png)

35. Anche se è possibile modificare il modulo per compilare
    automaticamente i campi automaticamente, per questo lab si
    completerà questo passaggio manualmente per osservare come funziona
    l'app.

Compila i campi con le seguenti informazioni:

- Date: Enter any future date

- Time: 15:00

- Agent Name: [**Sarah Connor**](urn:gd:lg:a:send-vm-keys)

- Feedback: [**The property is impressive,but the kitchen needs minor
  upgrades.**](urn:gd:lg:a:send-vm-keys)

- Client Full Name: [**John Almeda**](urn:gd:lg:a:send-vm-keys)

- Client Email: [**john.almeda@example.com**](urn:gd:lg:a:send-vm-keys)

- Client Address: [**210 Pine Road, Portland, OR
  97204**](urn:gd:lg:a:send-vm-keys)

- Status: Pending

- Property: Luxury Villa

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image37.png)

36. Seleziona il segno di spunta nell'angolo in alto a destra dello
    schermo.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image38.png)

37. Seleziona la **X** nell'angolo in alto a destra per chiudere l'app.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image39.png)

Se viene visualizzata una finestra di dialogo che dice **Did you
know?**, selezionare **OK.**

![](./media/image40.png)

La nuova richiesta viene aggiunta a sinistra dell'elenco delle
richieste.

38. Nella parte superiore dello schermo, seleziona il pulsante **Save**
    per salvare la nuova app che hai creato.

Se il sistema lo richiede, salva il nome dell'app come **Real Estate
Showings**.

![Immagine dello schermo](./media/image41.png)

39. Esci dall'app per tornare alla home page di Power Apps.
