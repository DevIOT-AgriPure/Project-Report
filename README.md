- [Capítulo IV: Solution Software Design](#capítulo-iv-solution-software-design)
  - [4.1. Strategic-Level Domain-Driven Design.](#41-strategic-level-domain-driven-design)
    - [4.1.1. EventStorming.](#411-eventstorming)
      - [4.1.1.1 Candidate Context Discovery.](#4111-candidate-context-discovery)
      - [4.1.1.2 Domain Message Flows Modeling.](#4112-domain-message-flows-modeling)
      - [4.1.1.3 Bounded Context Canvases.](#4113-bounded-context-canvases)
    - [4.1.2. Context Mapping.](#412-context-mapping)
    - [4.1.3. Software Architecture.](#413-software-architecture)
      - [4.1.3.1. Software Architecture System Landscape Diagram. ](#4131-software-architecture-system-landscape-diagram-)
      - [4.1.3.2. Software Architecture Context Level Diagrams. ](#4132-software-architecture-context-level-diagrams-)
      - [4.1.3.2. Software Architecture Container Level Diagrams. ](#4132-software-architecture-container-level-diagrams-)
      - [4.1.3.3. Software Architecture Deployment Diagrams. ](#4133-software-architecture-deployment-diagrams-)
  - [4.2. Tactical-Level Domain-Driven Design.](#42-tactical-level-domain-driven-design)
    - [4.2.1. Bounded Context: User Acount Manager](#421-bounded-context-user-acount-manager)
      - [4.2.1.1. Domain Layer.](#4211-domain-layer)
      - [4.2.1.2 Interface layer](#4212-interface-layer)
      - [4.2.1.3 Application Layer](#4213-application-layer)
      - [4.2.1.4 Infrastructure Layer](#4214-infrastructure-layer)
      - [4.2.1.5. Bounded Context Software Architecture Component Level Diagrams](#4215-bounded-context-software-architecture-component-level-diagrams)
      - [4.2.1.6 Bounded Context Software Architecture Code Level Diagrams](#4216-bounded-context-software-architecture-code-level-diagrams)
        - [4.2.1.6.1 Bounded Context Domain Layer Class Diagrams](#42161-bounded-context-domain-layer-class-diagrams)
        - [4.2.1.6.2 Bounded Context Database Diagrams](#42162-bounded-context-database-diagrams)
    - [4.2.2. Bounded Context: Plant Management](#422-bounded-context-plant-management)
      - [4.2.2.1. Domain Layer.](#4221-domain-layer)
      - [4.2.2.2 Interface layer](#4222-interface-layer)
      - [4.2.2.3 Application Layer](#4223-application-layer)
      - [4.2.2.4 Infrastructure Layer](#4224-infrastructure-layer)
      - [4.2.2.5. Bounded Context Software Architecture Component Level Diagrams](#4225-bounded-context-software-architecture-component-level-diagrams)
      - [4.2.2.6 Bounded Context Software Architecture Code Level Diagrams](#4226-bounded-context-software-architecture-code-level-diagrams)
        - [4.2.2.6.1 Bounded Context Domain Layer Class Diagrams](#42261-bounded-context-domain-layer-class-diagrams)
        - [4.2.2.6.2 Bounded Context Database Diagrams](#42262-bounded-context-database-diagrams)
    - [4.2.3. Bounded Context: Suscription Management](#423-bounded-context-suscription-management)
      - [4.2.3.1. Plan.](#4231-plan)
      - [4.2.3.2 Interface layer](#4232-interface-layer)
      - [4.2.3.3 Application Layer](#4233-application-layer)
      - [4.2.3.4 Infrastructure Layer](#4234-infrastructure-layer)
      - [4.2.3.5. Bounded Context Software Architecture Component Level Diagrams](#4235-bounded-context-software-architecture-component-level-diagrams)
      - [4.2.3.6 Bounded Context Software Architecture Code Level Diagrams](#4236-bounded-context-software-architecture-code-level-diagrams)
        - [4.2.3.6.1 Bounded Context Domain Layer Class Diagrams](#42361-bounded-context-domain-layer-class-diagrams)
        - [4.2.1.6.2 Bounded Context Database Diagrams](#42162-bounded-context-database-diagrams-1)
    - [4.2.4. Bounded Context: Crop Management](#424-bounded-context-crop-management)
      - [4.2.4.1. Crop.](#4241-crop)
      - [4.2.4.2 Interface layer](#4242-interface-layer)
      - [4.2.4.3 Application Layer](#4243-application-layer)
      - [4.2.4.4 Infrastructure Layer](#4244-infrastructure-layer)
      - [4.2.4.5. Bounded Context Software Architecture Component Level Diagrams](#4245-bounded-context-software-architecture-component-level-diagrams)
      - [4.2.4.6 Bounded Context Software Architecture Code Level Diagrams](#4246-bounded-context-software-architecture-code-level-diagrams)
        - [4.2.4.6.1 Bounded Context Domain Layer Class Diagrams](#42461-bounded-context-domain-layer-class-diagrams)
        - [4.2.4.6.2 Bounded Context Database Diagrams](#42462-bounded-context-database-diagrams)
    - [4.2.5. Bounded Context: Project Management](#425-bounded-context-project-management)
      - [4.2.5.1. Domain Layer.](#4251-domain-layer)
      - [4.2.5.2 Interface layer](#4252-interface-layer)
      - [4.2.5.3 Application Layer](#4253-application-layer)
      - [4.2.5.4 Infrastructure Layer](#4254-infrastructure-layer)
      - [4.2.5.5. Bounded Context Software Architecture Component Level Diagrams](#4255-bounded-context-software-architecture-component-level-diagrams)
      - [4.2.5.6 Bounded Context Software Architecture Code Level Diagrams](#4256-bounded-context-software-architecture-code-level-diagrams)
        - [4.2.5.6.1 Bounded Context Domain Layer Class Diagrams](#42561-bounded-context-domain-layer-class-diagrams)
        - [4.2.5.6.2 Bounded Context Database Diagrams](#42562-bounded-context-database-diagrams)
      - [4.2.6. Bounded Context: Notification](#426-bounded-context-notification)
      - [4.2.6.1. Domain Layer.](#4261-domain-layer)
      - [4.2.6.2 Interface layer](#4262-interface-layer)
      - [4.2.6.3 Application Layer](#4263-application-layer)
      - [4.2.6.4 Infrastructure Layer](#4264-infrastructure-layer)
      - [4.2.6.5. Bounded Context Software Architecture Component Level Diagrams](#4265-bounded-context-software-architecture-component-level-diagrams)
      - [4.2.6.6 Bounded Context Software Architecture Code Level Diagrams](#4266-bounded-context-software-architecture-code-level-diagrams)
        - [4.2.6.6.1 Bounded Context Domain Layer Class Diagrams](#42661-bounded-context-domain-layer-class-diagrams)
        - [4.2.6.6.2 Bounded Context Database Diagrams](#42662-bounded-context-database-diagrams)

# Capítulo IV: Solution Software Design 
## 4.1. Strategic-Level Domain-Driven Design. 
### 4.1.1. EventStorming. 
- **Unstructured exploration:** El siguiente gráfico representa la lluvia de eventos que el equipo realizó.
	![Unstructured exploration](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/event-storming/unstructured.PNG?raw=true)
- **Timelines:** Este gráfico de timelines representa la secuencia temporal de eventos y acciones clave relacionados con la gestión de cultivos, monitoreo, búsqueda de especialista en nuestra aplicación. Cada línea de tiempo corresponde a un aspecto específico de la gestión de cultivos y muestra cómo se desarrollan los eventos con el tiempo. Este diagrama nos ayuda a comprender la lógica temporal de la aplicación y cómo los eventos se relacionan entre sí para proporcionar una visión general de la gestión de cultivos.	
	![Timelines](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/event-storming/timeline.PNG?raw=true)
- **Pivotal Points:** Este gráfico representa los Pivotal Points en el flujo de eventos de nuestro sistema de gestión de cultivos. Los Pivotal Points son momentos críticos en los cuales se producen cambios significativos o se toman decisiones clave que afectan la lógica y el comportamiento del sistema. Identificar y comprender estos puntos pivote es esencial para garantizar que nuestro software capture adecuadamente la complejidad y los requisitos críticos del negocio.	
	![Pivotal Points](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/event-storming/pivotal.PNG?raw=true)
- **Comands:** Este gráfico representa los comandos que los usuarios pueden emitir para interactuar con nuestro sistema de gestión de cultivos. Los comandos son acciones que los usuarios toman para lograr sus objetivos y modificar el estado del sistema. Identificar estos comandos es esencial para comprender cómo los usuarios interactúan con nuestra aplicación y qué acciones pueden realizar para gestionar sus cultivos de manera efectiva.	
	![Comands](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/event-storming/commands.PNG?raw=true)
- **Policies:** Este gráfico representa las políticas que dictan cómo el sistema de gestión de cultivos responde a eventos y acciones específicas. Las políticas son reglas o directrices que guían el comportamiento del sistema en situaciones diversas. Identificar y comprender estas políticas es esencial para asegurar que nuestro software funcione de acuerdo con las reglas de negocio y las expectativas de los usuarios.	
	![Policies](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/event-storming/policies.PNG?raw=true)
- **Read Models:** Este gráfico representa los modelos de lectura que permitirán a los usuarios acceder eficientemente a los datos relacionados con la gestión de cultivos en nuestro sistema. Los modelos de lectura son representaciones optimizadas de los datos que se utilizan para generar informes, consultas y visualizaciones. Identificar y definir estos modelos es esencial para garantizar que los usuarios puedan obtener la información que necesitan de manera rápida y precisa.
	![Read Models](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/event-storming/readmodels.PNG?raw=true)
- **External Systems:** Este gráfico representa la interacción planificada de nuestra aplicación con sistemas externos que son parte integral de nuestro ecosistema de gestión de cultivos. Los sistemas externos son componentes que se comunican con nuestra aplicación para intercambiar información y realizar acciones específicas. Identificar y comprender estas interacciones es crucial para garantizar que nuestro sistema sea capaz de integrarse efectivamente con otros sistemas y cumplir con los requisitos de negocio.
	![External Systems](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/event-storming/externalsystems.PNG?raw=true)
- **Agregates:** Este gráfico representa los agregados y las entidades clave que desempeñan un papel fundamental en la gestión de cultivos de nuestro sistema. Los agregados son grupos lógicos de entidades y datos que tienen un significado coherente en el contexto del negocio. Identificar y definir estos agregados es esencial para diseñar una estructura de datos efectiva y garantizar que nuestra aplicación refleje adecuadamente la realidad del dominio agrícola.
	![Agregates](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/event-storming/agregates.PNG?raw=true)	
#### 4.1.1.1 Candidate Context Discovery.

Identificar candidatos de contexto implica descubrir áreas potenciales deenfoque en un sistema complejo. Esto implica analizar el sistema paraidentificar sus componentes esenciales y sus interacciones, agrupándolos enáreas lógicas para simplificar el proceso de diseño e implementación. Elobjetivo principal es mejorar la escalabilidad, el rendimiento y la facilidadde mantenimiento del sistema.
![Candidates context](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/event-storming/boundedcontexts.jpg?raw=true)
		
#### 4.1.1.2 Domain Message Flows Modeling. 
#### 4.1.1.3 Bounded Context Canvases. 
- El Bounded Context es un patrón de diseño en la arquitectura de software que divide un sistema en áreas de dominio separadas con lenguajes y límites claros. Esto facilita la administración y escalabilidad de sistemas complejos, ya que cada contexto acotado puede desarrollarse y mantenerse de manera independiente. Los Bounded Context Canvases, por otro lado, son herramientas visuales para el diseño de arquitecturas de software basadas en Bounded Contexts. Su objetivo es fomentar la colaboración entre equipos y garantizar la coherencia y la relación adecuada entre los diferentes contextos delimitados en el sistema.

	- **Bounded Context 1: Notification Management**
	    ![Bounded Context 1](https://media.discordapp.net/attachments/912089666939916348/1149126632427241482/Bounded_Context_Canvas_by_Nick_Tune_6.jpg?width=1351&height=668)
	- **Bounded Context 2: Project Management**
	    ![Bounded Context 2](https://media.discordapp.net/attachments/912089666939916348/1149126632745992222/Bounded_Context_Canvas_by_Nick_Tune_7.jpg?width=1301&height=668)
	- **Bounded Context 3: Crop Management**
	    ![Bounded Context 3](https://media.discordapp.net/attachments/912089666939916348/1149126634281123951/Bounded_Context_Canvas_by_Nick_Tune_3.jpg?width=1371&height=669)
	- **Bounded Context 4: Knowledge Management**
	![Bounded Context 4](https://media.discordapp.net/attachments/912089666939916348/1149126634012692480/Bounded_Context_Canvas_by_Nick_Tune_2.jpg?width=1345&height=669)
	- **Bounded Context 5: Specialist Contact**
        ![Bounded Context 5](https://media.discordapp.net/attachments/912089666939916348/1149126633060585522/Bounded_Context_Canvas_by_Nick_Tune_8.jpg?width=1336&height=669)
	- **Bounded Context 6: Identity Access**
        ![Bounded Context 6](https://media.discordapp.net/attachments/912089666939916348/1149126633467428904/Bounded_Context_Canvas_by_Nick_Tune.jpg?width=1326&height=669)



### 4.1.2. Context Mapping. 
		
El Context Mapping es una metodología empleada en el desarrollo de software para comprender y representar gráficamente las conexiones entre los usuarios, los conceptos y los equipos que forman parte de un proyecto.

### 4.1.3. Software Architecture. 
#### 4.1.3.1. Software Architecture System Landscape Diagram. ![Landscape Diagram](https://media.discordapp.net/attachments/1143666758042013892/1149092447788486677/landscape.drawio.png?width=1025&height=405) 
#### 4.1.3.2. Software Architecture Context Level Diagrams. ![Context diagram](https://media.discordapp.net/attachments/1143666758042013892/1149089602737537094/Context.drawio.png?width=954&height=473)
#### 4.1.3.2. Software Architecture Container Level Diagrams. ![Container DIagram](https://media.discordapp.net/attachments/1143666758042013892/1149106586892111892/container.drawio.png?width=454&height=473)
#### 4.1.3.3. Software Architecture Deployment Diagrams. ![Deployment Diagram](https://media.discordapp.net/attachments/1149587894416183327/1149594351039684608/C4-Deployme.drawio_1.png?width=702&height=473) 

## 4.2. Tactical-Level Domain-Driven Design.

El Tactical-Level Domain-Driven Design es una metodología de diseño de software que se enfoca en la representación del dominio y la estructuración de objetos en niveles específicos, que abarcan desde la lógica empresarial hasta la aplicación y la infraestructura.
### 4.2.1. Bounded Context: User Acount Manager
#### 4.2.1.1. Domain Layer.
- Nombre: User
- Categoria: Entity
- Propósito: Almacenar datos de nuestros usuarios
- Atributos
	| Nombre    | Tipo de dato | VisibilidadDescripción                                  |
	|-----------|--------------|---------------------------------------------------------|
	| id        | int          | private     | Id identidad                              |
	| email     | string       | private     | Almacena email del usuario                |
	| password  | string       | private     | Almacena contraseña de acceso del usuario |
- Métodos:
	| Nombre       | Tipo de dato | VisibilidadDescripción                                   |
	|--------------|--------------|----------------------------------------------------------|
	| User         | void         | public     |Constructor de la identidad                   |
	| getFullName  | string       | public      | Obtieel nombre completo del usuario        |
	| validPassword| bool  | public      | Valida la contraseña del usuario   |                

#### 4.2.1.2 Interface layer
- Nombre: Users.controller
- Categorìa: Controller
- Propòsito: Controlar registro de usuarios
- Mètodos:
	| Nombre     | Tipo de dato | Visibilidad | Descripción                             |
	|------------|--------------|-------------|-----------------------------------------|
	| Register   | Promise      | public      | Registra un usuario nuevo               |
	| Log In     | Promise      | public      | Permite iniciar sesiòn al usuario       |
	| ModifyUser | Promise      | public      | Permite modificar los datos del usuario |
	| DeleteUser | Promise      | public      | Permite eliminar un usuario             |
#### 4.2.1.3 Application Layer
- Nombre: CreateUser.handler
- Categorìa: Handler
- Propòsito: Handler para registrar un usuario
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| CreateUser.handler | void         | public      | Constructor             |
	| execute  | void         | public      | Permite registrar al usuario |	
- Nombre: CreateUser.command
- Categorìa: Command
- Propòsito: Command para registrar un usuario
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| CreateUser.command | void         | public      | Constructor          	|
- Nombre: LogIn.handler
- Categorìa: Handler
- Propòsito: Handler para logear un usuario
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| LogIn.handler | void         | public      | Constructor             |
	| execute  | void         | public      | Permite iniciar sesiòn al usuario |	
- Nombre: LogIn.command
- Categorìa: Command
- Propòsito: Command para logear un usuario
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| LogIn.command | void         | public      | Constructor          	|

- Nombre: DeleteUser.handler
- Categorìa: Handler
- Propòsito: Handler para eliminar un usuario
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| DeleteUser.handler | void         | public      | Constructor             |
	| execute  | void         | public      | Permite elminar datos del usuario 
- Nombre: ModifiUser.command
- Categorìa: Command
- Propòsito: Command para modificar un usuario
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| DeleteUser.command | void         | public      | Constructor          	|
			
## **4.2.1.4 Infrastructure Layer**
- Nombre: UserRepository
- Categorìa: Repository
- Propòsito: Obtener datos del usuario
- Mètodos: 
	| Nombre  | Tipo de dato       | Visibilidad | Descripción                                   |
	|---------|--------------------|-------------|-----------------------------------------------|
	| getById | getUserResource    | public      | Devuelve los datos necesarios de un usuario   |
	| getAll  | array              | public      | Devuelve todos los objetos en un arreglo      |
	| create  | createUserResource | public      | Crea un nuevo objeto                          |
	| update  | updateUserResource | public      | Actualiza o modifica los valores de un objeto |
	| delete  | void               | public      | Elimina un objeto                             |
## **4.2.1.5. Bounded Context Software Architecture Component Level Diagrams**

El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes User](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/c4_component_user.PNG?raw=true)

## **4.2.1.6 Bounded Context Software Architecture Code Level Diagrams**

Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código			

## **4.2.1.6.1 Bounded Context Domain Layer Class Diagrams**

Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
![Diagrama de clases user](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/diagram_class_user.PNG?raw=true)

## **4.2.1.6.2 Bounded Context Database Diagrams**

Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos. Este diagrama muestra la relación entre la tabla Shipments y la tabla Comments.
![Diagrama de base de datos](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/database_diagram_user.PNG?raw=true)
	
## **4.2.2. Bounded Context: Suscriptions and Payments**
## **4.2.1.1. Domain Layer.** 
- Nombre: Suscription
- Categoria: Entity
- Propósito: Almacenar datos de las suscripciones de los usuarios
- Atributos
	| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
	|-----------|--------------|-------------|----------------------------------------------|
	| id        | int          | private     | Id de identidad                              |
	|planType|PlanType|private|Tipo de plan|
	|profileId|int|private|Id del perfil|
	|payDate|Datetime|private|Fecha del siguiente pago|
	|status|string|private|Estado de la suscripción|
	|cost|float|private|Costo de la suscripción
	
- Métodos:
	| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
	|--------------|--------------|-------------|-----------------------------------------------|
	| getPayDate  |Datetime      | public      | Obtiene la fecha de pago      |
	| getPlanType     | string       | public      | Obtiene el tipo de plan                    |
	| updatePlan|string|public|Actualiza el tipo de plan

- Nombre: PlanType
- Categorìa: Enum
- Propòsito: Proveer los tipos de plan
- Atributos: 
	| Nombre       | Tipo de dato | Visibilidad |
	|--------------|--------------|-------------|
	| MONTHLY       | string       | public      |
	| YEAR   | string       | public     
- Nombre: Order
- Categoría: Entity
- Propósito: Almancear información de las órdenes de pago
- Atributos:
	|Nombre|Tipo de dato|Visibilidad|Descripción|
	|------|------------|-----------|-----------|
	|id|int|private|Id de la identidad|
	|amount|float|private|Monto a pagar|
	|status|OrderStatus|private|Estado del pago|
	|profileId|int|private|Id del perfi
- Nombre: OrderStatus
- Categorìa: Enum
- Propòsito: Proveer los estados de una orden de pago
- Atributos: 
	| Nombre       | Tipo de dato | Visibilidad |
	|--------------|--------------|-------------|
	| CANCELED       | string       | public      |
	| IN_WAIT   | string       | public      |
## **4.2.1.2 Interface layer**
- Nombre: Suscription.controller
- Categorìa: Controller
- Propòsito: Controlar registro de suscripciones
- Mètodos:
	| Nombre     | Tipo de dato | Visibilidad | Descripción                             |
	|------------|--------------|-------------|-----------------------------------------|
	| Register   | Promise      | public      | Registra una suscripciones nueva              |
	| ModifySuscription| Promise      | public      | Permite modificar los datos de una suscripción |
	| DeleteSuscription | Promise      | public      | Permite eliminar una suscripción    |
## **4.2.1.3 Application Layer**
- Nombre: AssignProfileCommandHandler
- Categoría: COmmandHandler
- Propósito: Handler para la asignación de una suscripción
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Suscription>|public|Método de ejecución del comando|

- Nombre: UpdateSuscriptionCOmmandHandler
- Categoría: Command Handler
- Propósito: Handler para la actualización de una suscripción
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Suscription>|public|Método de ejecución del comando|

- Nombre: SuscriptionAssignedEventHandler
- Categoría: Event Handler
- Propósito: Gestionar la asignación de una suscripción
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Suscription>|public|Método de ejecución del event
- Nombre: SuscriptionUpdatedEventHandler
- Categoría: Event Handler
- Propósito: Gestionar la actualización de una suscripción
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Suscription>|public|Método de ejecución del comand
- Nombre: CreatePayOrderCommandHandler
- Categoría: Command Handler
- Propósito: Handler para la creación de una orden de pago
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Order>|public|Método de ejecución del comand
- Nombre: PayOrderCOmmandHandler
- Categoría: Command Handler
- Propósito: Handler para el pago de órdenes
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Order>|public|Método de ejecución del comand
- Nombre: PayOrderCreatedEventHandler
- Categoría: Event Handler
- Propósito: Gestionarla creación de una orden de pago
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Order>|public|Método de ejecución del event
- Nombre: OrderPayedEventHandler
- Categoría: Event Handler
- Propósito: Gestionar el p
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Order>|public|Método de ejecución del evento|
			
## **4.2.1.4 Infrastructure Layer**
- Nombre: SuscriptionRepository
- Categorìa: Repository
- Propòsito: Obtener datos de las suscripciones
- Mètodos: 
	| Nombre  | Tipo de dato       | Visibilidad | Descripción                                   |
	|---------|--------------------|-------------|-----------------------------------------------|
	| getById | getSuscriptionResource    | public      | Devuelve una suscripción por su Id   |
	|getByProfileId|getSuscriptionResource|public|Devuelve una suscripción el id del perfil
	| getAll  | array              | public      | Devuelve todas las suscriciones      |
	| create  | createSuscriptionResource | public      | Crea ususcripción                          |
	| update  | updateSuscriptionResource | public      | Actualiza una suscripción |
	| delete  | void               | public      | Elimina una suscripción                          |
## **4.2.1.5. Bounded Context Software Architecture Component Level Diagrams**

El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes User](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/c4_component_suscription.PNG?raw=true)
## **4.2.1.6 Bounded Context Software Architecture Code Level Diagrams**

Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código		

## **4.2.1.6.1 Bounded Context Domain Layer Class Diagrams**

Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
![Diagrama clases User](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/diagram_class_suscription.PNG?raw=true)

## **4.2.1.6.2 Bounded Context Database Diagrams**

Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos. Este diagrama muestra la relación entre la tabla Shipments y la tabla Comments.
![Database diagram](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/database_diagram_suscription.PNG?raw=true)

## **4.2.2. Bounded Context: Profile Management**
## **4.2.2.1. Domain Layer.** 
- Nombre: Profile
- Categoria: Entity
- Propósito: Almacenar datos de los perfiles de usuarios
- Atributos
	| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
	|-----------|--------------|-------------|----------------------------------------------|
	| id | int       | private     | Id de identidad               |
	|userId|int|private|Id del usuario|
	| suscripcionId        | int          | private     | Id del la suscripcion             |
	| firstName | string       | private     | Almacena el nombre del usuario               |
	| lastName  | string       | private     | Almacena el apellido del usuario             |
	| cellphone  | string       | private     | Almacena el número telefónico del usuario        |
	| rol  | UserRol     | private     | Almacena el tipo de usuario      |

- Nombre: Rol
- Categorìa: Enum
- Propòsito: Proveer los tipos de usuario
- Atributos: 
	| Nombre       | Tipo de dato | Visibilidad |
	|--------------|--------------|-------------|
	| FARMER       | string       | public      |
	| SPECIALIST   | string       | public      |
	| ADM          | string       | public      |

- Métodos:
	| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
	|-----------|--------------|-------------|----------------------------------------------|
	| constructor | Profile       | public     | Constructor de la clase              |
	|getFullname|string|public|devuelve el nombre completo del perfil|
	|setSuscription|void|public|Permite editar la suscripción del usuari
- Nombre: IProfileRepository
- Categoría: Repository
- Propósito: Persistir los perfiles
	| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
	|-----------|--------------|-------------|----------------------------------------------|
	|getByUserId|ProfileResource|public|Devuelve el perfil según el id de usuario|
	|add|void|public|Añade un perfil|
	|update|void|public|Modifica un perfil|
	|delete|void|public|Elimina un perfil|
			
## **4.2.2.2 Interface layer**
- Nombre: Profile.controller
- Categorìa: Controller
- Propòsito: Controlar registro de perfiles
- Mètodos:
	| Nombre     | Tipo de dato | Visibilidad | Descripción                             |
	|------------|--------------|-------------|-----------------------------------------|
	| Post   | Promise      | public      | Registra un nuevo perfil              |
	| GetAll | Promise      | public      | Devuelve todos los perfiles |
	|FindByUserId|Promise|public|Devuelve un érfil por el id del usuario|
	|Put|Promise|public|Modifica un perfil|
	|Delete|Promise|Elimina un perfil|

## **4.2.2.3 Application Layer**
- Nombre: 
- Categoría: 
- Propósito:
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Profile>|public|Método de ejecución del comando|

- Nombre: CreateUserProfileCommandHandler
- Categoría: Command Handler
- Propósito: Handler para la creación de un perfil de usuario
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handle|Promise<Profile>|public|Método de ejecución del comando|

- Nombre: ModifyUserProfileCommandHandler
- Categoría: Command Handler
- Propósito: Handler para la modificación de un perfil de usuario
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Profile>|public|Método de ejecución del comando|

- Nombre: DeleteUserProfileCommandHandler
- Categoría: Command Handler
- Propósito: Handler para la eliminación de un perfil de usuario
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Profile>|public|Método de ejecución del comand
- Nombre: UserProfileModifiedEventHandler
- Categoría: Event Handler
- Propósito: Gestionar la modificación de un perfil
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Profile>|public|Método de ejecución del event
- Nombre: UserProfileDeletedEventHandler
- Categoría: Event Handler
- Propósito: Gestionar la eliminación de un perfil
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Profile>|public|Método de ejecución del event
- Nombre: UserProfileCreatedEventHandler
- Categoría: Event Handler
- Propósito: Gestionar la creación de un perfil
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<Profile>|public|Método de ejecución del evento|
			
## **4.2.2.4 Infrastructure layer**
- Nombre: ProfileRepository
- Categoría: Repository
- Propósito: Persistir los perfiles
	| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
	|-----------|--------------|-------------|----------------------------------------------|
	|getByUserId|ProfileResource|public|Devuelve el perfil según el id de usuario|
	|add|void|public|Añade un perfil|
	|update|void|public|Modifica un perfil|
	|delete|void|public|Elimina un perfil|
		
## **4.2.2.5. Bounded Context Software Architecture Component Level Diagrams**

El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes ](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/c4_component_profile.PNG?raw=true)

## **4.2.2.6 Bounded Context Software Architecture Code Level Diagrams**

Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código				

## **4.2.2.6.1 Bounded Context Domain Layer Class Diagrams**

Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
![Diagrama clases PLantas](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/diagram_class_profile.PNG?raw=true)

## **4.2.2.6.2 Bounded Context Database Diagrams**

Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos. 
![DC profile](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/database_diagram_profile.PNG?raw=true)


## **4.2.2. Bounded Context: Plant Management**
## **4.2.2.1. Domain Layer.** 
- Nombre: Plant
- Categoria: Entity
- Propósito: Almacenar datos de las plantas
- Atributos
	| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
	|-----------|--------------|-------------|----------------------------------------------|
	| id | int       | private     | Id de identidad               |
	| plantName        | string          | private     | Nombre de la planta                         |
	| plantDescription        | string          | private     | Descripción de la planta        
- Métodos:
	| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
	|--------------|--------------|-------------|-----------------------------------------------|
	| Plant       | void         | public      | Constructor de la identidad                   |
	| getPlantName  | string       | public      | Obtiene el nombre de la planta       |
	| getDescription      | string       | public      | Retorna la desripción                
- Nombre: IPlantRepository
- Categoría: Repository
- Propósito: Persistir las plantas
- Métodos: 
	| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
	|--------------|--------------|-------------|-----------------------------------------------|
	| IPlantRepository       | ISuscriptionRepository         | public      | Constructor de identidad                   |
	| add  | void       | public      | Crear una planta      |
	| updatePlant     | void       | public      |Permite actualizar los datos de una planta|
	|deletePlant|void|public|Permite eliminar una planta|
	| ListPlants|array|public|Devuelve una lista de todas las plantas|
	|FindByName|promise<PlantResource>|public|Devuelve una planta por el nombre|
	|FindById|promise<PlantResource|publicDevuelve una planta por el Id|
		

#### 4.2.2.2 Interface layer
- Nombre: Plant.controller
- Categorìa: Controller
- Propòsito: Controlar registro de suscripciones
- Mètodos:
	| Nombre     | Tipo de dato | Visibilidad | Descripción                             |
	|------------|--------------|-------------|-----------------------------------------|
	| Post   | Promise      | public      | Registra una nueva planta              |
	| GetAll | Promise      | public      | Devuelve todas las plantas |
	|GetByName|Promise|public|Devuelve una plata por su nombre|
	|GetById|Promise|public|Devuelve una planta por su id|
	|deleteById|Promise|Elimina una planta|

#### 4.2.2.3 Application Layer
- Nombre: RegisterPlant.handler
- Categorìa: Handler
- Propòsito: Handler para registrar una planta
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| RegisterPlant.handler | void         | public      | Constructor             |
	| execute  | void         | public      | Permite registrar una planta |	
- Nombre: RegisterPlant.command
- Categorìa: Command
- Propòsito: Command para registrar una planta
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| RegisterPlant.command | void         | public      | Constructor          	|
- Nombre: SearchPlant.handler
- Categorìa: Handler
- Propòsito: Handler para buscar una planta
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| SearchPlant.handler | void         | public      | Constructor             |
	| execute  | void         | public      | Permite buscar una planta |	
- Nombre: SearchPlant.command
- Categorìa: Command
- Propòsito: Command para registrar una planta
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| SearchPlant.command | void         | public      | Constructor          	|
- Nombre: IdentifyPlant.handler
- Categorìa: Handler
- Propòsito: Handler para identificar una planta
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| IdentifyPlant.handler | void         | public      | Constructor             |
	| execute  | void         | public      | Permite identificar una planta |	
- Nombre: IdentifyPlant.command
- Categorìa: Command
- Propòsito: Command para identificar una planta
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| IdentifyPlant.command | void         | public      | Constructor          	|
			
			
#### 4.2.2.4 Infrastructure Layer
- Nombre: PlantRepository
- Categoría: Repository
- Propósito: Persistir las plantas
- Métodos: 
	| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
	|--------------|--------------|-------------|-----------------------------------------------|
	| PlantRepository       | ISuscriptionRepository         | public      | Constructor de la identidad                   |
	| add  | void       | public      | Crear una planta      |
	| updatePlant     | void       | public      |Permite actualizar los datos de una planta|
	|deletePlant|void|public|Permite eliminar una planta|
	| ListPlants|array|public|Devuelve una lista de todas las plantas|
	|FindByName|promise<PlantResource>|public|Devuelve una planta por el nombre|
	|FindById|promise<PlantResource|publicDevuelve una planta por el Id|
				
#### 4.2.2.5. Bounded Context Software Architecture Component Level Diagrams

El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. 
![Diagrama de componentes plantas](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/c4_component_plant.PNG?raw=true)

#### 4.2.2.6 Bounded Context Software Architecture Code Level Diagrams

Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código		

##### 4.2.2.6.1 Bounded Context Domain Layer Class Diagrams

Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
![Diagrama clases PLantas](https://cdn.discordapp.com/attachments/1143666758042013890/1153884913712509080/image.png)

##### 4.2.2.6.2 Bounded Context Database Diagrams

Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos. Este diagrama muestra la relación entre la tabla Shipments y la tabla Comments.

## **4.2.3. Bounded Context: IoT Asset Management**
## **4.2.2.1. Domain Layer.** 
- Nombre: IoTDevice
- Categoría: Entity
- Propósito: Almacenar datos de los dispositivos IoT
- Atributos:
	| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
	|-----------|--------------|-------------|----------------------------------------------|
	| Id | int       | private     | Id de identidad               |
	| deviceName        | string          | private     | Nombre del dispositivo  |
	|status|Status|private|Estado del dispositivo|
	|registerAt|date|private|Fecha de creación|
- Nombre: Status
- Categoría: Enum
- Propósito: Almacenar los estados de un dispositivo IoT
- Atributos: 
	| Nombre    | Tipo de dato | Visibilidad |
	|-----------|--------------|-------------|
	| ON | string       | public    |
	| OFF  | string          | public     |
		

## **4.2.1.2 Interface layer**
- Nombre: IoT.controller
- Categorìa: Controller
- Propòsito: Controlar registro de dispositivos IoT
- Mètodos:
	| Nombre     | Tipo de dato | Visibilidad | Descripción                             |
	|------------|--------------|-------------|-----------------------------------------|
	| Register   | Promise      | public      | Registra un nuevo dispositivo IoT               |
	| Modify | Promise      | public      | Permite modificar dispositivo IoT |
	| GetIoTByOd|Promise|public|Permite obtener un dispositivo IoT|
	| GetIoTByUserId|Promise|public|Permite obtener una lista de los dispositivos de un usuario|
	| DeleteIoT | Promise      | public      | Permite eliminar un dispositivo  |
## **4.2.1.3 Application Layer**
- Nombre: RegisterIoTDeviceCommandHandler
- Categoría: Command Handler
- Propósito: Handler de registro de dispositivos IoT
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<IoTDevice>|public|Método de ejecución del comando|

- Nombre: DeleteIoTDeviceCOmmandHandler
- Categoría: Command Handler
- Propósito: Handler para la eliminación de un dispositivo IoT
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<IoTDevice>|public|Método de ejecución del comand
- Nombre: AssignCroptoaIoTDeviceCommandHandler
- Categoría: Command Handler
- Propósito:
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<IoTDevice>|public|Método de ejecución del comando|

- Nombre: ActivateMonitoringCropCommandHandler
- Categoría: Command Handler
- Propósito: Handler para la activación de monitoreo de cultivo
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<IoT>|public|Método de ejecución del comand
- Nombre: IoTDeviceRegisteredEventHandler
- Categoría: Event Handler
- Propósito: Gestionar registro de dispositivos IoT
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<IoTDevice>|public|Método de ejecución del comando|

- Nombre: IoTDeviceDeletedEventHandler
- Categoría: Event Handler
- Propósito: Gestionar la eliminación de un dispositivo IoT
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<IoTDevice>|public|Método de ejecución del comand
- Nombre: CroptoaIoTDeviceAssignedEventHandler
- Categoría: Command Handler
- Propósito: Gestionar la asignación de un dispositivo IoT a un cultivo
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<IoTDevice>|public|Método de ejecución del comando|

- Nombre: MonitoringCropActivatedEventHandler
- Categoría: Event Handler
- Propósito: Gestionar para la activación de monitoreo de cultivo
	|Nombre|Tipo de retorno|Visibilidad|Descripción|
	|------|---------------|-----------|-----------|
	|Handler|Promise<IoT>|public|Método de ejecución del comando|
			
#### 4.2.3.4 Infrastructure Layer
- Nombre: SuscriptionRepository
- Categoría: Repository
- Propósito: Persistir las suscripciones
- Métodos: 
	| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
	|--------------|--------------|-------------|-----------------------------------------------|
	| SuscriptionRepository       | SuscriptionRepository         | public      | Constructor de la identidad                   |
	| add  | void       | public      | Crear una suscripción      |
	| updateDayPay      | void       | public      | Permite actualizar la fecha de pago de la suscripción                |
	| updatePlan|Plan|public|Permite actualizar el tipo de plan de la suscripción|
	|	deletePlan|void|public|Permite eliminar planes|

- Nombre: PlanRepository
- Categoría: Repository
- Propósito: Persistir los planes
- Métodos: 
	| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
	|--------------|--------------|-------------|-----------------------------------------------|
	| PlanRepository      | PlanRepository         | public      | Constructor de la identidad                   |
	| add  | void       | public      | Crear un plan      |
	| delete | void |public|Eliminar un plan|
				
#### 4.2.3.5. Bounded Context Software Architecture Component Level Diagrams

El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. 
![Diagrama de componentes sUSCRIPTION](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/c4_omponent_iotdevice.PNG?raw=true)

#### 4.2.3.6 Bounded Context Software Architecture Code Level Diagrams
Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código				
##### 4.2.3.6.1 Bounded Context Domain Layer Class Diagrams
Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
![Diagrama clases](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/diagram_class_iot.PNG?raw=true)
##### 4.2.1.6.2 Bounded Context Database Diagrams
Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos.
![BD iot](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/database_diagram_iot.PNG?raw=true)
		
## **4.2.4. Bounded Context: Crop Management**
## **4.2.4.1. Crop.** 
- Nombre: Crop
- Categoria: Entity
- Propósito: Almacenar los datos de los cultivos
- Atributos
	| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
	|-----------|--------------|-------------|----------------------------------------------|
	| Id | int       | private     | Id de identidad               |
	| userId        | int          | private     | Id del usuario al que pertenece         |
	|plantId|int|private|Id de planta que se está cultivando|
	|createAt|date|private|Fecha de creación|
	|updateAt|date|private|Última fecha de actualización|
	|imageSrc|string|private|Enlace a la imagen del cultivo|
- Métodos:
	| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
	|--------------|--------------|-------------|-----------------------------------------------|
	| Crop       | Crop         | public      | Constructor de la identidad                   |
	| addReport  | void       | public      | Añade un reporte al cultivo       |
	| getReport      | String       | public      | Retorna un reporte del cultivo  |
	| ModifyLastUpdate|void|private|Modifica la última fecha de actualizació
- Nombre: Report
- Categoría: Entity
- Propósito: Almacenar los reportes de los cultivos
- Atributos:
	| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
	|-----------|--------------|-------------|----------------------------------------------|
	| Id | int       | private     | Id de identidad               |
	| createAt|date|private|Fecha de creacion|
	| imageSrc|string|private|Enlace a la imagen del cultivo al momento de crear el reporte|
	|Description|string|private|Descripción de como se encuentra el cultivo al momento de generar reporte|



## **4.2.4.2 Interface layer**
- Nombre: Crop.controller
- Categorìa: Controller
- Propòsito: Controlar registro de cultivos
- Mètodos:
	| Nombre     | Tipo de dato | Visibilidad | Descripción                             |
	|------------|--------------|-------------|-----------------------------------------|
	| Register   | Promise      | public      | Registra un nuevo cultivo               |
	| Modify | Promise      | public      | Permite modificar cultivo de un usuario |
	| GetCropById|Promise|public|Permite obtener un cultivo|
	| GetCropsByUserId|Promise|public|Permite obtener una lista de los cultivos de un usuario|
	| DeleteCrop | Promise      | public      | Permite eliminar un cultivo  |
			
## **4.2.4.3 Application Layer**
- Nombre: RegisterCrop.handler
- Categorìa: Handler
- Propòsito: Handler para registrar un cultivo
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| RegisterCrop.handler | void         | public      | Constructor             |
	| execute  | void         | public      | Permite registrar un cultivo |	

- Nombre: DisplayInformation.handler
- Categorìa: Handler
- Propòsito: Handler para mostrar la información delcultivo en tiempo real
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| DisplayInformation.handler | void         | public      | Constructor     |
	| execute  | void         | public      | Permite mostrar información en tiempo real |	
- Nombre: DisplayInformation.command
- Categorìa: Command
- Propòsito: Command para mostrar la información delcultivo en tiempo real
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| DisplayInformation.command | void         | public      | Constructor      |


- Nombre: AddReport.handler
- Categorìa: Handler
- Propòsito: Handler para registrar un reporte de cultivo
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| AddReport.handler | void         | public      | Constructor             |
	| execute  | void         | public      | Permite registrar un cultivo 
- Nombre: AddReport.command
- Categorìa: Command
- Propòsito: Command para asignar una suscripción
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| AddReport.command | void         | public      | Constructor          


- Nombre: DeleteCrop.handler
- Categorìa: Handler
- Propòsito: Handler para eliminar un cultivo
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| DeleteCrop.handler | void         | public      | Constructor     |
	| execute  | void         | public      | Permite mostrar información en tiempo real 
- Nombre: DeleteCrop.command
- Categorìa: Command
- Propòsito: Command para mostrar la información del cultivo en tiempo real
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| DeleteCrop.command | void         | public      | Constructor      |

			
#### 4.2.4.4 Infrastructure Layer
- Nombre: CropRepository
- Categoría: Repository
- Propósito: Persistir los cultivos
- Métodos: 
	| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
	|--------------|--------------|-------------|-----------------------------------------------|
	| CropRepository       | CropRepository         | public      | Constructor de la identidad |
	| add  | void       | public      | Crear un cultivo     |
	| AddReport      | void       | public      | Permite actualizar un reporte al cultivo|
	| DeleteCrip|void|public|Permite eliminar un cultivo|

- Nombre: IoTRepository
- Categoría: Repository
- Propósito: Persistir los dispositivos
- Métodos: 
	| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
	|--------------|--------------|-------------|-----------------------------------------------|
	| IoTRepository      | IoTRepository         | public      | Constructor de la identidad                   |
	| add  | void       | public      | Registrar un dispositivo      |
	| FinByUserId  | array       | public      | Devuelve una lista de dispositivos IoT por Id del usuario |
	| FinById  | IoTResource       | public      | Devuelve un IoT device |
	| delete | void |public|Eliminar un dispositivo|
				
#### 4.2.4.5. Bounded Context Software Architecture Component Level Diagrams
El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes Crop](https://cdn.discordapp.com/attachments/1149587894416183327/1153891010666053642/image.png)
#### 4.2.4.6 Bounded Context Software Architecture Code Level Diagrams
Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código				
##### 4.2.4.6.1 Bounded Context Domain Layer Class Diagrams
Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
![Diagrama clases Suscription](https://cdn.discordapp.com/attachments/1143666758042013890/1152481306656120885/image.png)
##### 4.2.4.6.2 Bounded Context Database Diagrams
Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos.
![BD iot](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/database_diagram_iot.PNG?raw=true)

### **4.2.4. Bounded Context: Advisory Management**
#### **4.2.4.1. Domain Layer.** 
- Nombre: Project
- Categoria: Entity
- Propósito: Almacenar los datos de los proyectos
- Atributos :
	| Nombre    | Tipo de dato | VisibilidadDescripción                                  |
	|-----------|--------------|---------------------------------------------------------|
	| Id | int       | private     | Id identidad               |
	|cropId|int|private|Id del crop|
	|title|string|private|Título del paso|

- Nombre: Step
- Categoría: Entity
- Propósito: Almacenar los pasos de un proyecto
- Atributos:
	| Nombre    | Tipo de dato | VisibilidadDescripción                                  |
	|-----------|--------------|---------------------------------------------------------|
	| Id | int       | private     | Id identidad               |
	|orderStep|int|private|Número de orden|
	|title|string|private|Título del paso|
	|description|string|private|Título|
	|status|StepStatus|string|private|Estado del paso|
	|deadLine|date|string|Fecha límite para cumplir el paso|

- Nombre: StepStatus
- Categoría: Enum
- Propósito: Almacenar los estados de un paso
- Atributos: 
	| Nombre    | Tipo de dato | Visibilidad |
	|-----------|--------------|-------------|
	| IN_PROCESS | int       | public    | 
	|ACCOMPLISHED|int|public|
	|FAILED|string|public|
		
#### 4.2.5.2 Interface layer
- Nombre: Project.controller
- Categorìa: Controller
- Propòsito: Controlar registro de proyectos
- Mètodos:
	| Nombre     | Tipo de dato | Visibilidad | Descripción                             |
	|------------|--------------|-------------|-----------------------------------------|
	| Register   | Promise      | public      | Registra un nuevo proyecto     |
	| Modify | Promise      | public      | Permite modificar proyecto de un cultivo |
	| GetProjectById|Promise|public|Permite obtener un cultivo|
	| GetProjectByUserId|Promise|public|Permite obtener una lista de los proyecto de un usuario|
	| DeleteProject | Promise      | public      | Permite eliminar un proyecto  |

#### 4.2.5.3 Application Layer
- Nombre: CreateProject.event-handler
- Categorìa: Event Handler
- Propòsito: Gestionar la creaciòn de un proyecto
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| handle | void         | public      | Constructor             |
- Nombre: CreateStep.event-handler
- Categorìa: Event-Handler
- Propòsito: GEstionar la creaciòn de un paso de proyecto
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| handler | void         | public      | Constructor             |	
- Nombre: ASsigProject.event-handler
- Categorìa: Event-Handler
- Propòsito: GEstionar la asignaciòn de un proyecto
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| handler | void         | public      | Constructor             |	

			
#### 4.2.5.4 Infrastructure Layer
- Nombre: ProjectRepository
- Categoría: Repository
- Propósito: Persistir los proyectos
- Métodos: 
	| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
	|--------------|--------------|-------------|-----------------------------------------------|
	| ProjectRepository       | CropRepository         | public      | Constructor de la identidad |
	| add  | void       | public      | Crear un proyecto     |
	| AddStep      | void       | public      | Permite aañadir un paso al proyecto|
	| DeleteProyect|void|public|Permite eliminar un proyecto|
	|DeleteStep|void|public|Permite eliminar un paso dle proyecto|
	|ModifiStep|public|Permite modificar un paso del proyecto|

				
#### 4.2.5.5. Bounded Context Software Architecture Component Level Diagrams
El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes sUSCRIPTION](https://cdn.discordapp.com/attachments/1143666758042013890/1152477663966011422/image.png)
#### 4.2.5.6 Bounded Context Software Architecture Code Level Diagrams
Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código				
##### 4.2.5.6.1 Bounded Context Domain Layer Class Diagrams
Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
![Diagrama clases Suscription](https://cdn.discordapp.com/attachments/1143666758042013890/1152481306656120885/image.png)
##### 4.2.5.6.2 Bounded Context Database Diagrams
Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos. Este diagrama muestra la relación entre la tabla Shipments y la tabla Comments.
![BD iot](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/database_diagram_iot.PNG?raw=true)
#### 4.2.6. Bounded Context: Notification
#### 4.2.6.1. Domain Layer.
- Nombre: Notification
- Categoria: Entity
- Propósito: Almacenar los datos de las notificaciones
- Atributos
	| Nombre    | Tipo de dato | VisibilidadDescripción                                  |
	|-----------|--------------|---------------------------------------------------------|
	| Id | int       | private     | Id identidad               |
	| userId        | int          | private     | Id dusuario         |
	|createAt|date|private|Fecha de creación|
	|importance|NotificationImportane|private|Importancde la notificación|
	|title|string|private|Título de la notificación|
	|body|string|private|Cuerpo de la notificación|
	
- Métodos:
	| Nombre       | Tipo de dato | VisibilidadDescripción                                   |
	|--------------|--------------|----------------------------------------------------------|
	| Notification       | Constructor       public      | Constructor de identidad                   |
	| getTitle  | string   | public      | Obtiene titulo de la notificacion |
	|getBody|string|public|Obtiene el cuerpo de notificación|

- Nombre: NotificationImportance
- Categoría: Entity
- Propósito: Almacenar los pasos de un proyecto
- Atributos:
	| Nombre    | Tipo de dato | VisibilidadDescripción                                  |
	|-----------|--------------|---------------------------------------------------------|
	| Id | int       | private     | Id identidad               |
	|orderStep|int|private|Número de orden|
	|title|string|private|Título del paso|
	|description|string|private|Título|
	|status|StepStatus|string|private|Estado del paso|
	|deadLine|date|string|Fecha límite para cumplir el paso|

- Nombre: NotificationImportance
- Categoría: Enum
- Propósito: Almacenar la importancia de cada notificación
- Atributos: 
	| Nombre    | Tipo de dato | Visibilidad |
	|-----------|--------------|-------------|
	| LOW | int       | public    | 
	|URGENT|int|public|
	|MEDIUM|string|public|
		
#### 4.2.6.2 Interface layer
- Nombre: Notification.controller
- Categorìa: Controller
- Propòsito: Controlar registro de notificaciones
- Mètodos:
	| Nombre     | Tipo de dato | Visibilidad | Descripción                             |
	|------------|--------------|-------------|-----------------------------------------|
	| Register   | Promise      | public      | Registra un nuevo proyecto     |
	| Modify | Promise      | public      | Permite modificar proyecto de un cultivo |
	| GetNotificationById|Promise|public|Permite obtener un cultivo|
	| GetNotificationsUserId|Promise|public|Permite obtener una lista de los proyecto de un usuario|
	| DeleteProject | Promise      | public      | Permite eliminar un proyecto  |

#### 4.2.6.3 Application Layer
- Nombre: NotificationSendeed.event-handler
- Categorìa: Event Handler
- Propòsito: Gestionar el envío de una notificación
- Mètodos: 
	| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
	|----------|--------------|-------------|-----------------------------------|
	| handle | void         | public      | Constructor             |


			
#### 4.2.6.4 Infrastructure Layer
- Nombre: NotificationRepository
- Categoría: Repository
- Propósito: Persistir las notificaciones
- Métodos: 
	| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
	|--------------|--------------|-------------|-----------------------------------------------|
	| NotificationRepository       | CropRepository         | public      | Constructor de la identidad |
	| add  | void       | public      | Crear una notificación     |
	| DeleteProyect|void|public|Permite eliminar un proyecto|

				
#### 4.2.6.5. Bounded Context Software Architecture Component Level Diagrams
El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes sUSCRIPTION](https://cdn.discordapp.com/attachments/1143666758042013890/1152477663966011422/image.png)
#### 4.2.6.6 Bounded Context Software Architecture Code Level Diagrams
Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código				
##### 4.2.6.6.1 Bounded Context Domain Layer Class Diagrams
Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
![Diagrama clases Suscription](https://cdn.discordapp.com/attachments/1143666758042013890/1152481306656120885/image.png)
##### 4.2.6.6.2 Bounded Context Database Diagrams
Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos.
![BD iot](https://github.com/DevIOT-AgriPure/Project-Report/blob/feature/capitulo-4/images/bcArchitecture/database_diagram_iot.PNG?raw=true)	
