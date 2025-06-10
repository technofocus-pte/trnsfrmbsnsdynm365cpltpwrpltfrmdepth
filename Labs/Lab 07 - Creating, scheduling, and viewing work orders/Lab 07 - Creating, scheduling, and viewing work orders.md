# Lab 7: Creazione, programmazione e visualizzazione di ordini di lavoro in Outlook con Copilot in Field Service

**Nota**: Il passaggio a un tema diverso in Outlook Web non è supportato
nei componenti aggiuntivi di Outlook.

## Esercizio 1: Aprire il componente aggiuntivo Field Service Outlook

1.  In una nuova scheda apri **Outlook** utilizzando il link
    [**http://www.outlook.com/**](urn:gd:lg:a:send-vm-keys).

![](./media/image1.png)

2.  Accedere con le credenziali **Office 365 admin tenant**.

![](./media/image2.png)

3.  Apri una qualsiasi delle e-mail. Durante un'e-mail, seleziona
    l'icona **Apps**. Se l'icona App non è visualizzata, selezionare
    altre opzioni (...) e quindi selezionare App.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image3.png)

4.  Seleziona l’app **Dynamics 365 Field Service for Outlook**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image4.png)

5.  Seleziona **Sign in to get started**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image5.png)

6.  Seleziona **Sign-in to Dynamics 365**.

![](./media/image6.png)

7.  Seleziona **Dynamics 365 environment**. Per questo lab, seleziona
    l'ambiente di **Field Service Trial.**

**Nota:** se ti imbatti nell'avviso "This environment is not valid for
Field Service", per il momento salta questo lab e provalo in un secondo
momento una volta che la funzionalità sarà resa disponibile per questo
ambiente di prova.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image7.png)

8.  Seleziona **Get Started**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image8.png)

## Esercizio 2: Creare un ordine di lavoro in Outlook utilizzando Copilot in Field Service

1.  In un'e-mail, apri il **Field Service add-in**.

2.  Nella scheda **Home** selezionare **Create a work order from
    email.**

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image9.png)

3.  Nella pagina **Create work order** utilizzare la tabella seguente
    per immettere le informazioni richieste, quindi selezionare
    **Create**.

[TABLE]

> **Nota**: Per qualsiasi campo dell'ordine di lavoro, se un valore non
> è disponibile nell'elenco a discesa, selezionare **+**. Si apre l'app
> Field Service in cui puoi inserire un nuovo valore e i relativi
> dettagli. Salva e chiudi l'app Field Service. Digitare il nuovo valore
> o selezionare **Refresh** per aggiungere il nuovo valore all'elenco a
> discesa.
>
> ![Uno screenshot di un computer Descrizione generata
> automaticamente](./media/image10.png)

4.  Dopo la creazione dell'ordine di lavoro, il numero dell'ordine di
    lavoro viene visualizzato nella parte superiore del riquadro **Field
    Service**. L' impostazione predefinita **System Status** è
    **Unscheduled**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image11.png)

**Suggerimento**: Se desideri aprire l'ordine di lavoro nell'app
Dynamics 365 Field Service, seleziona l'icona a comparsa.

![](./media/image12.png)

## Esercizio 3: Ottenere assistenza per la pianificazione

In Outlook, la funzionalità di assistenza alla pianificazione consente
di pianificare, riprogrammare o spostare una prenotazione per un ordine
di lavoro.

### Attività 1: Pianificare un ordine di lavoro in Outlook

La programmazione si basa sulla disponibilità delle risorse, sulle
competenze, sugli intervalli di tempo promessi dal cliente, sulla
vicinanza alla posizione del cliente e sulla business unit.

1.  Nella pagina **Field Service Add-in**, passa alla scheda **Work
    orders**, quindi apri un ordine di lavoro non pianificato.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image13.png)

2.  Nella pagina **Work order**, seleziona **Schedule** in **Suggested
    actions**. Il sistema cerca i tecnici disponibili in base ai
    requisiti dell'ordine di lavoro e quindi visualizza i suggerimenti.

![Uno screenshot dello schermo di un computer Descrizione generata
automaticamente](./media/image14.png)

3.  Se il sistema non trova suggerimenti o non trovi il tecnico adatto,
    utilizza invece la Scheda **Go to schedule board**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image15.png)

4.  Verrà visualizzata la scheda **Dynamics 365 Field Service Schedule
    Board**.

5.  Assicurati di essere in modalità **Initial public view**. Seleziona
    **Book** per prenotare l'ordine di lavoro.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image16.png)

6.  Seleziona l'ordine di lavoro per il campo **Requirement** e
    seleziona la **Resource**.

7.  Seleziona la **Start date**, **Start time** e la **End date**, **End
    time**.

8.  Seleziona **Book**. L'ordine di lavoro è ora prenotato.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image17.png)

9.  Passare alla scheda **Outlook**. Il tecnico viene prenotato e lo
    stato dell'ordine di lavoro viene modificato in **Scheduled.**0

![](./media/image18.png)

10. Seleziona **View schedule** per conoscere altri dettagli della
    pianificazione dell'ordine di lavoro.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image19.png)

### Attività 2: Riprogrammare un ordine di lavoro in Outlook

Riprogrammare un ordine di lavoro programmato su una risorsa, una data o
un'ora diversa. Utilizza l'assistenza alla pianificazione per fornire
pianificazioni in base alla disponibilità delle risorse, alle
competenze, agli intervalli di tempo promessi dal cliente, alla
vicinanza alla posizione del cliente e alla business unit.

1.  Dalla pagina **Work orders**, apri un ordine di lavoro programmato.

![](./media/image20.png)

2.  Seleziona **View schedule** in **Suggested actions**.

![Uno screenshot di un telefono Descrizione generata
automaticamente](./media/image21.png)

3.  Nella pagina dei dettagli della pianificazione, seleziona
    **Reschedule**.

![Uno screenshot di un contattaci Descrizione generata
automaticamente](./media/image22.png)

4.  Seleziona **Go to schedule board** per riprogrammare l'ordine di
    lavoro.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image23.png)

5.  Esamina i tecnici e la loro disponibilità. È possibile cercare un
    tecnico per nome, filtrare per date o ordinare i tecnici per ora di
    inizio o tempo di viaggio. Se la **Estimated Duration** non è stata
    impostata nei requisiti delle risorse, 30 minuti viene utilizzato
    come impostazione predefinita.

6.  Una volta riprogrammato l'ordine di lavoro, viene visualizzata una
    conferma nella parte superiore del riquadro **Field Service**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image24.png)

### Attività 3: Spostare una prenotazione in Outlook

1.  Nella pagina **Field Service Add-in**, vai alla scheda **Work
    orders**, quindi apri un ordine di lavoro pianificato.

![](./media/image25.png)

2.  Seleziona **View schedule** in **Suggested actions**.

![Uno screenshot dello schermo di un computer Descrizione generata
automaticamente](./media/image26.png)

3.  Nella pagina dei dettagli della pianificazione, seleziona **Move
    booking**.

![Uno screenshot di un contattaci Descrizione generata
automaticamente](./media/image27.png)

4.  È possibile modificare la risorsa corrente.

5.  Seleziona la data e l'ora e seleziona **Update**.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image28.png)

6.  Il tecnico è prenotato. Viene visualizzata una conferma nella parte
    superiore del riquadro **Field Service**.

![](./media/image29.png)

## Esercizio 4: Visualizzare gli ordini di lavoro in Outlook

1.  In un'e-mail, apri il **Field Service add-in**.

2.  Nella scheda **Work orders** viene visualizzato un elenco di un
    massimo di 50 ordini di lavoro. L'ordine di lavoro più recente viene
    visualizzato per primo.

**Suggerimento**: per visualizzare altri ordini di lavoro nell'app Field
Service, seleziona **See more** nella parte inferiore dell'elenco.

![](./media/image30.png)

3.  Per trovare un ordine di lavoro specifico, immettere l'ID
    dell'ordine di lavoro nella casella **Find by ID** e selezionare
    **Search**.

![](./media/image31.png)

4.  Per filtrare gli ordini di lavoro in base allo stato o alla
    priorità, selezionare **Filter**

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image32.png)

5.  Fai la tua scelta, ad esempio, seleziona gli ordini di lavoro con
    stato **Scheduled** e quindi seleziona **Apply**.

![Uno screenshot di una schermata di accesso Descrizione generata
automaticamente](./media/image33.png)

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image34.png)

6.  Per rimuovere un filtro, selezionare **Filter**, deselezionare ogni
    selezione e quindi selezionare **Apply**.

![Uno screenshot di un modulo di accesso Descrizione generata
automaticamente](./media/image35.png)

## Esercizio 5: Modificare un ordine di lavoro in Outlook

1.  In un'e-mail, nella pagina del **Field Service Add-in**, passa alla
    scheda **Work orders**, quindi apri uno degli ordini di lavoro.

![Uno screenshot di un computer Descrizione generata
automaticamente](./media/image36.png)

**Suggerimento**: utilizza **Find by ID** o **Filter** per trovare
l'ordine di lavoro, se necessario.

2.  Apporta le modifiche necessarie, ad esempio modifica lo
    **Substatus** dell'ordine di lavoro e seleziona **Save**.

![Uno screenshot di un telefono Descrizione generata
automaticamente](./media/image37.png)

3.  L'ordine di lavoro viene aggiornato. Viene visualizzata una conferma
    nella parte superiore del riquadro **Field Service**.

![Uno screenshot di un telefono Descrizione generata
automaticamente](./media/image38.png)
