# Lab 7 : Création, planification et affichage d'ordres de travail dans Outlook à l'aide de Copilot dans Field Service

**Remarque** : Le passage à un autre thème dans Outlook Web n'est pas
pris en charge dans les compléments Outlook.

## Exercice 1 : Ouvrir le complément Outlook de Field Service

1.  Dans un nouvel onglet, ouvrez **Outlook** à l'aide du lien
    [**http://www.outlook.com/**](urn:gd:lg:a:send-vm-keys).

![](./media/image1.png)

2.  Connectez-vous à l'aide de vos informations d'identification de
    **Office 365 admin tenant** 

![](./media/image2.png)

3.  Ouvrez l'un des e-mails. Dans un e-mail, sélectionnez l' icône
    **Apps**. Si vous ne voyez pas l'icône Applications, sélectionnez
    Plus d'options (...), puis sélectionnez les Applications.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image3.png)

4.  Sélectionnez l **'**application **Dynamics 365 Field Service Pour
    Outlook** .

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image4.png)

5.  Sélectionnez **Sign in to get started**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image5.png)

6.  Sélectionnez **Sign-in to Dynamics 365**.

![](./media/image6.png)

7.  Sélectionnez votre **Dynamics 365 environment**. Pour cet atelier,
    sélectionnez **Field Service Trial**  Environnement.

**Remarque :** Si vous rencontrez l'avertissement indiquant « Cet
environnement n'est pas valide pour Field Service », ignorez cet atelier
pour l'instant et essayez-le plus tard une fois que la fonctionnalité
sera mise à la disposition de cet environnement d'essai.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image7.png)

8.  Sélectionnez **Get started** .

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image8.png)

## Exercice 2 : Création d'un ordre de travail dans Outlook à l'aide de Copilot dans Field Service

1.  Dans un e-mail, ouvrez le **Field Service add-in**.

2.  Sous l' onglet **Home**, sélectionnez **Create a work order from
    email**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image9.png)

3.  Sur la page **Create work order** , utilisez le tableau suivant pour
    entrer les informations demandées, puis sélectionnez **Create**.

[TABLE]

> **Remarque** : Pour n'importe quel champ de l'ordre de travail, si une
> valeur n'est pas disponible dans la liste déroulante, sélectionnez
> **+**. L'application Field Service s'ouvre pour vous permettre de
> saisir une nouvelle valeur et ses détails. Enregistrez et fermez
> l'application Field Service. Tapez la nouvelle valeur ou sélectionnez
> **Refresh** pour ajouter la nouvelle valeur à la liste déroulante.
>
> ![Une capture d'écran d'un ordinateur Description générée
> automatiquement](./media/image10.png)

4.  Une fois l'ordre de travail créé, le numéro de l'ordre de travail
    s'affiche en haut du volet **Field Service**  La valeur par défaut
    de **System Status**  est **Unscheduled**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image11.png)

**Conseil** : Si vous souhaitez ouvrir l'ordre de travail dans Dynamics
365 Field Service app ,sélectionnez l'icône qui surgit .

![](./media/image12.png)

## Exercice 3 : Obtenir de l'aide pour planifier

Dans Outlook, la fonctionnalité d'assistance à la planification vous
permet de planifier, de reprogrammer ou de déplacer une réservation pour
un ordre de travail.

### Tâche 1 : Planifier un ordre de travail dans Outlook

La planification est basée sur la disponibilité des ressources, les
compétences, les créneaux horaires promis par le client, la proximité de
l'emplacement du client et l'unité commerciale.

1.  Sur la page **Field Service Add-in**, accédez à l' onglet **Work
    orders** , puis ouvrez un ordre de travail non planifié.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image13.png)

2.  Sur la page **Work order**  sélectionnez **Schedule** sous
    **Suggested actions**. Le système recherche les techniciens
    disponibles en fonction des exigences de l'ordre de travail, puis
    affiche des suggestions.

![Une capture d'écran d'un écran d'ordinateur Description générée
automatiquement](./media/image14.png)

3.  Si le système ne trouve pas de suggestions ou si vous ne trouvez pas
    le bon technicien, utilisez plutôt le **Go to schedule board**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image15.png)

4.  Vous serez redirigé vers le **Dynamics 365 Field Service Schedule
    Board**.

5.  Assurez-vous que vous êtes en mode **Initial public view** .
    Sélectionnez **Book**  pour enregistrer l'ordre de travail.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image16.png)

6.  Sélectionnez votre ordre de travail pour le champ **Requirement** et
    sélectionnez la **ressource**.

7.  Sélectionnez la date de  **Start date**, **Start time** et **End
    date**, **End time**

8.  Sélectionnez **Book**. L'ordre de travail est maintenant réservé.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image17.png)

9.  Accédez à l' onglet **Outlook**. Le technicien est réservé et le
    statut de l'ordre de travail passe à **Scheduled**.0

![](./media/image18.png)

10. Sélectionnez **View schedule**  pour connaître plus de détails sur
    le calendrier de l'ordre de travail.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image19.png)

### Tâche 2 : Replanifier un ordre de travail dans Outlook

Replanifier un ordre de travail planifié à une ressource, une date ou
une heure différente. Utilisez l'assistant de planification pour fournir
des calendriers en fonction de la disponibilité des ressources, des
compétences, des créneaux horaires promis par le client, de la proximité
de l'emplacement du client et de l'unité commerciale.

1.  À partir de la page **Work orders**, ouvrez un ordre de travail
    planifié.

![](./media/image20.png)

2.  Sélectionnez **View schedule**  sous **Suggested actions**.

![Une capture d'écran d'un téléphone Description générée
automatiquement](./media/image21.png)

3.  Sur la page des détails de la planification, sélectionnez
    **Reschedule**.

![Une capture d'écran d'un contactez-nous Description générée
automatiquement](./media/image22.png)

4.  Sélectionnez **Go to schedule board**  pour replanifier l'ordre de
    travail.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image23.png)

5.  Passez en revue les techniciens et leur disponibilité. Vous pouvez
    rechercher un technicien par son nom, filtrer par dates ou trier les
    techniciens par heure de début ou temps de trajet. Si la **Estimated
    duration** n'a pas été configurée dans les besoins en ressources, 30
    minutes sont utilisées par défaut.

6.  Une fois l'ordre de travail reprogrammé, une confirmation s'affiche
    en haut du volet **Field Service**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image24.png)

### Tâche 3 : Déplacer une réservation dans Outlook

1.  Sur la page **Field Service Add-in**  accédez à l' onglet **Work
    orders**  puis ouvrez un ordre de travail planifié.

![](./media/image25.png)

2.  Sélectionnez **View schedule**  sous **Suggested actions**.

![Une capture d'écran d'un écran d'ordinateur Description générée
automatiquement](./media/image26.png)

3.  Sur la page des détails de l'horaire, sélectionnez **Move booking**

![Une capture d'écran d'un contactez-nous Description générée
automatiquement](./media/image27.png)

4.  Vous pouvez modifier la ressource actuelle.

5.  Sélectionnez la date et l'heure, puis sélectionnez **Update**.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image28.png)

6.  Le technicien est réservé. Une confirmation s'affiche en haut du
    volet **Field Service**.

![](./media/image29.png)

## Exercice 4 : Afficher les ordres de travail dans Outlook

1.  Dans un e-mail, ouvrez le **Field Service add-in**.

2.  Dans l' onglet **Work orders** , une liste de 50 ordres de travail
    s'affiche. L'ordre de travail le plus récent s'affiche en premier.

**Conseil** : Pour afficher plus d'ordres de travail dans l'application
Field Service, sélectionnez **See more** en bas de la liste.

![](./media/image30.png)

3.  Pour trouver un ordre de travail particulier, entrez l'ID de l'ordre
    de travail dans la zone **Find by ID**  et sélectionnez **Search**..

![](./media/image31.png)

4.  Pour filtrer les ordres de travail par statut ou par priorité,
    sélectionnez **Filter**

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image32.png)

5.  Faites votre choix, par exemple, sélectionnez les ordres de travail
    avec le statut **Scheduled**,puis sélectionnez **Apply**.

![Une capture d'écran d'un écran de connexion Description générée
automatiquement](./media/image33.png)

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image34.png)

6.  Pour supprimer un filtre, sélectionnez **Filter**, effacez chaque
    sélection, puis sélectionnez **Apply**.

![Une capture d'écran d'un formulaire de connexion Description générée
automatiquement](./media/image35.png)

## Exercice 5 : Modifier un ordre de travail dans Outlook

1.  Dans un e-mail, sur la page **Field Service Add-in** , accédez à l'
    onglet **Work orders**  puis ouvrez l'un des ordres de travail.

![Une capture d'écran d'un ordinateur Description générée
automatiquement](./media/image36.png)

**Conseil** : Utilisez **Find by ID**  ou **Filter** pour trouver
l'ordre de travail si nécessaire.

2.  Apportez les modifications nécessaires, par exemple, modifiez le
    **Substatus**  de l'ordre de travail et sélectionnez **Save**.

![Une capture d'écran d'un téléphone Description générée
automatiquement](./media/image37.png)

3.  L'ordre de travail est mis à jour. Une confirmation s'affiche en
    haut du volet **Field Service**.

![Une capture d'écran d'un téléphone Description générée
automatiquement](./media/image38.png)
