- [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
  - [3.1. To-Be Scenario Mapping.](#31-to-be-scenario-mapping)
  - [3.2. User Stories.](#32-user-stories)
  - [3.3. Impact Mapping.](#33-impact-mapping)
  - [3.4. Product Backlog.](#34-product-backlog)

# Capítulo III: Requirements Specification
## 3.1. To-Be Scenario Mapping.

***Segmento 1: Agricultores***

| Steps | Busca informacion sobre agricultura | Ingresa a la app de AgriPure | Se reigstra en AgriPure | Obtiene la informacion deseada | 
| -------------- | -------------- | -------------- | -------------- | -------------- | 
| Doing | Investiga sobre superficies y cultivos e ingresa desde anuncios publicitarios | La informacion se adecua a sus necesidades | Se suscribe a AgriPure para mejorar en su cultivo | Mejorar el cuidado de su cultivo |
| Thinking | Donde puedo dejar crecer mis cultivos? | Funcionara lo que encontre en internet? | Valdra la pena pagar por ese servicio? | Como puedo seguir aprendiendo en esta app? | 
| Feeling | Concentrado | Seguro | Satisfecho | Motivado | 

***Segmento 2: Especialistas***

| Steps | Descubrimiento e interes | Descubrimiento de AgriPure | Adopcion y uso inicial | Integracion continua | 
| -------------- | -------------- | -------------- | -------------- | -------------- | 
| Doing | El especialista se cuestiona si podria enseñar sus capacidades a otros agricultores | El especialista ve que en AgriPure puede ofrecerse para ayudar a otros | El especialista agrega sus datos y se postula como especialista de la aplicacion | El especialista es contactado multiples veces por los usuarios de AgriPure|
| Thinking | Como sere capaz de apoyar a otros agricultores? | Sera esta mi oportunidad? | Espero que alguien me contacte | Me encanta este servicio, y mucho mas el hecho de ayudar a los demas. | 
| Feeling | Curiosidad | Emocion y Anticipacion | Entusiasmo | Satisfaccion | 

## 3.2. User Stories.

| Story ID | Titulo | Descripcion | Criterios de Aceptacion | Relacionado con |
|-----------|-----------|-----------|-----------|-----------|
| US001 | Registro de usuario | Como usuario deseo poder registrarme en la aplicación para poder acceder a sus beneficios | **Escenario: Registro de cuenta exitoso.** Dado que un usuario tiene una cuenta de correo electrónico Cuando el usuario completa el proceso de registro Entonces, la aplicación confirma el registro exitoso. **Escenario: Registro erróneo de cuenta.** Dado que un usuario tiene una cuenta de correo electrónico Cuando el usuario completa el proceso de registro con información incorrecta o faltante Entonces, la aplicación muestra un mensaje de error relacionado con la información ingresada. **Escenario: Iniciar sesión en cuenta existente.** Dado que un usuario ya ha registrado una cuenta en la aplicación Cuando el usuario inicia sesión en la aplicación Entonces, la aplicación permite el inicio de sesión y redirige al usuario a la pantalla principal | EP002 Opciones relacionadas a la cuenta del usuario | 
| US002 | Cerrar sesión de usuario | Como usuario deseo poder cerrar sesión en el dispositivo para proteger mi cuenta | **Escenario: Cierre de Sesión Exitoso** Dado que el usuario ha iniciado sesión en la aplicación Cuando el usuario desee cerrar su sesión Y selecciona la opción correspondiente para cerrar sesión Entonces la aplicación cierra la sesión del usuario y lo redirige a la pantalla de inicio de sesión **Escenario: Cierre de Sesión Fallido** Dado que el usuario ha iniciado sesión en la aplicación Cuando el usuario desee cerrar su sesión Y selecciona la opción correspondiente para cerrar sesión Pero ocurre un error durante el proceso de cierre de sesión, como una conexión de red interrumpida Entonces la aplicación muestra un mensaje de error que indica que no se pudo cerrar la sesión y permite al usuario intentarlo nuevamente | EP002 Opciones relacionadas a la cuenta del usuario |
| US003 | Actualización de datos del usuario | Como usuario deseo poder actualizar mis datos guardados en la aplicación para que la aplicación me funcione correctamente | **Escenario: Acceso a pestaña Información Personal.** Dado que un usuario desea actualizar sus datos Cuando el usuario ingrese a la configuracion Entonces la aplicación muestra una serie de configuraciones, incluida la opción de "Información Personal". **Escenario: Actualización de los datos.** Dado que el usuario se encuentra en la seccion de Información Personal Cuando el usuario haya actualizado todos los datos que desee Y el usuario guarda los cambios Entonces se muestra una pequeña ventana de confirmación. **Escenario: Confirmación de cambios** Dado que el usuario se encuentra en la pequeña ventana de confirmación para actualización de datos Cuando el usuario selecciona Aceptar Entonces la aplicación actualiza los datos Y muestrará un mensaje diciendo “Datos actualizados correctamente” | EP002 Opciones relacionadas a la cuenta del usuario |
| US004 | Selección de planta a sembrar | Como usuario deseo poder ingresar la planta que deseo sembrar para que la aplicación me ayude en su control | **Escenario: Ingreso de nueva planta** Dado que el usuario se encuentra en la pantalla principal Cuando el usuario agrega una Nueva planta Entonces la aplicación le solicita el nombre de la planta a sembrar **Escenario: Lista de posibles plantas buscadas** Dado que el usuario ya ingresó el nombre de la planta Cuando el usuario selecciona Buscar Entonces la aplicación le muestra todas las opciones que coincidan con el nombre ingresado **Escenario: Selección de nueva planta** Dado que el usuario visualiza la lista de posibles plantas que busca Cuando el usuario selecciona una de las opciones Entonces la aplicación muestra una serie de información Y le da la opción de Guardar nueva planta | EP001 Definición de funcionalidades de la aplicación |
| US005 | Guía de elección de tierra de sembrado | Como usuario deseo saber qué tipo de tierra debe usarse por cada tipo de planta para que la siembra sea más eficiente | **Escenario: Ver opciones de la planta guardada** Dado que el usuario se encuentra en la aplicación Cuando el usuario selecciona alguna de las plantas que ha guardado previamente Entonces la aplicación le muestra opciones **Escenario: Visualizar la información sobre el tipo de tierra** Dado que el usuario visualiza las opciones de la planta, cuando el usuario selecciona "Ver tipo de tierra", la aplicación presenta información sobre el tipo de tierra necesario para el cultivo, junto con indicaciones adicionales como el pH o el nivel de humedad. **Escenario: Ver opciones de la planta** Dado que el usuario se encuentra en la aplicación, cuando el usuario selecciona alguna de las plantas guardadas previamente, la aplicación le muestra la opción "Distancia de siembra". **Escenario: Ver distancia entre plantas** Dado que el usuario visualiza las opciones de la planta, cuando el usuario seleccione la opción "Distancia de siembra," entonces la aplicación le muestra la distancia óptima de siembra de la planta en formato de texto y gráficos. | EP001 Definición de funcionalidades de la aplicación |
| US006 | Distancia de siembra entre las plantas | Como usuario deseo saber a qué distancia debo plantar cada planta para optimizar el proceso | **Escenario: Ver opciones de la planta** Dado que el usuario se encuentra en la aplicación, cuando el usuario selecciona una de las plantas guardadas previamente, entonces la aplicación le muestra la opción "Distancia de siembra." **Escenario: Ver distancia entre plantas** Dado que el usuario visualiza las opciones de la planta, cuando el usuario seleccione la opción "Distancia de siembra," entonces la aplicación le muestra la distancia óptima de siembra de la planta en formato de texto y gráficos. | EP001 Definición de funcionalidades de la aplicación |
| US007 | Distancia de profundidad de siembra | Como usuario deseo saber a qué profundidad debo plantar cada planta para que estas crezcan de la mejor manera | **Escenario: Ver opciones de la planta** Dado que el usuario se encuentra en la aplicación, cuando el usuario selecciona alguna de las plantas guardadas previamente, entonces la aplicación le muestra la opción "Profundidad de siembra." **Escenario: Ver profundidad al plantar** Dado que el usuario visualiza las opciones de la planta, cuando el usuario seleccione la opción "Profundidad de siembra," entonces la aplicación deberá mostrar un gráfico que represente la profundidad adecuada a la que se debe sembrar la planta. | EP001 Definición de funcionalidades de la aplicación |
| US008 | Fechas de fumigación | Como usuario deseo saber cuáles son los días que debo fumigar mis plantas para que no se infecten de plagas | **Escenario: Generar fechas de fumigación**Dado que el usuario guardó una planta previamente y el usuario se encuentra en la pestaña de Opciones de la planta, cuando el usuario selecciona la opción  de Generar fechas de fumigación, la aplicación muestra en pantalla los días adecuados y los coloca en un calendario. **Escenario: Visualizar fechas en calendario** Dado que el usuario ya ha generado las fechas de fumigación para ciertas plantas, cuando el usuario ingresa al calendario desde la pantalla principal, la aplicación muestra el calendario con las fechas en las que debe fumigar la planta. | EP001 Definición de funcionalidades de la aplicación|
| US009 | Fechas de fertilización | Como usuario deseo saber en qué fechas debo fertilizar mis plantas para que crezcan y produzcan más frutos. |**Escenario: Generar fechas de fertilización** Dado que el usuario ha guardado una planta previamente y se encuentra en la pestaña de Opciones de la planta, cuando el usuario selecciona la opción de Generar fechas de fertilización, la aplicación muestra en pantalla los días adecuados y los coloca en un calendario. **Escenario: Visualizar fechas en calendario** Dado que el usuario ya generó las fechas de fertilización de ciertas plantas Cuando el usuario ingresé al calendario desde la pantalla principal Entonces la aplicación muestra el calendario con las fechas en las que debe fertilizar la planta. | EP001 Definición de funcionalidades de la aplicación|
| US010 | Contacto a Especialista | Como usuario deseo poder contactar a un especialista para que me pueda ayudar y aconsejarme. | **Escenario: Acceso a la sección Expertos** Dado que el usuario se encuentra en la pantalla principal Cuando el usuario selecciona un especialistas en la parte inferior de la pantalla Entonces la aplicación lo dirige a la sección de Expertos. **Escenario: Buscar a un especialista** Dado que el usuario se encuentra en la pestaña Expertos Cuando el usuario selecciona en una categoría que necesite ayuda Entonces la aplicación le muestra un listado de expertos que conocen el tema.**Escenario: Contactar a un especialista** Dado que el usuario se encuentra en la pestaña Expertos y encuentre a un especialista Cuando el usuario pulsa la opción de Detalles. Entonces se muestra la opción de contactar a ese especialista, al igual que ver información sobre ella. | EP001 Definición de funcionalidades de la aplicación|
| US011 | Botón call to action | Como usuario deseo que el landing page posea un botón call-to-action para poder descargar directamente hacia la aplicación | **Escenario: Presión del botón CTA** Dado que el usuario se encuentra en el landing page Cuando el usuario selecciona el botón Call to action llamado Descargar Entonces el sistema redirige a la tienda virtual que posea el dispositivo para descargar la aplicación móvil. **Escenario: Presión del botón CTA para descargar la aplicación** Dado que el usuario se encuentra en el landing page, cuando el usuario selecciona el botón Call to action (CTA) llamado "Descargar", entonces el sistema redirige automáticamente al usuario a la tienda virtual correspondiente según el dispositivo que esté utilizando.| EP003 Definición de estructura del landing page|
| US012 | Visualización de redes sociales | Como usuario deseo poder acceder a las redes sociales del startup por medio del landing page para conocer más acerca de este. | **Escenario: Visualización de redes sociales en el footer** Dado que el usuario se encuentra en el landing page, cuando el usuario desliza la página hasta el final, la aplicación muestra el footer en el cual se encuentran las redes sociales y demás información. **Escenario: Acceso a las redes sociales desde el footer** Dado que el usuario se encuentra en el landing page, cuando el usuario desliza la página hasta el final y ve el footer con las redes sociales,entonces el usuario hace clic en uno de los íconos de redes sociales que se encuentran en el footer. La aplicación abrirá la página correspondiente de la red social en una nueva pestaña o ventana del navegador| EP003 Definición de estructura del landing page|
| US013 | Visualización de características de aplicación | Como usuario deseo poder visualizar las características que posee la aplicación en el landing page para estar informado de lo que se me ofrece. | **Escenario: Visualización de las características** Dado que el usuario se encuentra en el landing page Cuando el usuario deslice la página Entonces el landing page le irá mostrando uno a uno las características y lo que ofrece la aplicación. **Escenario: Visualización de las características en el landing page** Dado que el usuario se encuentra en el landing page, cuando el usuario desliza la página hacia abajo, el landing page le muestra una serie de tarjetas o secciones, cada una describiendo una característica específica de la aplicación | EP003 Definición de estructura del landing page|
| US014 | Aplicación tolerante a fallos | Como usuario deseo que la aplicación sea tolerante a fallos para que pueda resistir el ingreso de múltiples usuarios a la vez | **Escenario: Ingreso masivo de usuarios** Dado que la aplicación está funcionando, cuando la aplicación recibe una gran cantidad de usuarios, entonces la aplicación es capaz de soportar a los usuarios y continúa con sus funciones correctamente.**Escenario: Prueba de resistencia con ingreso masivo de usuarios** Dado que la aplicación está en funcionamiento y se encuentra bajo condiciones de prueba de resistencia, cuando se simula un ingreso masivo de usuarios a la aplicación, entonces la aplicación demuestra su capacidad de ser tolerante a fallos. | EP004 Definición de requisitos no funcionales|
| US015 | Aplicación responsive | Como usuario deseo que la aplicación móvil sea totalmente responsive para poder usarlo desde distintos dispositivos | **Escenario: Usuario ingresa desde distintos dispositivos** Dado que el usuario utiliza la aplicación móvil, cuando el usuario ingresa a la aplicación desde distintos dispositivos, la aplicación se adapta a todos y continúa siendo funcional y visualmente estable.**Escenario: Usuario ingresa desde distintos dispositivos** Dado que el usuario utiliza la aplicación móvil, cuando el usuario ingresa a la aplicación desde distintos dispositivos, la aplicación se adapta a todos y continúa siendo funcional y visualmente estable. | EP004 Definición de requisitos no funcionales|
| US016 | Aplicación intuitiva | Como usuario deseo que la aplicación móvil sea intuitiva y de fácil uso para poder manejarla de manera eficiente | **Escenario: El usuario usa las funciones.** Dado que el usuario se ha registrado en la aplicación móvil, cuando el usuario decide utilizar la aplicación, entonces el usuario no tiene ningún problema en utilizar cualquiera de las funcionalidades. **Escenario: Exploración sin problemas de las funcionalidades**. Dado que el usuario ha completado el registro en la aplicación móvil, cuando el usuario decide explorar las diferentes funcionalidades de la aplicación, el usuario encuentra que cada funcionalidad es fácil de entender y utilizar. El usuario puede navegar y utilizar todas las características de la aplicación sin dificultades. | EP004 Definición de requisitos no funcionales|
| US017 | Aceptar mensajes de otros agricultores | Como especialista, deseo aceptar las solicitudes de los otros agricultores para poder apoyarlos en sus consultas | **Escenario: El especialista acepta la solicitud.** Dado que el especialista se encuentra en un chat con un agricultor, cuando acepte la opcion de "Aceptar mensajes", entonces puede iniciar la conversación con el otro agricultor. **Escenario: El especialista responde a una solicitud de chat.** Dado que el especialista está disponible para asistir a otros agricultores, cuando un agricultor envía una solicitud de chat, el especialista recibe una notificación. El especialista puede responder a la solicitud y comenzar una conversación con el agricultor que busca asesoramiento. | EP001 Definición de funcionalidades de la aplicación|
| US018 | Usar la camara para registrar cultivos | Como usuario, deseo usar la funcionalidad de camara para que pueda registrar mis cultivos de manera mas facil | **Escenario: El usuario usa la camara.** Dado que el usuario quiere registrar su cultivo, cuando va a la aplicación en la sección de fotografía y aparece la opción de encender la cámara, entonces toma una foto de su cultivo. El sistema reconoce automáticamente la imagen gracias a los datos internos de la app.**Escenario: Planta no reconocida.** Dado que el usuario desea identificar una planta desconocida en su jardín, cuando va a la aplicación en la sección de fotografía y utiliza la cámara para tomar una foto de la planta no identificada, entonces el sistema procesa la imagen. Si la planta no se encuentra en la base de datos, la aplicación muestra un mensaje indicando que la planta no pudo ser reconocida y sugiere buscar asesoramiento adicional o investigar sobre la planta de manera manual.  | EP001 Definición de funcionalidades de la aplicación|
| US019 | Seleccionar un plan | Como usuario de la aplicacion, me gustaria seleccionar uno de los planes que ofrece CropMaster| **Escenario: El usuario selecciona un plan.** Dado que el usuario quiere seleccionar un plan, cuando crea una cuenta personal, entonces le aparece la opción de escoger un plan. | EP002 Opciones relacionadas a la cuenta del usuario|
| US020 | Mejorar su Plan | Como usuario de la aplicacion, me gustaria cambiar mi plan gratis a uno premium para que pueda apreciar mejores funcionalidades | **Escenario: El usuario cambia de plan.** Dado que el usuario quiere mejorar su plan, cuando va a las opciones de su cuenta, entonces puede mejorar su plan a un precio específico. **Escenario: El usuario no puede cambiar de plan.** Dado que el usuario desea cambiar su plan actual, cuando va a las opciones de su cuenta, la aplicación le muestra un mensaje indicando que no es posible cambiar de plan Entonces, el usuario no puede cambiar su plan en ese momento y debe esperar hasta que se cumplan las condiciones necesarias para hacerlo. | EP002 Opciones relacionadas a la cuenta del usuario|
| US021 | Coordinar fechas con especialista | Como usuario de la aplicacion, me gustaria coordinar una fecha unica con el especialista para que pueda apoyarme por llamada o presencialmente | **Escenario: El especialista rechaza la fecha.** Dado que el usuario quiere coordinar una fecha, cuando selecciona la opción de coordinar fecha y el especialista la rechaza, entonces el usuario no puede realizar la reunión. **Escenario: El especialista acepta la fecha.** Dado que el usuario quiere coordinar una fecha, cuando selecciona la opción de coordinar fecha y el especialista la acepta, entonces se puede realizar la reunión. | EP001 Definición de funcionalidades de la aplicación|
| US022 | Establecer horarios de disponibilidad | Como especialista me gustaria establecer mis horarios en mi perfil para que los agricultores puedan ver mi disponibilidad | **Escenario: El especialista establece su disponibilidad.** Dado que el especialista quiere establecer su disponibilidad, cuando va a la opción de establecer horarios, entonces puede marcar las horas en las que está libre o no para que pueda ser contactado. | EP002 Opciones relacionadas a la cuenta del usuario |
| US023 | Modificar mi perfil de especialista | Como especialista me gustaria modificar mi perfil para que pueda mostrar mas informacion mia, al igual que enlaces a mis otros contactos. | **Escenario: El especialista modifiqua su perfil.** Dado que el especialista quiere modificar su perfil, cuando va a la configuración de su perfil, entonces es capaz de modificar libremente su descripción, foto de perfil y enlaces. **Escenario: El especialista no puede modificar su perfil** Dado que el especialista desea modificar su perfil para mostrar más información, cuando intenta acceder a la configuración de su perfil, entonces la aplicación muestra un mensaje de error indicando que debido a problemas técnicos, no es posible realizar cambios en el perfil en ese momento. | EP002 Opciones relacionadas a la cuenta del usuario |
| TS001 | Implementación de Seguridad | Para proteger los datos y recursos del sistema contra accesos no autorizados, el equipo de desarrollo debe implementar medidas de seguridad, incluyendo autenticación de usuarios. | **Escenario: Autenticación de Usuarios.** Los usuarios deben proporcionar credenciales válidas (nombre de usuario y contraseña) para iniciar sesión. **Escenario: Registro de Usuarios.** Los usuarios deben proporcionar información de registro, como nombre, dirección de correo electrónico y contraseña. **Escenario: Restricción de Acceso No Autorizado.** Los usuarios autenticados deben tener acceso solo a las áreas y funcionalidades para las que están autorizados.| EP006 Gestión de Datos y Comunicación Backend|
| TS002 | Creación de API Restful | Con el objetivo de permitir la comunicación eficiente entre el frontend y el backend, el equipo de desarrollo debe diseñar y crear endpoints API RESTful que sigan las mejores prácticas de diseño de APIs. | **Escenario: Diseño de Endpoints API** Se debe realizar un diseño detallado de los endpoints de la API RESTful, identificando los recursos y las operaciones que se expondrán a través de la API. **Escenario: Implementación de Endpoints API** Los endpoints deben ser funcionales y capaces de realizar las operaciones definidas, como lectura, escritura, actualización y eliminación de datos. | EP006 Gestión de Datos y Comunicación Backend
| TS003 | Integración de Servicios Externos | Para habilitar características como sistemas de reconocimiento de imagen, el equipo de desarrollo debe integrar servicios externos a través de API o SDK. | **Escenario: Selección de Servicios Externos** Se debe investigar y seleccionar los servicios externos adecuados para la integración, específicamente aquellos que permitan el reconocimiento de imágenes. **Escenario: Integración de API o SDK** Debe establecerse una conexión funcional con los servicios externos seleccionados utilizando la API o el SDK proporcionado por el proveedor del servicio. | EP006 Gestión de Datos y Comunicación Backend|
| TS004 |  Programación Asíncrona | Con el objetivo de gestionar tareas que requieren tiempo y recursos, el equipo de desarrollo debe implementar programación asíncrona utilizando bibliotecas adecuadas. |**Escenario:  Identificación de Tareas Asíncronas** Se debe identificar y documentar las tareas específicas en la aplicación que requieren programación asíncrona debido a su naturaleza que consume tiempo y recursos. **Escenario: Manejo de Errores Asíncronos** Deben implementarse mecanismos de manejo de errores para abordar posibles problemas que puedan surgir durante la ejecución de tareas asíncronas. | EP006 Gestión de Datos y Comunicación Backend|
| TS005 |  Integración de Dispositivos IoT | Con el fin de permitir a los usuarios monitorear sus plantas de manera efectiva, el equipo de desarrollo debe implementar la integración de dispositivos IoT. Esto incluye la capacidad de vincular y configurar dispositivos IoT. |**Escenario: Vinculación de Dispositivos IoT** Los usuarios deben poder iniciar el proceso de vinculación de dispositivos IoT desde la aplicación. **Escenario: Registro de Dispositivos Vinculados** La aplicación debe mantener un registro de los dispositivos IoT vinculados por cada usuario. |EP005 Integración de Dispositivos IoT|
| TS006 | Gestión de Dispositivos Vinculados | Para facilitar la administración de dispositivos vinculados, los usuarios deben poder ver una lista de sus dispositivos IoT registrados, editar su configuración y eliminar dispositivos. | **Escenario: Vista de la Lista de Dispositivos Vinculados** Los usuarios deben poder acceder a una vista que muestre una lista de todos los dispositivos IoT vinculados a sus cuentas. **Escenario: Eliminación de Dispositivos Vinculados** Los usuarios deben poder eliminar dispositivos IoT vinculados a sus cuentas si ya no desean monitorearlos. | EP005 Integración de Dispositivos IoT|
| TS007 | Visualización de Datos en la Interfaz de Usuario | Con el objetivo de brindar a los usuarios una experiencia de monitoreo efectiva, la aplicación debe mostrar los datos de los sensores en una interfaz de usuario. | **Escenario:  Diseño de la Interfaz de Usuario** Debe crearse un diseño de interfaz de usuario que muestre los datos de los sensores de manera clara y comprensible. **Escenario: Mostrar Datos de Sensores en Tiempo Real** La interfaz de usuario debe ser capaz de mostrar los datos de los sensores en tiempo real, actualizando la información automáticamente a medida que se reciben nuevos datos.|EP005 Integración de Dispositivos IoT|
| TS008 | Notificaciones y Alertas | Para mantener a los usuarios informados sobre el estado de sus plantas, la aplicación debe permitir la configuración de notificaciones y alertas basadas en datos de sensores. | **Escenario: Entrega de Notificaciones** Las notificaciones configuradas deben entregarse de manera efectiva a los usuarios a través de los canales de comunicación seleccionados. **Escenario: Configuración de Notificaciones** Deben estar disponibles opciones para habilitar o deshabilitar notificaciones y ajustar umbrales de activación.| EP005 Integración de Dispositivos IoT|

## 3.3. Impact Mapping.

***Segmento 1: Agricultores***

![Impact Map Agricultores](https://media.discordapp.net/attachments/912089666939916348/1149177185303797923/Flowchart.jpg?width=833&height=669)

***Segmento 2: Especialistas***

![Impact Map Especialistas](https://media.discordapp.net/attachments/912089666939916348/1149181676568719490/Flowchart_1.jpg?width=968&height=669)

## 3.4. Product Backlog.

| #Orden | Story ID | Titulo | Descripcion | Story Points |
|-----------|-----------|-----------|-----------|-----------|
| 1    | US004    | Selección de planta a sembrar    | Como usuario deseo poder ingresar la planta que deseo sembrar para que la aplicación me ayude en su control    | 8    |
| 2    | US005    | Guía de elección de tierra de sembrado    | Como usuario deseo saber qué tipo de tierra debe usarse por cada tipo de planta para que la siembra sea más eficiente    | 8    |
| 3    | US006    | Distancia de siembra entre las plantas    | Como usuario deseo saber a qué distancia debo plantar cada planta para optimizar el proceso   | 3    |
| 4    | US007    | Distancia de profundidad de siembra    | Como usuario deseo saber a qué profundidad debo plantar cada planta para que estas crezcan de la mejor manera    | 3    |
| 5    | US008    | Fechas de fumigación    | Como usuario deseo saber cuáles son los días que debo fumigar mis plantas para que no se infecten de plagas    | 5    |
| 6    | US009    | Fechas de fertilización    | Como usuario deseo saber en qué fechas debo fertilizar mis plantas para que crezcan y produzcan más frutos.   | 5    |
| 8    | US011    | Botón call to action    | Como usuario deseo que el landing page posea un botón call-to-action para poder descargar directamente hacia la aplicación    | 3    |
| 9    | US012    | Visualización de redes sociales    | Como usuario deseo poder acceder a las redes sociales del startup por medio del landing page para conocer más acerca de este.    | 2    |
| 10   | US013   | Visualización de características de aplicación  | Como usuario deseo poder visualizar las características que posee la aplicación en el landing page para estar informado de lo que se me ofrece.   | 3   |
| 11   | US014   | Aplicación tolerante a fallos   | Como usuario deseo que la aplicación sea tolerante a fallos para que pueda resistir el ingreso de múltiples usuarios a la vez   | 5   |
| 12   | US015   | Aplicación responsive   | Como usuario deseo que la aplicación sea totalmente responsive para poder usarlo desde distintos dispositivos  | 5   |
| 13   | US016   | Aplicación intuitiva   | Como usuario deseo que la aplicación móvil sea intuitiva y de fácil uso para poder manejarla de manera eficiente   | 5   |
| 14   | US017   | Aceptar mensajes de otros agricultores   | Como especialista, deseo aceptar las solicitudes de los otros agricultores para poder apoyarlos en sus consultas   |  5  |
| 15   | US018   | Usar la camara para registrar cultivos   | Como usuario, deseo usar la funcionalidad de camara para que pueda registrar mis cultivos de manera mas facil   |  5  |
| 16   | US019   | Seleccionar un plan   | Como usuario de la aplicacion, me gustaria seleccionar uno de los planes que ofrece AgriPure   | 8   |
| 17   | US020   | Mejorar su Plan  | Como usuario de la aplicacion, me gustaria cambiar mi plan gratis a uno premium para que pueda apreciar mejores funcionalidades   | 5   |
| 18   | US021   | Coordinar fechas con especialista   | Como usuario de la aplicacion, me gustaria coordinar una fecha unica con el especialista para que pueda apoyarme por llamada o presencialmente   | 8   |
| 19   | US022   | Establecer horarios de disponibilidad   | Como especialista me gustaria establecer mis horarios en mi perfil para que los agricultores puedan ver mi disponibilidad  | 8   |
| 20   | US023   | Modificar mi perfil de especialista   | Como especialista me gustaria modificar mi perfil para que pueda mostrar mas informacion mia, al igual que enlaces a mis otros contactos.   | 8   |
| 21   | US001   | Registro de usuario   | Como usuario deseo poder registrarme en la aplicación para poder acceder a sus beneficios   | 8   |
| 22   | US002   | Cerrar sesión de usuario   | Como usuario deseo poder cerrar sesión en el dispositivo para que nadie más pueda usar mi cuenta   | 2   |
| 23   | US003   | Actualización de datos del usuario   | Como usuario deseo poder actualizar mis datos guardados en la aplicación para que la aplicación me funcione correctamente   | 3   |
