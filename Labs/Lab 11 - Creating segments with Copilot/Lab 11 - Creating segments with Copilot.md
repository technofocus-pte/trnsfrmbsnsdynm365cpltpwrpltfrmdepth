# Lab 11: Erstellen von Segmenten mit Copilot for Customer Insights - Daten (Vorschau)

## Übung 1: Hinzufügen von Daten

1.  Greifen Sie über den angegebenen Link auf Ihre **Customer Insights -
    Datenumgebung** zu
    [**https://home.ci.ai.dynamics.com/**](https://home.ci.ai.dynamics.com/).
    Wählen Sie im linken Navigationsbereich **Data** \> **Data sources**
    aus.

![](./media/image1.png)

Hinweis: Schließen Sie das Pop-up Fenster –Copilot in Customer Insights
– Data, wird vorgestellt.

![](./media/image2.png)

2.  Wählen Sie **Add a data source** aus.

![](./media/image3.png)

3.  Wählen Sie **Microsoft Power Query** aus.

4.  Geben Sie **GroceryContacts** in **Data source** **Name** für die
    Datenquelle ein und wählen Sie dann **Next** aus.

![](./media/image4.png)

5.  Auf der Seite **Choose data source** wählen Sie **Text/CSV** aus.

![](./media/image5.png)

6.  Auf der Seite **Connection settings**, wählen Sie **Upload file**
    und wählen Sie dann **browse** aus.

![](./media/image6.png)

7.  Wählen Sie **Grocery_Contacts.csv** in **C:\LabFiles** in Ihrer
    **VM** aus. Wählen Sie **Open** aus.

![](./media/image7.png)

8.  Wählen Sie **Sign in** aus, im sich in Ihren Account einzuloggen.

![](./media/image8.png)

9.  Geben Sie Ihre **Anmeldeinformationen für den Office
    365-Administratormandanten** ein.

![A screenshot of a computer error Description automatically
generated](./media/image9.png)

10. Wählen Sie **Next** aus.

![A screenshot of a computer Description automatically
generated](./media/image10.png)

11. Auf der Seite **Preview file data**, wählen Sie **Transform data**
    aus.

![](./media/image11.png)

12. Auf der Seite **Transform data**, gehen Sie zu **Transform** und
    wählen Sie dann die Schaltfläche **Use first row as headers \> Use
    first row as headers**.

![](./media/image12.png)

13. Klicken Sie mit der rechten Maustaste auf das Symbol **birthdate**,
    gehen Sie zu **Change type**, und wählen Sie dann **Date** aus.

![](./media/image13.png)

14. Wählen Sie die folgenden Spalten aus, indem Sie die **Strg-Taste**
    auf der Tastatur gedrückt
    halten: **annualincome**, **msrc_creditscore**, **msrc_customerrelationshipduration**,
    und **msrc_distancetoneareststore**.

15. Wenn diese Spalten markiert sind, klicken Sie mit der rechten
    Maustaste auf eine der Spalten und gehen Sie zu **Change type**, und
    wählen Sie dann **Decimal number** aus.

![](./media/image14.png)

16. Unter **Properties** auf der rechten Seite, ändern Sie **Name** zu
    [**contact**](urn:gd:lg:a:send-vm-keys) und wählen Sie dann die
    **Enter** Taste auf Ihrer Tastatur.

![](./media/image15.png)

17. Wählen Sie **Next** aus.

![](./media/image16.png)

18. Auf der **Refresh settings** Seite, wählen Sie **Refresh manually**
    aus. Wählen Sie dann **Save** aus.

![A screenshot of a computer Description automatically
generated](./media/image17.png)

19. Warten Sie, bis die Data Source erfolgreich hinzugefügt wurde.

![A screenshot of a computer Description automatically
generated](./media/image18.png)

20. Auf der Seite **Data sources**, wählen Sie **Add a data source**
    aus.

![A screenshot of a computer Description automatically
generated](./media/image19.png)

21. Wählen Sie **Microsoft Power Query** aus.

22. Geben Sie [**GroceryTransactions**](urn:gd:lg:a:send-vm-keys) in
    **Data source Name** für die Datenquelle ein und wählen Sie
    **Next**.

![A screenshot of a computer Description automatically
generated](./media/image20.png)

23. Auf der Seite **Choose data source** wählen Sie **Text/CSV** aus.

![A screenshot of a computer Description automatically
generated](./media/image21.png)

24. Auf der Seite **Connection settings** wählen Sie **Upload file** und
    wählen Sie dann **Browse** aus.

![A screenshot of a computer Description automatically
generated](./media/image22.png)

25. Wählen Sie **Grocery_transaction.csv** in **C:\LabFiles** in Ihrem
    **VM- Lab**. Klicken Sie auf **Open**.

![](./media/image23.png)

26. Nachdem die Datei hochgeladen wurde, wählen Sie **Next**.

![A screenshot of a computer Description automatically
generated](./media/image24.png)

27. Auf der Seite **Preview file data**, wählen Sie **Transform data**
    aus.

![A screenshot of a computer Description automatically
generated](./media/image25.png)

28. Gehen Sie wie zuvor zu **Transform** und wählen Sie **Use first row
    as headers \> Use first row as headers** aus.

![A screenshot of a computer Description automatically
generated](./media/image26.png)

29. Scrollen Sie zur Spalte msrc_transactiontimestamp und wählen Sie sie
    aus. Klicken Sie mit der rechten Maustaste auf die Spalte, wählen
    Sie **Change Type** aus, und wählen Sie dann **Date/Time** aus.

![A screenshot of a computer Description automatically
generated](./media/image27.png)

30. Halten Sie die **Strg-Taste** auf Ihrer Tastatur gedrückt, um die
    **Spalten msrc_transactionamount** und **msrc_discountappliedamount
    auszuwählen.** Klicken Sie mit der rechten Maustaste auf eine der
    Spalten, wechseln Sie zu **Change** **Type**, und wählen Sie dann
    **Decimal number** aus.

![](./media/image28.png)

31. Wählen Sie **Next** aus.

![](./media/image29.png)

32. Auf der Seite **Refresh settings**, wählen Sie **Refresh manually**
    aus. Wählen Sie **Save** aus.

![A screenshot of a computer Description automatically
generated](./media/image30.png)

33. Warten Sie, bis die Data source erfolgreich hinzugefügt wurde.

![A screenshot of a computer Description automatically
generated](./media/image31.png)

# Übung 2: Vereinheitlichen Sie Ihre Daten

1.  In **Customer Insights - Data**, erweitern Sie **Data** im linken
    Navigationsbereich, und wählen Sie dann **Unify** aus.

2.  Wählen Sie **Get started** im **Customer data** Bereich aus.

![A screenshot of a computer Description automatically
generated](./media/image32.png)

3.  Auf der Seite **Describe the customer data to be unified**, wählen
    Sie die Schaltfläche **Select tables and columns**.

![A screenshot of a computer Description automatically
generated](./media/image33.png)

4.  Wählen Sie die Tablle **contact** und **Grocery_transaction** aus
    und wählen Sie dann **Apply** aus.

![A screenshot of a computer Description automatically
generated](./media/image34.png)

5.  Wählen Sie die Tabelle **Contact** und dann **contactid** als
    Primärschlüssel aus.

![A screenshot of a computer screen Description automatically
generated](./media/image35.png)

6.  Wählen Sie die Tabelle **Grocery_transaction** und wählen Sie dann
    **msrc_transactionid** als Primärschlüssel aus. Wählen Sie dann
    **Next** aus.

![A screenshot of a computer Description automatically
generated](./media/image36.png)

7.  Auf der Seite **Define deduplication rules**, klicken Sie auf
    **Next**.

![A screenshot of a computer Description automatically
generated](./media/image37.png)

8.  Auf der Seite **Define matching rule**, richten Sie die Tabelle in
    der folgenden Reihenfolge
    ein: **contact** und **Grocery_transaction**.

9.  Stellen Sie sicher, dass das Kontrollkästchen **Include all
    records** für alle Tabellen aktiviert ist.

![A screenshot of a computer Description automatically
generated](./media/image38.png)

10. Wählen Sie **+ Add rule** und dann die Tabelle
    **Grocery_transaction**.

![A screenshot of a computer Description automatically
generated](./media/image39.png)

11. Wählen Sie **contactid** und **msrc_customerid**, und nennen Sie
    dann die Regel [**ContactTransactions**](urn:gd:lg:a:send-vm-keys).
    Wählen Sie **Done** aus.

![A screenshot of a computer Description automatically
generated](./media/image40.png)

12. Wählen Sie **Next** aus.

![A screenshot of a computer Description automatically
generated](./media/image41.png)

13. Überprüfen und bearbeiten Sie, wie Quelldaten in einheitlichen
    Kundenfeldern auf der Seite **Unified Data View** kombiniert werden.
    Klicken Sie **Next**.

![A screenshot of a computer Description automatically
generated](./media/image42.png)

14. Auf der Seite **Review and create customer profiles**, wählen Sie
    **Create customer profiles** aus.

![A screenshot of a computer Description automatically
generated](./media/image43.png)

15. Dieser Vorgang dauert einige Minuten.

16. Überprüfen Sie die **Customer data**, **Deduplication
    rules**, **Matching rules**, und **Unified data view** auf der Seite
    **Unify**.

![A screenshot of a computer Description automatically
generated](./media/image44.png)

## Übung 3: Erstellen von Segmenten mit Copilot for Customer Insights – Daten (Vorschau)

1.  In **Customer Insights - Data**, gehen Sie
    zu **Insights** \> **Segments** und wählen Sie + **New segment,** um
    so ein Segment zu erstellen.

![A screenshot of a computer Description automatically
generated](./media/image45.png)

2.  Wählen Sie das Copilot-Symbol aus, um den **Copilot-Bereich** zu
    öffnen.

![A screenshot of a computer Description automatically
generated](./media/image46.png)

3.  Geben Sie eine Beschreibung Ihres Segments ein oder wählen Sie eine
    der vorgeschlagenen Eingabeaufforderungen aus. Wählen Sie z. B.
    **Customers who have a loyalty membership** aus.

![A screenshot of a chat Description automatically
generated](./media/image47.png)

4.  Wählen Sie **Use** aus, um das Ergebnis auf eine Regel anzuwenden.

![A screenshot of a chat Description automatically
generated](./media/image48.png)

5.  Wählen Sie **Run** aus.

![A screenshot of a computer Description automatically
generated](./media/image49.png)

6.  Auf der Seite **Review details**, geben Sie **Loyalty
    membership** in Feld **Name** ein und wählen Sie dann **Run** aus.

![A screenshot of a computer Description automatically
generated](./media/image50.png)

7.  Das Segment **Loyalty membership** wird jetzt erstellt.

![A screenshot of a computer Description automatically
generated](./media/image51.png)

**Hinweis**: Wenn das resultierende Segment mehrere [***relationship
paths***](https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/relationships),
wird standardmäßig der kürzeste Pfad verwendet. **Bearbeiten Sie** das
Segment, um den Beziehungspfad zu ändern.
