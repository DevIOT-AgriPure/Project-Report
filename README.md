## Capítulo V: Solution UI/UX Design
- 5.1. Style Guidelines.
  - 5.1.1. General Style Guidelines
  
  Con el propósito de dar estilo y reconocimiento, nuestra app web posee una gran variedad de ajustes en los temas de colores, las fuentes de tipografía y en el aspecto de diseño estructural. 
  - **Tipografía:** Avenir Light

    El tipo de letra escogida, sucesor de Avenir, resalta un tono   suave y moderno. Ofreciendo así, una visión amigable y fácil de   leer para nuestra plataforma.

  
  - 5.1.2. Web, Mobile and IoT Style Guidelines.
  
  En el presente apartado, demostraremos las decisiones que fueron tomadas en base a los estándares visuales y los diferentes tipos de interacción con respecto al responsive web interfaz.

  - **Colores:** 
    - **Color primario**
  
      HEX:  ![PrimeryColor](https://media.discordapp.net/attachments/1063259243727306824/1155576290246660096/image.png) 008000

      El color verde contiene la representación de la vegetación y los cultivos, con el tono degradé, incluyendo todo tipo de cultivos.
    - **Color secundario**
     
      HEX: ![SecondaryColor](https://media.discordapp.net/attachments/1063259243727306824/1155576306969362483/image.png) E49E43

      El color ámbar representa la juventud y la calidez que resaltan los cultivos a plena luz.
  - **Espaciado o Spacing:**
    - **Ilustraciones:**
      Proponemos cuadros de imágenes simples/minimalistas, con el propósito de enviar la información de manera directa como se planeaba.
    - **Fotografía:**
      La fotografía es una herramienta esencial en nuestro rubro, ya que nos permite apoyar la información escrita sobre cualquier tema de agricultura.
    - **Botones:**
      Se emplean botones con márgenes redondeados para demostrar adaptabilidad y usabilidad.



- 5.2. Information Architecture.
  
  En esta sección detallamos y sustentamos las decisiones de diseño que tomamos como equipo durante el desarrollo del proyecto. Siempre con el objetivo de facilitar al usuario adaptarse a nuestra aplicación, explicaremos las propuestas claves para el diseño de nuestro Landing Page y nuestra App.
  - 5.2.1. Organization Systems.
    - **Visual:** En este ámbito, aplicamos una estructura organizativa claramente jerárquica. Este enfoque se basa en la creación de aspectos visuales que facilitan la comprensión de la información para el usuario, pero de manera más simple. Dentro del contexto de nuestra página web, los elementos más prominentes se encuentran en el nivel superior de la jerarquía, abarcando aquellos elementos principales que atraerán la atención de nuestros usuarios, ya sean empleados o empleadores, al ingresar al sitio, como el logotipo, los encabezados, las tarjetas y los botones, entre otros. En el segundo nivel se encuentran los elementos que están directamente relacionados con los de nivel superior, como los subtítulos y las descripciones, así como los campos de entrada de información. Finalmente, en el tercer y último nivel se sitúan los elementos independientes o complementarios, como el icono de búsqueda, la foto de perfil, entre otros.
    - **Por contenido:** En esta parte, el usuario tiene la opción de organizar la información que se presenta de acuerdo a los criterios que le resulten más apropiados:

      - **Orden alfabético:** Los trabajos en los que el empleado       actualmente se encuentra se disponen en orden alfabético.

      - **Orden cronológico:** Las ofertas de trabajo se muestran en      función de su fecha más reciente.

      - **Prioridad personalizada:** Se presentan perfiles recomendados en      base a las necesidades específicas de especialistas que la      oferta publicada por el empleador pueda requerir.    
  - 5.2.2. Labeling Systems.
    - **Encabezados (headings):** Estas etiquetas resultan beneficiosas para los usuarios, ya que les permiten comprender de manera inmediata toda la información contenida en una sección, simplemente al leerlas.

    - **Etiquetas textuales:** Son etiquetas que se emplean habitualmente para señalar categorías específicas.

    - **Etiquetas icónicas (iconic labels):** Implican el uso de imágenes para que la etiqueta tenga un significado claro sin requerir texto adicional. No obstante, por lo general, se acompañan de etiquetas de texto para evitar confusiones por parte del usuario.

    Estos dos tipos de etiquetas se hacen visibles en la barra de navegación de nuestro prototipo.
  - 5.2.3. SEO Tags and Meta Tags.

    Las etiquetas meta desempeñan un papel crucial al señalar información codificada y definir los metadatos. No se muestran directamente en los sitios web, sino que son interpretadas por los navegadores o rastreadores web. Estas etiquetas meta simplifican el análisis de los archivos HTML y contribuyen a mantener el contenido del archivo de manera eficiente. Además, son valiosas para mejorar la posición de nuestra página web en los resultados de búsqueda.

    - **Titulo:** Esta etiqueta se cuenta entre las más importantes y suele ubicarse antes que cualquier otra etiqueta meta. Todos los motores de búsqueda la utilizan como encabezado en las páginas de resultados de búsqueda (SERP).
  
      ```<title> Mejora tu producción con AgriPure </title>```

    - **Codificación de caracteres:** Esta etiqueta ayudará a que muestre correctamente los caracteres especiales en la página. 
  
      ``` <meta charset="utf-8"/> ```
    - **Descripcion:** Esta meta etiqueta nos sirve para proporcionar un resumen del contenido de la página web. Aquí debemos dar una breve información de lo que se puede visualizar en la página.
      ```<meta name="description" content="Índice de vegetación. El índice de vegetación ayuda a que el agricultor pueda ver.... "/> ```
    - **Palabras Clave:** En esta etiqueta se pone las palabras claves relacionadas con el tema o contenido de la página web.

        ``` <meta name="keywords" content="cultivo, guía de cultivo, gestión de siembra"/>  ```

    - **Autor y Derechos de Autor:** Se utiliza para registrar la información del autor de la página web y la propiedad y derechos de autor.

       ``` <meta name="author" content="AgriPure" /><meta name="copyright" content="Copyright AgriPure team" /> ```

  - 5.2.4. Searching Systems.

    Hemos implementado los sistemas de búsqueda en el apartado de búsqueda de tipos de plantas.  Aquí el usuario escribirá y buscará dentro de una caja de texto la planta que desea sembrar. Entonces se deslizará una overlay hacia abajo mostrando las recomendaciones de tipo de planta que quizá esté buscando.
  - 5.2.5. Navigation Systems.
      - **Landing Page:** 
      El usuario podrá direccionarse a otra frame por medio de realizar un click en los linklabel, cada uno con una dirección relacionada al contenido del label, que se encontraran en los encabezados o headers. Usaremos un encabezado de nuestros diseños para una breve demostración. Al dar click en “Comienza ya” y “Registrate”, los llevará a las secciones con sus temáticas correspondientes. Asimismo, se implementarán botones para facilitar la navegación del usuario en caso se hayan quedado interesados con algún bloque de la página principal.

- 5.3. Landing Page UI Design.
  
    Para esta sección mostraremos el desarrollo visual de nuestro Landing Page. Para ello, utilizamos una herramienta de diseño web como Figma, debido a sus funciones y plugins que nos permite desarrollar el prototipo sin limitaciones. Asimismo, se evidenciará el uso de los Style Guidelines e Information Architecture.
  - 5.3.1. Landing Page Wireframe.

	Mobile:
	![texto](https://media.discordapp.net/attachments/912089666939916348/1155679042515779644/image.png?width=195&height=669)
	![texto](https://media.discordapp.net/attachments/912089666939916348/1155679133519593522/image.png?width=144&height=668)
	![texto](https://media.discordapp.net/attachments/912089666939916348/1155679191258366103/image.png?width=182&height=669)	
	Tablet:
		![texto](https://media.discordapp.net/attachments/1063259243727306824/1155582004579012730/image.png)
		Desktop:
		![texto](https://media.discordapp.net/attachments/1063259243727306824/1155582004579012730/image.png)
  - 5.3.2. Landing Page Mock-up.
- 5.4. Applications UX/UI Design.
  - 5.4.1. Applications Wireframes.
  - 5.4.2. Applications Wireflow Diagrams.
  - 5.4.3. Applications Mock-ups.
  - 5.4.4. Applications User Flow Diagrams
  
     Es un tipo de diagrama utilizado en el diseño de aplicaciones y sitios web para visualizar cómo los usuarios interactúan con la interfaz y las funcionalidades de una aplicación. Estos diagramas representaran el camino que un usuario típico sigue mientras utiliza la aplicación, desde el inicio hasta la finalización de una tarea o proceso.
  
  | User Goal | Como usuario deseo poder registrarme en la aplicación para poder acceder a sus beneficios.  |
  |-----------|-----------|
  | Task Flow | ![texto](https://media.discordapp.net/attachments/1063259243727306824/1155582004579012730/image.png) |
  | User Flow | ![texto](https://media.discordapp.net/attachments/1063259243727306824/1155582152994455696/image.png) |

  | User Goal | Como usuario deseo poder cerrar sesión en el dispositivo para que nadie más pueda usar mi cuenta  |
  |-----------|-----------|
  | Task Flow | ![texto](https://media.discordapp.net/attachments/1063259243727306824/1155582495438417970/image.png) |
  | User Flow | ![texto](https://media.discordapp.net/attachments/1063259243727306824/1155582576136835283/image.png) |

  | User Goal | Como usuario deseo poder actualizar mis datos guardados en la aplicación para que esta me funcione correctamente  |
  |-----------|-----------|
  | Task Flow | ![texto](https://media.discordapp.net/attachments/1063259243727306824/1155582742159970374/image.png) |
  | User Flow | ![texto](https://media.discordapp.net/attachments/1063259243727306824/1155582756655472680/image.png) |  

  | User Goal | Como usuario deseo poder ingresar la planta que deseo sembrar para que la aplicación me ayude en su control |
  |-----------|-----------|
  | Task Flow | ![texto](https://media.discordapp.net/attachments/1063259243727306824/1155582877942173797/image.png) |
  | User Flow | ![texto](https://media.discordapp.net/attachments/1063259243727306824/1155582897697333298/image.png) |  

  | User Goal | Como usuario deseo saber cuáles son los días que debo fumigar mis plantas para que no se infecten de plagas, al igual de saber en qué fechas debo fertilizar mis plantas para que crezcan y produzcan más frutos. |
  |-----------|-----------|
  | Task Flow | ![texto](https://media.discordapp.net/attachments/1063259243727306824/1155583170809430087/image.png) |
  | User Flow | ![texto](https://media.discordapp.net/attachments/1063259243727306824/1155583194188480554/image.png) |    



- 5.5. Applications Prototyping.
  
<!--stackedit_data:
eyJoaXN0b3J5IjpbNzU1NzQ5ODg1XX0=
-->