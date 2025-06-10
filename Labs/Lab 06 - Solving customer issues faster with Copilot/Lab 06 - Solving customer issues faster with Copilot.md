# Laboratorio 6: Resolver los problemas de los clientes más rápido con Copilot in Dynamics 365 Customer Service

## Ejercicio 1: Resumir casos

Copilot case resume le ayuda entender el contexto de un caso y resolver
los problemas de los clientes con eficacia. El case summary incluye
información clave como case title, customer, subject, product, priority,
case type, y description.

1.  Para navegar a su **Customer Service workspace**, vaya a **Power
    Platform admin center** con este
    enlace [**https://admin.powerplatform.microsoft.com**](urn:gd:lg:a:send-vm-keys).

2.  Seleccione la pantalla **Environments** y seleccione **Customer
    Service Trial** environment.

![](./media/image1.png)

3.  En la página **Customer Service Trial environment**, haga clic
    en **Environment URL**.

![](./media/image2.png)

4.  Se le navegará a **Customer Service workspace**. Si se le navega a
    la página Published app, seleccione **Customer Service workspace**.

Ojo: si el URL no le lleva a Customer Service workspace, cambie a la
página al hacer clic en la pestañajunto a Dynamics 365.

![A screenshot of a computer Description automatically
generated](./media/image3.png)

5.  Seleccione el **Customer Service Agent Dashboard**.

![A screenshot of a computer Description automatically
generated](./media/image4.png)

6.  Seleccione uno de los casos enlistados en **Customer Service Agent
    Dashboard**.

![A screenshot of a computer Description automatically
generated](./media/image5.png)

7.  Se aparece **Case summary** como un card en el case form. Cuando
    abre un case, se minimiza el **Summary** card por defecto.

![A screenshot of a computer Description automatically
generated](./media/image6.png)

8.  Maximice la pestaña **Summary**.

![A screenshot of a computer Description automatically
generated](./media/image7.png)

9.  Puede ver el case summary generado.

![A screenshot of a computer Description automatically
generated](./media/image8.png)

## Ejercicio 2: Redacte preguntas

1.  Desde el **Customer Service Agent Dashboard** seleccione uno de los
    casos de muestra, por ejemplo, **A Mineral Build Up in Water
    Supply**.

![A screenshot of a computer Description automatically
generated](./media/image9.png)

Puede preguntar free-form questions justo como se los preguntaría a sus
compañeros o supervisores que pudieran saber las respuestas.

2.  En el panel **Copilot**, que se abre en la parte derecha de la
    pantalla, tecle [**What is mineral built up in water
    supply?**](urn:gd:lg:a:send-vm-keys) Y seleccione el ícono **Send**.

> **Ojo**: el proceso de configurar Copilot puede llevar un poco de
> tiempo. Para optimizar su sesión de laboratorio, guarde su progreso y
> seguir a la siguiente actividad del laboratorio. Puede volver a este
> laboratorio una vez que se complete el Copilot setup para continuar
> donde lo deja.

![A screenshot of a computer Description automatically
generated](./media/image10.png)

3.  Puede ver que **Copilot** ha respondido a su pregunta.

![A screenshot of a computer Description automatically
generated](./media/image11.png)

4.  Puede preguntar más cosas como, what to do........ o cómo arreglas
    un problema de obstrucción en el smart brew system o [**What to do
    if water doesn't come consistently in smart brew
    system?**](urn:gd:lg:a:send-vm-keys) Y haga clic en el
    ícono **Send**. **Copilot** dará respuestas a sus preguntas.

![A screenshot of a computer Description automatically
generated](./media/image12.png)

5.  Con **Copilot**, puede tomar varias acciones:

    - **Preguntar una pregunta directa**: Copilot muestra una respuesta
      más relevante desde knowledge sources que su organización ha hecho
      disponible.

    - **Preguntar preguntas de seguimiento de turnos**: Si la respuesta
      de Copilot no le parece útil, puede preguntar preguntas de
      seguimiento y guiar a Copilot de una manera más natural y
      conversacional.

    - **Preguntar a Copilot para intentar una mejor respuesta**: Copilot
      también puede reformular las repuestas basadas en orientación.

Por ejemplo, **tecle**, [**Can you summarize your
response?**](urn:gd:lg:a:send-vm-keys) o [**Can you attempt a response
providing details for each of the steps you
mentioned?**](urn:gd:lg:a:send-vm-keys)

![A screenshot of a computer Description automatically
generated](./media/image13.png)

6.  Si está satisfecho con la respuesta que Copilot proporciona, puede
    usar la respuesta entera o una parte de ella para responder a la
    pregunta del cliente:

    - Copie una parte de la respuesta del Copilot en su chat o léalo en
      una conversación verbal. Seleccione el ícono **Copy** para copiar
      la respuesta entera al clipboard.

![A screenshot of a computer Description automatically
generated](./media/image14.png)

**Ojo**: Cuando está en una conversación de mensajes digitales activas,
seleccione **Send to customer** para abrir una ventana de editing donde
puede revisar la respuesta y mandárselo al cliente. También puede
cambiar los keywords del cliente para pedir al Copilot que genere una
respuesta más adecuada.

7.  Seleccione **Check sources** para ver el knowledge base o enlaces de
    website por los cual Copilot derivó la respuesta. Puede usar esta
    información adicional como un recurso o compártala con el cliente.

![A screenshot of a computer screen Description automatically
generated](./media/image15.png)

8.  Haga clic en le enlace y entonces puede ver el contenido en la parte
    izquierda.

![A screenshot of a computer Description automatically
generated](./media/image16.png)

9.  Cierre la pestaña recién abierta. Aquí en este caso 'Troubleshooting
    Brewing Issues'.

![A screenshot of a computer Description automatically
generated](./media/image17.png)

10. Para valorar la utilidad de las repuestas de Copilot, seleccione
    thumbs-up o thumbs-down.

![A screenshot of a computer Description automatically
generated](./media/image18.png)

11. Después de que se acaba la conversación del cliente, o si quiere que
    Copilot ignore la conversación, seleccione **Clear chat** en la
    parte superior del panel **Copilot**.

![A screenshot of a computer Description automatically
generated](./media/image19.png)

## Ejercicio 3: Redacte emails

1.  Seleccione una pestaña **Write an email** en el panel **Copilot**.

![A screenshot of a computer Description automatically
generated](./media/image20.png)

2.  En la página case overview, seleccione la pestaña **Related** y
    luego seleccione **Activities.**

![A screenshot of a computer Description automatically
generated](./media/image21.png)

3.  Seleccione **+New Activity \> Email**.

![A screenshot of a computer Description automatically
generated](./media/image22.png)

4.  Cuando empieza a redactar un email, Copilot abre en el panel derecho
    y y presenta con cinco prompts y un prompt personalizado:

    - **Suggest a call**: Redacta una respuesta que sugiere una llamada
      con el cliente hoy o mañana.

    - **Request more information**: Redacta una respuesta que pide más
      detalles- del cliente para resolver el problema.

    - **Empathize with feedback**: Redacta una respuesta que proporciona
      una respuesta empática a un cliente que expresa una queja.

    - **Provide product/service details**: Redacta una respuesta que
      ofrece detalles o responde a las preguntas de los clientes sobre
      un producto o servicio particular.

    - **Resolve the customer's problem**: Redacta una respuesta que
      proporciona una resolución ---y pasos de resolución si corresponde
      ---al problema del cliente.

    - **Custom**: Le permit poner su propio prompt para la respuesta.

![A screenshot of a computer Description automatically
generated](./media/image23.png)

5.  Seleccione **Resolve the customer's problem** desde la lista
    predefinida de prompts.

![A screenshot of a computer Description automatically
generated](./media/image24.png)

6.  Como puede ver, Copilot ha generado una segerencia.

![A screenshot of a computer Description automatically
generated](./media/image25.png)

7.  Ahora puede revisar la respuesta. Haga cualesquiera cambios
    necesarios, y luego seleccione **Copy to email** para copiar la
    respuesta entera a su draft. O seleccione parte de la respuesta y
    use el menú del clic derecho para copiar y pear la selección.

![A screenshot of a phone Description automatically
generated](./media/image26.png)

8.  Response ahora está disponible en body part en la parte izquierda.

![A screenshot of a computer Description automatically
generated](./media/image27.png)

9.  Ahora puede mandar el email o guardarlo.

![A screenshot of a computer Description automatically
generated](./media/image28.png)
