# Atelier 11 : Création de segments avec Copilot pour Customer Insights - Données (aperçu)

## Exercice 1 : Ajouter vos données

1.  Accédez à votre **Customer Insights - Data**  l'aide du lien indiqué
    [**https://home.ci.ai.dynamics.com/**](urn:gd:lg:a:send-vm-keys).
    Dans le volet de navigation gauche, sélectionnez **Data** \> **Data
    sources**.

![](./media/image1.png)

Remarque : Fermez la fenêtre contextuelle – introduction de Copilot dans
Customer Insights – Données.

![](./media/image2.png)

2.  Sélectionnez **Add a data source**.

![](./media/image3.png)

3.  Sélectionnez **Microsoft Power Query**.

4.  Entrez **GroceryContacts** dans le Nom de la **source de** données
    de la source de données et sélectionnez **Next**.

![](./media/image4.png)

5.  Sur la page **Choose data source** sélectionnez **Texte/CSV**.

![](./media/image5.png)

6.  Sur la page **Connection settings** ,sélectionnez **Upload file**,
    puis **Browse**.

![](./media/image6.png)

7.  Sélectionnez **Grocery_Contacts.csv** partir de **C :\LabFiles**
    dans votre **VM** de laboratoire. Sélectionnez **Open**.

![](./media/image7.png)

8.  Sélectionnez **Sign in** pour vous connecter à votre compte.

![](./media/image8.png)

9.  Entrez vos informations d'identification de **Office 365 admin
    tenant** .

![Une capture d'écran d'une erreur informatique Description générée
automatiquement](./media/image9.png)

10. Sélectionnez **Next**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image10.png)

11. Sur la page **Preview file data** , sélectionnez **Transform Data**.

![](./media/image11.png)

12. Sur la page **Transform data** , accédez au ruban **Transform** puis
    sélectionnez l' option **Use first row as headers \> Use first row
    as headers** .

![](./media/image12.png)

13. Cliquez avec le bouton droit sur la colonne **birthdate**, accédez à
    **Change type**, puis sélectionnez **Date**.

![](./media/image13.png)

14. Sélectionnez les colonnes suivantes en maintenant la touche **Ctrl**
    de votre clavier enfoncée : **annualincome ,msrc_creditscore**,
    **msrc_customerrelationshipduration** et
    **msrc_distancetoneareststore**.

15. Lorsque ces colonnes sont mises en surbrillance, cliquez avec le
    bouton droit sur l'une d'entre elles, accédez à **Change type** ,
    puis sélectionnez **Decimal number.**

![](./media/image14.png)

16. Sous **Properties** sur le côté droit, remplacez le **Name** par
    [**contact**](urn:gd:lg:a:send-vm-keys), puis appuyez sur la touche
    **Enter** de votre clavier.

![](./media/image15.png)

17. Sélectionnez **Next**.

![](./media/image16.png)

18. Sur la page **Refresh settings**  sélectionnez **Refresh manually**.
    Sélectionnez **Save**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image17.png)

19. Attendez que la source de données soit ajoutée avec succès.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image18.png)

20. Sur la page **date sources**, sélectionnez **Add a data source**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image19.png)

21. Sélectionnez **Microsoft Power Query**.

22. Entrer[**ÉpicerieTransactions**](urn:gd:lg:a:send-vm-keys)dans
    le**N** the **Data source Name**  la source de données et
    sélectionnez **Next**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image20.png)

23. Sur la page **Choose data source**  sélectionnez **Texte/CSV**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image21.png)

24. Sur la page **Connection settings** ,sélectionnez **Upload file** et
    puis sélectionnez **Browser**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image22.png)

25. Sélectionnez **Grocery_transaction.csv** partir de **C :\LabFiles**
    dans votre **VM** de l’atelier. Cliquez sur **Open**.

![](./media/image23.png)

26. Une fois le fichier téléchargé, sélectionnez **Next**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image24.png)

27. Sur la page **Preview file data** , sélectionnez **Transform data**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image25.png)

28. Comme précédemment, accédez à **Transform** et sélectionnez **Use
    first row as headers \> Use first row as headers.**

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image26.png)

29. Faites défiler et sélectionnez la colonne
    **msrc_transactiontimestamp**. Cliquez avec le bouton droit sur la
    colonne, sélectionnez **Change type**, puis Date**/Heure**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image27.png)

30. Maintenez la touche **Ctrl** de votre clavier enfoncée pour
    sélectionner les colonnes **msrc_transactionamount** et
    **msrc_discountappliedamount**. Cliquez avec le bouton droit sur
    l'une des colonnes, accédez à **Change type**, puis sélectionnez
    **Decimal number**.

![](./media/image28.png)

31. Sélectionnez **Next**.

![](./media/image29.png)

32. Sur la page **Refresh settings** , sélectionnez **Refresh
    manually**. Sélectionnez **Save**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image30.png)

33. Attendez que la source de données soit ajoutée avec succès.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image31.png)

# Exercice 2 : Unifier vos données

1.  Dans **Customer Insights - Données**, développez **Data** dans le
    volet de navigation de gauche, puis sélectionnez **Unify**.

2.  Sélectionnez **Get started**  dans la zone **Customer data**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image32.png)

3.  Sur la page **Describe the customer data to be unified** 
    sélectionnez le bouton **Select tables and columns.**

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image33.png)

4.  Sélectionnez la table des **contact** et **de Grocery_transaction**,
    puis sélectionnez **Apply**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image34.png)

5.  Sélectionnez la table des **contacts**, puis **contactid** comme clé
    primaire.

![Une capture d'écran d'un écran d'ordinateur Description générée
automatiquement](./media/image35.png)

6.  Sélectionnez la table **Grocery_transaction**, puis sélectionnez
    **msrc_transactionid** comme clé primaire. Sélectionnez **Next**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image36.png)

7.  Sur la page **Define deduplication rules** , cliquez sur **Next**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image37.png)

8.  Sur la page **Define matching rules** . configurez les tables dans
    l'ordre suivant : **contact** et **Grocery_transaction**.

9.  Assurez-vous que la case **Include all records**  est cochée pour
    toutes les tables.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image38.png)

10. Sélectionnez **+ Add rule** en regard de la table
    **Grocery_transaction**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image39.png)

11. Choisissez **contactid** et **msrc_customerid**, puis nommez la
    règle [**contacttransactions**](urn:gd:lg:a:send-vm-keys). Choisir
    **Done**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image40.png)

12. Sélectionnez **Next**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image41.png)

13. Examinez et modifiez la façon dont les données sources sont
    combinées dans les champs client unifiés sur la **page Unified data
    view**  Cliquez sur **Next**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image42.png)

14. Sur la page **Review and create customer profiles** , sélectionnez
    **Create customer profiles**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image43.png)

15. Ce processus prendra plusieurs minutes.

16. Passez en revue le **Customer data**, **Deduplication
    rules**, **Matching rules**, et  **Unified data view**  sur la page
    **Unify**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image44.png)

## Exercice 3 : Créer des segments avec Copilot pour Customer Insights - Données (aperçu))

1.  Dans **Customer Insights - Data**, accédez à **Insights** \>
    **Segments** et sélectionnez + **New segment** pour créer un
    segment.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image45.png)

2.  Sélectionnez l'icône Copilot pour ouvrir le volet **Copilot**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image46.png)

3.  Entrez une description de votre segment ou choisissez l'une des
    invites suggérées. Par exemple, sélectionnez **Customers who have a
    loyalty membership**.

![Une capture d'écran d'un chat Description générée
automatiquement](./media/image47.png)

4.  Sélectionnez **Use** pour appliquer le résultat à une règle.

![Une capture d'écran d'un chat Description générée
automatiquement](./media/image48.png)

5.  Sélectionnez **Run**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image49.png)

6.  Sur la page **Review details**  entrez **Loyalty membership**  dans
    le champ **Name**, puis sélectionnez **Run**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image50.png)

7.  Le segment **Loyalty membership**  est maintenant créé.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image51.png)

**Remarque** : Si le segment résultant contient plusieurs
[***relationship
paths***](https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/relationships),
il utilise le chemin le plus court par défaut. **Edit** le segment pour
modifier le chemin d'accès à la relation.
