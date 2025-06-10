# Laboratorio 7: Crear, programar y visualizar los work orders en Outlook con Copilot in Field Service

**Ojo**: Cambiar del tema en Outlook Web no se admite en Outlook
add-ins.

## Ejercicio 1: Abra el Field Service Outlook Add-in

1.  En una nueva pestaña abra **Outlook** con el
    enlace [**http://www.outlook.com/**](urn:gd:lg:a:send-vm-keys).

![](./media/image1.png)

2.  Inicie sesión con sus **Office 365 admin tenant** credentials.

![](./media/image2.png)

3.  Abra cualquiera de los emails. Cuando está en un email, seleccione
    el ícono **Apps**. Si no ve el ícono de Apps, seleccione more
    options (…) y seleccione Apps.

![A screenshot of a computer Description automatically
generated](./media/image3.png)

4.  Seleccione el **Dynamics 365 Field Service for Outlook** app.

![A screenshot of a computer Description automatically
generated](./media/image4.png)

5.  Seleccione **Sign in to get started**.

![A screenshot of a computer Description automatically
generated](./media/image5.png)

6.  Seleccione **Sign-in to Dynamics 365**.

![](./media/image6.png)

7.  Seleccione su **Dynamics 365 environment**. Para este laboratorio,
    seleccione el **Field Service Trial** environment.

**Ojo:** Si aparece una alerta diciendo ‘This environment is not valid
for Field service’, entonces salte este laboratorio por ahora y pruebe
más tarde cuando esté disponible el feature en este entorno de prueba.

![A screenshot of a computer Description automatically
generated](./media/image7.png)

8.  Seleccione **Get started**.

![A screenshot of a computer Description automatically
generated](./media/image8.png)

## Ejercicio 2: Cree un work order en Outlook con Copilot in Field Service

1.  Cuando está en un email, abra el **Field Service add-in**.

2.  En la pestaña **Home**, seleccione **Create a work order from
    email**.

![A screenshot of a computer Description automatically
generated](./media/image9.png)

3.  En la página **Create work order**, use la siguiente table para
    introducir la información y seleccione **Create**.

[TABLE]

> **Ojo**: Para cualquier campo en el work order, si el valor no está
> disponible en la lista despegable, seleccione **+**. Se abre el Field
> Service app para que pueda introducir un nuevo valor y sus detalles.
> Guarde y cierre el Field Service app. Tecle el nuevo valor o
> seleccione **Refresh** para agregar un nuevo valor a la lista
> despegable.
>
> ![A screenshot of a computer Description automatically
> generated](./media/image10.png)

4.  Después de que se cree el work order, se ve el número de work order
    en la parte superior del panel **Field Service**. El **System
    Status** predeterminado es **Unscheduled**.

![A screenshot of a computer Description automatically
generated](./media/image11.png)

**Consejo**: Si quiere abrir el work order en Dynamics 365 Field Service
app, seleccione el ícono de maximizar.

![](./media/image12.png)

## Ejercicio 3: Obtenga schedule assistance

En Outlook, schedule assist functionality le ayuda a programar,
reprogramar o mover una reserva de work order.

### Tarea 1: Programe un work order en Outlook

La programación se basa en resource availability, skills, customer
promised time windows, customer location proximity, y business unit.

1.  En la página **Field Service Add-in**, navegue a la pestaña **Work
    orders** y luego abra un work order no programado.

![A screenshot of a computer Description automatically
generated](./media/image13.png)

2.  En la página **Work order**, seleccione **Schedule** en **Suggested
    actions**. El sistema busca técnicos disponibles en función de los
    requisitos de work order y luego mustra sugerencias.

![A screenshot of a computer screen Description automatically
generated](./media/image14.png)

3.  Si el sistema do encuentra sugerencias o si no encuentra el técnico
    justo, en su vez use el **Go to schedule board**.

![A screenshot of a computer Description automatically
generated](./media/image15.png)

4.  Se le navegará a **Dynamics 365 Field Service Schedule Board**.

5.  Asegure que está en el **Initial public view** mode.
    Seleccione **Book** para reservar el work order.

![A screenshot of a computer Description automatically
generated](./media/image16.png)

6.  Seleccione su work order para el campo **Requirement** y seleccione
    el **Resource**.

7.  Seleccione el **Start date**, **Start time** y **End date**, **End
    time**.

8.  Seleccione **Book**. Se reserva el work order ahora.

![A screenshot of a computer Description automatically
generated](./media/image17.png)

9.  Navegue a la pestaña **Outlook**. Está reservado el técnico, y el
    estado del work order se cambia a **Scheduled**.0

![](./media/image18.png)

10. Seleccione **View schedule** para saber más detalles del work order
    schedule.

![A screenshot of a computer Description automatically
generated](./media/image19.png)

### Tarea 2: Reprograme un work order en Outlook

Reprograme un work order programado a un recurso, fecha o tiempo
diferente. Use el schedule assist para proporcionar los programas en
función de la disponibilidad de recursos, habilidades, ventanas del
tiempo prometidos al cliente, la ubicación del cliente y la unidad de
empresas.

1.  Desde la página **Work orders**, abra un work order programado.

![](./media/image20.png)

2.  Seleccione **View schedule** en **Suggested actions**.

![A screenshot of a phone Description automatically
generated](./media/image21.png)

3.  En la página schedule details, seleccione **Reschedule**.

![A screenshot of a contact us Description automatically
generated](./media/image22.png)

4.  Seleccione **Go to schedule board** para reprogramar el work order.

![A screenshot of a computer Description automatically
generated](./media/image23.png)

5.  Revise los técnicos y su disponibilidad. Puede buscar al técnico por
    nombre, filtrar por fechas o reordenar los técnicos por la fecha de
    inicio o el tiempo de viaje. Si no se ha establecido
    el **Estimated** en el resource requirements, se usa 30 minutes como
    predeterminado.

6.  Una vez que se reprograme el work order, se ve una confirmación en
    la parte superior del panel **Field Service**.

![A screenshot of a computer Description automatically
generated](./media/image24.png)

### Tarea 3: Mueva una reserva en Outlook

1.  En la página **Field Service Add-in**, navegue a la pestaña **Work
    orders** y luego abra un scheduled work order.

![](./media/image25.png)

2.  Seleccione **View schedule** en **Suggested actions**.

![A screenshot of a computer screen Description automatically
generated](./media/image26.png)

3.  En la página schedule details, seleccione **Move booking**.

![A screenshot of a contact us Description automatically
generated](./media/image27.png)

4.  Puede cambiar el recurso actual.

5.  Seleccione la fecha y hora y seleccione **Update**.

![A screenshot of a computer Description automatically
generated](./media/image28.png)

6.  Se ha reservado al técnico. Se ve una confirmación en la parte
    superior del panel **Field Service**.

![](./media/image29.png)

## Ejercicio 4: Visualice los work orders en Outlook

1.  Cuando está en un email, abra el **Field Service add-in**.

2.  En la pestaña **Work orders**, aparece una lista de hasta 50 work
    orders. se ve el work order más reciente primero.

**Consejo**: Para visualizar más work orders en el Field Service app,
seleccione **See more** at the bottom of the list.

![](./media/image30.png)

3.  Para buscar un work order específico, introduzca el work order ID en
    el cuadro **Find by ID** y seleccione **Search**.

![](./media/image31.png)

4.  Para filtrar los work orders por status o priority,
    seleccione **Filter**

![A screenshot of a computer Description automatically
generated](./media/image32.png)

5.  Haga su elección, por ejemplo, seleccione los work orders con el
    status **Scheduled** y seleccione **Apply**.

![A screenshot of a login screen Description automatically
generated](./media/image33.png)

![A screenshot of a computer Description automatically
generated](./media/image34.png)

6.  Para quitar un filtro, seleccione **Filter**, borre cada selección,
    y seleccione **Apply**.

![A screenshot of a login form Description automatically
generated](./media/image35.png)

## Ejercicio 5: Edite un work order en Outlook

1.  Cuando está en un email, en la página **Field Service Add-in**,
    navegue a la pestaña **Work orders** y abra cualquira de los work
    orders.

![A screenshot of a computer Description automatically
generated](./media/image36.png)

**Consejo**: Use **Find by ID** o **Filter** para encontrar el work
order si es necesario.

2.  Haga los cambios necesarios, por ejemplo, cambie
    el **Substatus** del work order y seleccione **Save**.

![A screenshot of a phone Description automatically
generated](./media/image37.png)

3.  Se actualiza el work order. Se ve una confirmación en la parte
    encima del panel **Field Service**.

![A screenshot of a phone Description automatically
generated](./media/image38.png)
