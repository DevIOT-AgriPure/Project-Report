

## Capítulo VI: Product implementation, Validation & Deployment
- **6.1 Software Configuration Management**

    Para el desarrollo de proyecto se utilizarán diferentes herramientas de trabajo y colaboración que nos permitirá llevarlo a cabo de mejor manera.
    
    - **6.1.1 Software Development EnviromentConfiguration**
        En esta sección vamos a definir las líneas base del sistema de la gestión de la configuración. A continuación, se definirán las aplicaciones que serán utilizadas para el desarrollo de nuestro proyecto.

        - **LucidChart:** Aplicación web que se utilizará para la creación de diagramas de clases. Podemos acceder a través del siguiente enlace: [https://www.lucidchart.com/](https://www.lucidchart.com/) 

        - **Structurizr:** Aplicación web que se utilizará para la creación del diagrama c4. Podemos acceder a través del siguiente enlace: [https://structurizr.com/](https://structurizr.com/)

        - **UXPressia:** Aplicación web que se utilizará para la creación de artefactos Lean UX como User Personas,User Journey Maps, Empathy Maps, Impact Maps. Podemos acceder a través de: [https://uxpressia.com/](https://uxpressia.com/)

        - **Trello:** Aplicación web que se utilizará para el seguimiento de las historias de usuario en cada sprint. Podemos acceder a través de: [https://trello.com/](https://trello.com/)

        - **Figma:** Aplicación web que se utilizará para la creación de Wireframes y Mockups. También servirá para la creación de prototipos de nuestra aplicación web responsive. Podemos acceder a través de: [https://figma.com/](https://figma.com/)

        - **Visual Studio Code:** Entorno de desarrollo (IDLE) que utilizaremos para trabajar en nuestro front-end de nuestra aplicación web. Podemos descargarlo a través de: [https://code.visualstudio.com/](https://code.visualstudio.com/)

        - **Intellij Idea Ultima:** Entorno de desarrollo (IDLE) que utilizaremos para trabajar en nuestro back-end de nuestra aplicación web. Podemos descargarlo a través de: [https://www.jetbrains.com/idea/download/?section=windows](https://www.jetbrains.com/idea/download/?section=windows)

        - **VueJs:** Framework de javascript que utilizaremos para desarrollar nuestro front-end de nuestra aplicación web. Requiere instalar previamente NodeJs. Podemos descargar NodeJs a través de: [https://nodejs.org/es/](https://nodejs.org/es/). Luego, podremos instalar VueJs siguiendo las instrucciones de instalación dadas en el siguiente enlace: [https://es.vuejs.org/v2/guide/installation.html](https://es.vuejs.org/v2/guide/installation.html)

        - **GitHub:** Aplicación web que utilizaremos para el control de versiones de nuestro proyecto. Podemos acceder a sus servicios a través de: [https://github.com/](https://github.com/)

        - **Android Studio:** Entorno de desarrollo (IDLE) que utilizaremos para desarrollar nuestra aplicación móvil. Podemos acceder a través de: [https://developer.android.com/studio?gclid=CjwKCAjwmbqoBhAgEiwACIjzEALGhH7IKxVPgvmi7rUWtPaFlpD-Bw3QZAltOFF2JEIJvrA-ftw-hRoCfvsQAvD_BwE&gclsrc=aw.ds](https://developer.android.com/studio?gclid=CjwKCAjwmbqoBhAgEiwACIjzEALGhH7IKxVPgvmi7rUWtPaFlpD-Bw3QZAltOFF2JEIJvrA-ftw-hRoCfvsQAvD_BwE&gclsrc=aw.ds)

    - **6.1.2. Source Code Management**

        Como se mencionó anteriormente, se utilizará GitHub como sistema de control de versiones. Se han creado repositorios dentro de nuestra organización de GitHub.

        - Enlace al repositorio de la landing page: [https://github.com/DevIOT-AgriPure/AgriPure-Landing-Page](https://github.com/DevIOT-AgriPure/AgriPure-Landing-Page)

        - Enlace al repositorio de Front-End: [https://github.com/DevIOT-AgriPure/Agripure-Web-Application](https://github.com/DevIOT-AgriPure/Agripure-Web-Application)

        - Enlace al repositorio de Back-End: [https://github.com/DevIOT-AgriPure/AgriPure-WebServices](https://github.com/DevIOT-AgriPure/AgriPure-WebServices)

        Los repositorios mencionados anteriormente seguirán la metodología de Git Flow, que nos permitirá trabajar de manera eficiente y ágil en proyectos colaborativos. En este enfoque, utilizaremos las siguientes ramas:
        
        - **Main:** Esta rama contiene la versión completa del proyecto, asegurándose de que no haya errores en su ejecución. Es la versión que se encuentra en producción y es accesible para los usuarios finales.

        - **Hotfix:** En caso de que surja un problema con la versión en la rama Main, utilizaremos esta rama como respaldo para identificar y resolver el problema lo más rápido posible. Una vez resuelto, fusionaremos los cambios con las ramas Main y Develop, y luego eliminaremos esta rama.

        - **Release:** En esta rama, la aplicación web funciona sin problemas, pero debe someterse a pruebas exhaustivas para garantizar que todas las funcionalidades estén operativas. Cuando las pruebas sean exitosas y no se encuentren errores, esta versión se fusiona con la rama Main. La rama Release se crea a partir de la rama Develop.

        - **Develop:** En esta rama se encuentran las diferentes características (features) que se han fusionado y desarrollado durante el sprint actual.

        - **Feature:** Estas ramas se crean según sea necesario para agregar nuevas funcionalidades a la aplicación web. Se derivan de la rama Develop y se fusionan y actualizan lo más rápido posible para evitar problemas de conflicto.

        Flujo de trabajo basándose en la metodología GitFlow

        [https://nvie.com/img/git-model@2x.png](https://nvie.com/img/git-model@2x.png)

    - **6.1.3. Source Code Style Guide & Conventions**

        Para el desarrollo del código adoptamos convenciones y estilos presentes en diversas tecnologías a nivel mundial.

        - Front-End: Vue y Vuetify
        - Back-End: Java y Spring Boot
        - Landing-Page: HTML, CSS y Javascript
        - Base de datos: MySQL
        - Convenciones de idioma: Se empleará el idioma inglés para desarrollar el código, sea en nuestra landing page, front end services o back end services. También los títulos de los commits se encontrarán en el mismo idioma.
        - Convenciones de tecnología: Cada nombre de una tabla en nuestra base de datos iniciará con mayúscula, y si esta se compone de dos o más palabras, se separará cada una con un "_" y seguirá una mayúscula.
        - Cada Unit Test deberá ser escrito en lenguaje Gherkin y sus convenciones. Podremos revisarlos en el siguiente enlace: [https://specflow.org/gherkin/gherkin-conventions-for-readable-specifications/](https://specflow.org/gherkin/gherkin-conventions-for-readable-specifications/)
        - Para escribir el título de los commits, utilizaremos  Conventional Commits. Podemos revisar la documentación en el siguiente enlace: [https://www.conventionalcommits.org/en/v1.0.0/](https://www.conventionalcommits.org/en/v1.0.0/)
        - Para trabajar con JavaScript, se utilizarán las convenciones "Google Javascript Style Guide". Podemos acceder a estas a través del siguiente enlace: [https://google.github.io/styleguide/jsguide.html](https://google.github.io/styleguide/jsguide.html)
        - Para trabajar con Java y Spring Boot, se utilizarán las convenciones que el fabricante brinda y por su comunidad de desarrollo. Podremos observar estas convenciones en el siguiente enlace: [https://google.github.io/styleguide/javaguide.html](https://google.github.io/styleguide/javaguide.html)
    - **6.1.4. Software Deployment Configuration**
        En esta sección observaremos como desplegamos cada uno de nuestros servicios en la nube.

        **Landing Page:**

        Para el despliegue de nuestra landing page se utilizará "GitHub Pages" ya que es ideal para sitios web estáticos. Es muy fácil de realizar el despliegue. Para llevarlo a cabo, seguiremos los siguientes pasos:


        - **Accedemos al repositorio de nuestra landing page:** ![Landing page deploy](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-6/images/software-deploy-configuration/landingdeploy.PNG?raw=true)

        - **Nos vamos a configuración, a la sección de page** ![Landing page deploy conf](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-6/images/software-deploy-configuration/landingdeployconf.PNG?raw=true)

        - **Seleccionamos la rama de donde desplegaremos la landing** ![Landing page delpoy branch](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-6/images/software-deploy-configuration/ladingdeploybranch.PNG?raw=true)

        - **Esperamos unos instantes y la landing page estará desplegada** ![Landing page deployed]()

        **Web application**

        Para el despliegue de nuestro front-end service se utilizarà "Netlify", ya que es ideal para sitios web dinàmicos.

        **Web Services**

        Para el despliegue de nuestro back-end service se utilizarà "Railway", es ideal para subir soluciones y crear esquemas

- **6.2 Landing Page, Services & Applications Implementation.**

    - **6.2.1. Sprint 1**
    
    Para este sprint tomamos en cuenta las User Stories que tengan relaciòn con el desarrollo e implementaciòn de la landing page y la primera versión de nuestro front-end. Se encargò una tarea a cada integrante del equipo.

    - **6.2.1.1 Sprint Planning 1**

        - Sprint #: 1
        - Spring Planning Background
            | Date                            | 24/09/2023                                                   |
            |---------------------------------|--------------------------------------------------------------|
            | Time                            | 5pm                                                          |
            | Location                        | Llamada en discord                                           |
            | Prepared By                     | Talledo, Diego                                               |
            | Attendees (to planning meeting) | Soto, Franchesco Reynoso, Andrés Palomino, Bruno Alva, Frank |
        - Sprint Goal & User Stories
            | Sprint Goal 1                   | Implementar y desplegar la landing page. A su vez, desarrollar la primera    versión del front-end |
            |---------------------------------| ------------------------------------------------------------------------------------------------|
            | Sprint 1  Velocity               |                                                                                                    |
            | Sum of story  points             |                                                                                                    |

    - **6.2.1.2 Sprint Backlog 1**
        
        - Sprint #: 1
            | US Id | US Title | Task Id | Task Description | Task Estimation | Assigned To | Status |
            |-------|----------|---------|------------------|-----------------|-------------|--------|
            |US011  |Botón Call to action|    ST001     |      Diseño e implementación del Botón Call to action            |    4 horas     | Andrés Reynoso            |   Done  |
            |US012|Visualización de redes sociales|ST002| Diseño e implementación se la sección de redes sociales en la landing page| 8 horas | Diego Talledo|Done|
            |US013|Visualizar características de la aplicación|ST003|Diseño e implementación de la sección de características en la landing page| 8 horas| Franchesco Soto|Done|
            |US004|Selección de planta a sembrar|ST004|Diseño e implementación visual de la selección de planta a sembrar en front-end| 8 horas|Diego Talledo|In process|
            |US005|Guía de elección de tierra de sembrado|ST005|Diseño e implementación visual de la sección de guía de elección de tierra|8 horas|Franchesco Soto|In process|
            |US006|Distancia de siembra entre las plantas|ST006|Diseño e implementación visual de la sección de distancia de siembra|8 horas|Bruno Palomino|In process|
            |US007|Distancia de profundidad de siembra| ST007|Diseño e implementación visual de la sección de profundidad de siembra| 8 horas | Frank| In process|
            |US010|Contacto a especialista|ST008|Diseño e implementación visual de la sección de contacto a especialista| 8 horas| Bruno| In process|
        
    - **6.2.1.3. Development Evidence for Sprint Review**

        | Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited Date |
        |------------|--------|-----------|----------------|---------------------|---------------|
        |            |        |           |                |                     |               |
    - **6.2.1.4. Testing Suite Evidence for Sprint Review**

        | Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited Date |
        |------------|--------|-----------|----------------|---------------------|---------------|
        |            |        |           |                |                     |               |
    
    - **6.2.1.5. Execution Evidence for Sprint Review**

        Para la entrega del presente sprint se logró desarrollar lo acordado, implementación y despliegue. 
        Enlace a la Landing Page: ![urlLanding](https://deviot-agripure.github.io/AgriPure-Landing-Page/)
        

    - **6.2.1.6. Services Documentation Evidence for Sprint Review**


    - **6.2.1.7. Software Deployment Evidence for Sprint Review**


    - **6.2.1.8. Team Collaboration Insights During Sprint**

    