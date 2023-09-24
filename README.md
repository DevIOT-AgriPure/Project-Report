

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
