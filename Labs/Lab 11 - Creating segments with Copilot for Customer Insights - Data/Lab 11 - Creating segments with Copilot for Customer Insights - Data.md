# Laboratorio 11: Crear segments con Copilot for Customer Insights - Data (preview)

## Ejercicio 1: Agregue sus Datos

1.  Acceda a su **Customer Insights - Data** environment en el
    enlace [**https://home.ci.ai.dynamics.com/**](urn:gd:lg:a:send-vm-keys).
    desde la navegación izquierda, seleccione **Data** \> **Data
    sources**.

![](./media/image1.png)

Ojo: Cierre el pop up – introducing Copilot in Customer Insights – Data.

![](./media/image2.png)

2.  Seleccione **Add a data source**.

![](./media/image3.png)

3.  Seleccione **Microsoft Power Query**.

4.  Introduzca **GroceryContacts** en el **Data source** **Name** para
    el data source y seleccione **Next**.

![](./media/image4.png)

5.  En la página **Choose data source** seleccione **Text/CSV**.

![](./media/image5.png)

6.  En la página **Connection settings**, seleccione **Upload file** y
    seleccione **Browse**.

![](./media/image6.png)

7.  Seleccione **Grocery_Contacts.csv** desde **C:\LabFiles** en
    su **VM** del laboratorio. Seleccione **Open**.

![](./media/image7.png)

8.  Seleccione **Sign in**, para iniciar sesión en su cuenta.

![](./media/image8.png)

9.  Introduzca sus **Office 365 admin tenant** credentials.

![A screenshot of a computer error Description automatically
generated](./media/image9.png)

10. Seleccione **Next**.

![A screenshot of a computer Description automatically
generated](./media/image10.png)

11. En la página **Preview file data**, seleccione **Transform data**.

![](./media/image11.png)

12. En la página **Transform data**, vaya a **Transform** ribbon y
    seleccione la opción **Use first row as headers \> Use first row as
    headers**.

![](./media/image12.png)

13. Haga clic derecho en la columna **birthdate**, vaya a **Change
    type**, y seleccione **Date**.

![](./media/image13.png)

14. Seleccione las siguientes columnas al mantener presionado
    el **Ctrl**: **annualincome**, **msrc_creditscore**, **msrc_customerrelationshipduration**,
    y **msrc_distancetoneareststore**.

15. Cuando se destacan estas columnas, haga clic derecho en una de
    ellas, vaya a **Change type**, y seleccione **Decimal number**.

![](./media/image14.png)

16. En **Properties** en la parte derecha, cambie
    el **Name** a [**contact**](urn:gd:lg:a:send-vm-keys) y
    presione **Enter** key en su teclado.

![](./media/image15.png)

17. Seleccione **Next**.

![](./media/image16.png)

18. En la página **Refresh settings**, seleccione **Refresh manually**.
    Seleccione **Save**.

![A screenshot of a computer Description automatically
generated](./media/image17.png)

19. Espere a que se agregue Data source.

![A screenshot of a computer Description automatically
generated](./media/image18.png)

20. En la página **Data sources**, seleccione **Add a data source**.

![A screenshot of a computer Description automatically
generated](./media/image19.png)

21. Seleccione **Microsoft Power Query**.

22. Introduzca [**GroceryTransactions**](urn:gd:lg:a:send-vm-keys) en
    el **Data source Name** para el data source y seleccione **Next**.

![A screenshot of a computer Description automatically
generated](./media/image20.png)

23. En la página **Choose data source** seleccione **Text/CSV**.

![A screenshot of a computer Description automatically
generated](./media/image21.png)

24. En la página **Connection settings**, seleccione **Upload file** y
    luego seleccione **Browse**.

![A screenshot of a computer Description automatically
generated](./media/image22.png)

25. Seleccione **Grocery_transaction.csv** desde **C:\LabFiles** en
    su **VM** del laboratorio. Haga clic en **Open**.

![](./media/image23.png)

26. Una vez que se sube el archivo, seleccione **Next**.

![A screenshot of a computer Description automatically
generated](./media/image24.png)

27. En la página **Preview file data**, seleccione **Transform data**.

![A screenshot of a computer Description automatically
generated](./media/image25.png)

28. Como antes, vaya a **Transform** y seleccione **Use first row as
    headers \> Use first row as headers**.

![A screenshot of a computer Description automatically
generated](./media/image26.png)

29. Baje y seleccione columna **msrc_transactiontimestamp**. Haga clic
    derecho en la columna, seleccione **Change type**, y luego
    seleccione **Date/Time**.

![A screenshot of a computer Description automatically
generated](./media/image27.png)

30. Mantenga presionado el **Ctrl** key en su teclado para
    seleccionar las columnas
    **msrc_transactionamount** y **msrc_discountappliedamount**. Haga
    clic derecho en una de las columnas, vaya a **Change type**, y
    seleccione **Decimal number**.

![](./media/image28.png)

31. Seleccione **Next**.

![](./media/image29.png)

32. En la página **Refresh settings**, seleccione **Refresh manually**.
    Seleccione **Save**.

![A screenshot of a computer Description automatically
generated](./media/image30.png)

33. Espere a que se agregue el Data source.

![A screenshot of a computer Description automatically
generated](./media/image31.png)

# Ejercicio 2: Unifique sus datos

1.  En **Customer Insights - Data**, expanda **Data** en el panel de
    navegación izquierdo y seleccione **Unify**.

2.  Seleccione **Get started** en el **Customer data** area.

![A screenshot of a computer Description automatically
generated](./media/image32.png)

3.  En la página **Describe the customer data to be unified**,
    seleccione el botón **Select tables and columns**.

![A screenshot of a computer Description automatically
generated](./media/image33.png)

4.  Seleccione las tablas **contact** y **Grocery_transaction** y
    seleccione **Apply**.

![A screenshot of a computer Description automatically
generated](./media/image34.png)

5.  Seleccione la tabla **contact** y seleccione **contactid** como el
    primary key.

![A screenshot of a computer screen Description automatically
generated](./media/image35.png)

6.  Seleccione la tabla **Grocery_transaction** y
    seleccione **msrc_transactionid** como el primary key.
    Seleccione **Next**.

![A screenshot of a computer Description automatically
generated](./media/image36.png)

7.  En la página **Define deduplication rules**, haga clic en **Next**.

![A screenshot of a computer Description automatically
generated](./media/image37.png)

8.  En la página **Define matching rules**, establezca las tablas en el
    siguinte orden: **contact** and **Grocery_transaction**.

9.  Asegure que esté seleccionado el **Include all records** checkbox
    para todas las tablas.

![A screenshot of a computer Description automatically
generated](./media/image38.png)

10. Seleccione **+ Add rule** junto a la tabla **Grocery_transaction**.

![A screenshot of a computer Description automatically
generated](./media/image39.png)

11. Seleccione **contactid** y **msrc_customerid**, y nombre el
    rule [**contacttransactions**](urn:gd:lg:a:send-vm-keys).
    Seleccione **Done**.

![A screenshot of a computer Description automatically
generated](./media/image40.png)

12. Seleccione **Next**.

![A screenshot of a computer Description automatically
generated](./media/image41.png)

13. Review and edit how source data is combined into unified customer
    columns en la página **Unified data view**. Haga clic en **Next**.

![A screenshot of a computer Description automatically
generated](./media/image42.png)

14. En la página **Review and create customer profiles**,
    seleccione **Create customer profiles**.

![A screenshot of a computer Description automatically
generated](./media/image43.png)

15. Este proceso tardará unos minutos en completar.

16. Revise los campos **Customer data**, **Deduplication
    rules**, **Matching rules**, y **Unified data view** en la
    página **Unify**.

![A screenshot of a computer Description automatically
generated](./media/image44.png)

## Ejercicio 3: Cree segments con Copilot for Customer Insights - Data (preview)

1.  En **Customer Insights - Data**, vaya
    a **Insights** \> **Segments** y seleccione + **New segment** para
    crear un segment.

![A screenshot of a computer Description automatically
generated](./media/image45.png)

2.  Seleccione el ícono Copilot para abrir el panel de **Copilot**.

![A screenshot of a computer Description automatically
generated](./media/image46.png)

3.  Introduzca una descripción de su segment o elija uno de los
    suggested prompts. Por ejemplo, seleccione **Customers who have a
    loyalty membership**.

![A screenshot of a chat Description automatically
generated](./media/image47.png)

4.  Seleccione **Use** para aplicar el result a un rule.

![A screenshot of a chat Description automatically
generated](./media/image48.png)

5.  Seleccione **Run**.

![A screenshot of a computer Description automatically
generated](./media/image49.png)

6.  En la página **Review details**, introduzca **Loyalty
    membership** en el campo **Name** y luego seleccione **Run**.

![A screenshot of a computer Description automatically
generated](./media/image50.png)

7.  Se ha creado el **Loyalty membership** segment.

![A screenshot of a computer Description automatically
generated](./media/image51.png)

**Ojo**: si el segment resultante contiene [***relationship
paths***](https://learn.microsoft.com/en-us/dynamics365/customer-insights/data/relationships)
múltiples, usa el shortest path por defecto. **Edite** el segment para
cambiar el relationship path.
