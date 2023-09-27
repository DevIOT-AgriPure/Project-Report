- [Capítulo VI: Product implementation, Validation \& Deployment](#capítulo-vi-product-implementation-validation--deployment)
  - [6.1 Software Configuration Management](#61-software-configuration-management)
    - [6.1.1 Software Development EnviromentConfiguration](#611-software-development-enviromentconfiguration)
    - [6.1.2. Source Code Management](#612-source-code-management)
    - [6.1.3. Source Code Style Guide \& Conventions](#613-source-code-style-guide--conventions)
    - [6.1.4. Software Deployment Configuration](#614-software-deployment-configuration)
  - [6.2 Landing Page, Services \& Applications Implementation.](#62-landing-page-services--applications-implementation)
    - [6.2.1. Sprint 1](#621-sprint-1)
      - [6.2.1.1 Sprint Planning 1](#6211-sprint-planning-1)
      - [6.2.1.2 Sprint Backlog 1](#6212-sprint-backlog-1)
      - [6.2.1.3. Development Evidence for Sprint Review](#6213-development-evidence-for-sprint-review)
      - [6.2.1.4. Testing Suite Evidence for Sprint Review](#6214-testing-suite-evidence-for-sprint-review)
      - [6.2.1.5. Execution Evidence for Sprint Review](#6215-execution-evidence-for-sprint-review)
      - [6.2.1.6. Services Documentation Evidence for Sprint Review](#6216-services-documentation-evidence-for-sprint-review)
      - [6.2.1.7. Software Deployment Evidence for Sprint Review](#6217-software-deployment-evidence-for-sprint-review)
      - [6.2.1.8. Team Collaboration Insights During Sprint](#6218-team-collaboration-insights-during-sprint)


# Capítulo VI: Product implementation, Validation & Deployment
## 6.1 Software Configuration Management

Para el desarrollo de proyecto se utilizarán diferentes herramientas de trabajo y colaboración que nos permitirá llevarlo a cabo de mejor manera.
    
### 6.1.1 Software Development EnviromentConfiguration
  En esta sección vamos a definir las líneas base del sistema de la gestión de la configuración. A continuación, se definirán las aplicaciones que serán utilizadas para el desarrollo de nuestro proyecto.

  - **LucidChart:** Aplicación web que se utilizará para creación de diagramas de clases. Podemos accedertravés del siguiente enlace: [https://www.lucidchacom/](https://www.lucidchart.com/
  - **Structurizr:** Aplicación web que se utilizará pala creación del diagrama c4. Podemos acceder a travdel siguiente enlace: [https://structurizr.co(https://structurizr.com
  - **UXPressia:** Aplicación web que se utilizará pala creación de artefactos Lean UX como User PersonUser Journey Maps, Empathy Maps, Impact Maps. Podemacceder a través de: [https://uxpressia.com/](httpsuxpressia.com
  - **Trello:** Aplicación web que se utilizará para seguimiento de las historias de usuario en cada sprinPodemos acceder a través de: [https://trello.co(https://trello.com
  - **Figma:** Aplicación web que se utilizará para creación de Wireframes y Mockups. También servirá pala creación de prototipos de nuestra aplicación wresponsive. Podemos acceder a través de: [https://figcom/](https://figma.com
  - **Visual Studio Code:** Entorno de desarrollo (IDLque utilizaremos para trabajar en nuestro front-end nuestra aplicación web. Podemos descargarlo a travde: [https://code.visualstudio.com/](https://covisualstudio.com
  - **Intellij Idea Ultima:** Entorno de desarrol(IDLE) que utilizaremos para trabajar en nuestback-end de nuestra aplicación web. Podemos descargara través de: [https://www.jetbrains.com/idea/downloasection=windows](https://www.jetbrains.com/iddownload/?section=window
  - **VueJs:** Framework de javascript que utilizarempara desarrollar nuestro front-end de nuestaplicación web. Requiere instalar previamente NodeJPodemos descargar NodeJs a través de: [https://nodeorg/es/](https://nodejs.org/es/). Luego, podreminstalar VueJs siguiendo las instrucciones instalación dadas en el siguiente enlace: [https://vuejs.org/v2/guide/installation.html](https://es.vueorg/v2/guide/installation.htm
  - **GitHub:** Aplicación web que utilizaremos para control de versiones de nuestro proyecto. Podemacceder a sus servicios a través de: [https://githcom/](https://github.com
  - **Android Studio:** Entorno de desarrollo (IDLE) qutilizaremos para desarrollar nuestra aplicación móviPodemos acceder a través de: [https://developer.androcom/studgclid=CjwKCAjwmbqoBhAgEiwACIjzEALGhH7IKxVPgvmi7rUWtPaD-Bw3QZAltOFF2JEIJvrA-ftw-hRoCfvsQAvD_BwE&gclsrc=aw.(https://developer.android.com/studgclid=CjwKCAjwmbqoBhAgEiwACIjzEALGhH7IKxVPgvmi7rUWtPaD-Bw3QZAltOFF2JEIJvrA-ftw-hRoCfvsQAvD_BwE&gclsrc=aw.ds)

### 6.1.2. Source Code Management

  Como se mencionó anteriormente, se utilizará GitHcomo sistema de control de versiones. Se han crearepositorios dentro de nuestra organización de GitHu
  - Enlace al repositorio de la landing page: [httpsgithub.com/DevIOT-AgriPure/AgriPure-Landing-Pa(https://github.com/DevIOT-AgriPuAgriPure-Landing-Pag
  - Enlace al repositorio de Front-End: [https://githcom/DevIOT-AgriPure/Agripure-Web-Application](httpsgithub.com/DevIOT-AgriPure/Agripure-Web-Applicatio
  - Enlace al repositorio de Back-End: [https://githcom/DevIOT-AgriPure/AgriPure-WebServices](httpsgithub.com/DevIOT-AgriPure/AgriPure-WebService
  Los repositorios mencionados anteriormente seguirán metodología de Git Flow, que nos permitirá trabajar manera eficiente y ágil en proyectos colaborativos. este enfoque, utilizaremos las siguientes ramas:
  
  - **Main:** Esta rama contiene la versión completa dproyecto, asegurándose de que no haya errores en ejecución. Es la versión que se encuentra en producciy es accesible para los usuarios finale
  - **Hotfix:** En caso de que surja un problema con versión en la rama Main, utilizaremos esta rama corespaldo para identificar y resolver el problema lo mrápido posible. Una vez resuelto, fusionaremos lcambios con las ramas Main y Develop, y lueeliminaremos esta ram
  - **Release:** En esta rama, la aplicación web funciosin problemas, pero debe someterse a pruebexhaustivas para garantizar que todas lfuncionalidades estén operativas. Cuando las pruebsean exitosas y no se encuentren errores, esta versise fusiona con la rama Main. La rama Release se creapartir de la rama Develo
  - **Develop:** En esta rama se encuentran ldiferentes características (features) que se hfusionado y desarrollado durante el sprint actua
  - **Feature:** Estas ramas se crean según sea necesarpara agregar nuevas funcionalidades a la aplicaciweb. Se derivan de la rama Develop y se fusionanactualizan lo más rápido posible para evitar problemde conflict
  Flujo de trabajo basándose en la metodología GitFl
  [https://nvie.com/img/git-model@2x.png](https://nvcom/img/git-model@2x.png)

### 6.1.3. Source Code Style Guide & Conventions

  Para el desarrollo del código adoptamos convencionesestilos presentes en diversas tecnologías a nivmundia
  - Front-End: Vue y Vuetify
  - Back-End: Java y Spring Boot
  - Landing-Page: HTML, CSS y Javascript
  - Base de datos: MySQL
  - Convenciones de idioma: Se empleará el idioma inglpara desarrollar el código, sea en nuestra landipage, front end services o back end services. Tambilos títulos de los commits se encontrarán en el misidioma.
  - Convenciones de tecnología: Cada nombre de una taben nuestra base de datos iniciará con mayúscula, y esta se compone de dos o más palabras, se separará cauna con un "_" y seguirá una mayúscula.
  - Cada Unit Test deberá ser escrito en lenguaje Gherky sus convenciones. Podremos revisarlos en el siguienenlace: [https://specflow.org/gherkgherkin-conventions-for-readable-specification(https://specflow.org/gherkgherkin-conventions-for-readable-specifications/)
  - Para escribir el título de los commits, utilizaremoConventional Commits. Podemos revisar la documentacien el siguiente enlace: [https://wconventionalcommits.org/en/v1.0.0/](https://wconventionalcommits.org/en/v1.0.0/)
  - Para trabajar con JavaScript, se utilizarán lconvenciones "Google Javascript Style Guide". Podemacceder a estas a través del siguiente enlace: [httpsgoogle.github.io/styleguide/jsguide.html](httpsgoogle.github.io/styleguide/jsguide.html)
  - Para trabajar con Java y Spring Boot, se utilizarlas convenciones que el fabricante brinda y por comunidad de desarrollo. Podremos observar estconvenciones en el siguiente enlace: [https://googgithub.io/styleguide/javaguide.html](https://googgithub.io/styleguide/javaguide.html)
### 6.1.4. Software Deployment Configuration
  En esta sección observaremos como desplegamos cada ude nuestros servicios en la nub
  **Landing Page:
  Para el despliegue de nuestra landing page se utiliza"GitHub Pages" ya que es ideal para sitios westáticos. Es muy fácil de realizar el despliegue. Pallevarlo a cabo, seguiremos los siguientes paso
  - **Accedemos al repositorio de nuestra landing page:![Landing page deploy](https://github.cDevIOT-AgriPure/Project-Report/blob/feature/capituloimages/software-deploy-configuration/landingdeploy.Praw=tru
  - **Nos vamos a configuración, a la sección de page*[Landing page deploy conf](https://github.cDevIOT-AgriPure/Project-Report/blob/feature/capituloimages/software-deploy-configuration/landingdeploycoPNG?raw=tru
  - **Seleccionamos la rama de donde desplegaremos landing** ![Landing page delpoy branch](https://githcom/DevIOT-AgriPure/Project-Report/blob/featucapitulo-6/images/software-deploy-configuratiladingdeploybranch.PNG?raw=tru
  - **Esperamos unos instantes y la landing page estadesplegada** 

![Landing Deployed](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-6/images/software-deploy-configuration/LandingDeployed.PNG?raw=true)

   **Web application**

Para el despliegue de nuestro front-end service se utilizarà "Netlify", ya que es ideal para sitios web dinàmicos.

 **Web Services**

 Para el despliegue de nuestro back-end service se utilizarà "Railway", es ideal para subir soluciones y crear esquemas

## 6.2 Landing Page, Services & Applications Implementation.
### 6.2.1. Sprint 1
    
  Para este sprint tomamos en cuenta las User Stories que tengan relaciòn con el desarrollo e implementaciòn de la landing page y la primera versión de nuestro front-end. Se encargò una tarea a cada integrante del equipo.

#### 6.2.1.1 Sprint Planning 1

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

#### 6.2.1.2 Sprint Backlog 1
        
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
        
#### 6.2.1.3. Development Evidence for Sprint Review

  | Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited Date |
  |------------|--------|-----------|----------------|---------------------|---------------|
  |https://github.com/DevIOT-AgriPure/AgriPure-Landing-Page.git  | main |     8fce68724ed2a3777e3f471a4493aa5085a1ee5d|Create README.md|                     |24/08/2023|
  |https://github.com/DevIOT-AgriPure/AgriPure-Landing-Page.git  | main |     8fce68724ed2a3777e3f471a4493aa5085a1ee5d|Create README.md|                     |24/08/2023|
####  6.2.1.4. Testing Suite Evidence for Sprint Review

  | Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited Date |
  |------------|--------|-----------|----------------|---------------------|---------------|
  |            |        |           |                |                     |               |
    
####  6.2.1.5. Execution Evidence for Sprint Review

  Para la entrega del presente sprint se logró desarrollar lo acordado, implementación y despliegue. 
  Enlace a la Landing Page: [https://deviot-agripure.github.io/AgriPure-Landing-Page/](https://deviot-agripure.github.io/AgriPure-Landing-Page/)
        ![Landing Deployed](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-6/images/software-deploy-configuration/LandingDeployed.PNG?raw=true)


#### 6.2.1.6. Services Documentation Evidence for Sprint Review
  Para esta entrega no se han implementado los servicios Back-end, por lo que en posteriores sprints completaremos esta sección.


#### 6.2.1.7. Software Deployment Evidence for Sprint Review

Como se demostro anteriormente, la Landing Page se ha desplegado usando GitHub Pages, debido a la simplicidad de hacer deploys con paginas estaticas.

#### 6.2.1.8. Team Collaboration Insights During Sprint

    
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE5MDM5ODExNl19
-->