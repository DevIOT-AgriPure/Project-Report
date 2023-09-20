# Project-Report
New Version of the Project Report
## Capítulo IV: Solution Software Design 
- 4.1. Strategic-Level Domain-Driven Design. 
	- 4.1.1. EventStorming. 
	- **Timelines:** Este gráfico de timelines representa la secuencia temporal de eventos y acciones clave relacionados con la gestión de cultivos, monitoreo, búsqueda de especialista en nuestra aplicación. Cada línea de tiempo corresponde a un aspecto específico de la gestión de cultivos y muestra cómo se desarrollan los eventos con el tiempo. Este diagrama nos ayuda a comprender la lógica temporal de la aplicación y cómo los eventos se relacionan entre sí para proporcionar una visión general de la gestión de cultivos.	
	![Timelines](https://cdn.discordapp.com/attachments/1149587894416183327/1149588737613889566/Eventstorming_2.jpg)
	- **Pivotal Points:** Este gráfico representa los Pivotal Points en el flujo de eventos de nuestro sistema de gestión de cultivos. Los Pivotal Points son momentos críticos en los cuales se producen cambios significativos o se toman decisiones clave que afectan la lógica y el comportamiento del sistema. Identificar y comprender estos puntos pivote es esencial para garantizar que nuestro software capture adecuadamente la complejidad y los requisitos críticos del negocio.	
	![Paint Points](https://cdn.discordapp.com/attachments/1149587894416183327/1149588075333296148/Eventstorming_1.jpg)
	- **Comands:** Este gráfico representa los comandos que los usuarios pueden emitir para interactuar con nuestro sistema de gestión de cultivos. Los comandos son acciones que los usuarios toman para lograr sus objetivos y modificar el estado del sistema. Identificar estos comandos es esencial para comprender cómo los usuarios interactúan con nuestra aplicación y qué acciones pueden realizar para gestionar sus cultivos de manera efectiva.	
	![Comands](https://cdn.discordapp.com/attachments/1149587894416183327/1149589014064660481/Eventstorming_3.jpg)
	- **Policies:** Este gráfico representa las políticas que dictan cómo el sistema de gestión de cultivos responde a eventos y acciones específicas. Las políticas son reglas o directrices que guían el comportamiento del sistema en situaciones diversas. Identificar y comprender estas políticas es esencial para asegurar que nuestro software funcione de acuerdo con las reglas de negocio y las expectativas de los usuarios.	
	![Policies](https://cdn.discordapp.com/attachments/1149587894416183327/1149589239965683782/Eventstorming_4.jpg)
	- **Read Models:** Este gráfico representa los modelos de lectura que permitirán a los usuarios acceder eficientemente a los datos relacionados con la gestión de cultivos en nuestro sistema. Los modelos de lectura son representaciones optimizadas de los datos que se utilizan para generar informes, consultas y visualizaciones. Identificar y definir estos modelos es esencial para garantizar que los usuarios puedan obtener la información que necesitan de manera rápida y precisa.
	![Read Models](https://cdn.discordapp.com/attachments/1149587894416183327/1149589444786139137/Eventstorming_5.jpg)
	- **External Systems:** Este gráfico representa la interacción planificada de nuestra aplicación con sistemas externos que son parte integral de nuestro ecosistema de gestión de cultivos. Los sistemas externos son componentes que se comunican con nuestra aplicación para intercambiar información y realizar acciones específicas. Identificar y comprender estas interacciones es crucial para garantizar que nuestro sistema sea capaz de integrarse efectivamente con otros sistemas y cumplir con los requisitos de negocio.
	![External Systems](https://cdn.discordapp.com/attachments/1149587894416183327/1149589665226170378/Eventstorming_6.jpg)
	- **Agregates:** Este gráfico representa los agregados y las entidades clave que desempeñan un papel fundamental en la gestión de cultivos de nuestro sistema. Los agregados son grupos lógicos de entidades y datos que tienen un significado coherente en el contexto del negocio. Identificar y definir estos agregados es esencial para diseñar una estructura de datos efectiva y garantizar que nuestra aplicación refleje adecuadamente la realidad del dominio agrícola.
	![Agregates](https://cdn.discordapp.com/attachments/1149587894416183327/1149589993363361792/Eventstorming_7.jpg)	
		- 4.1.1.1 Candidate Context Discovery.
 
   			Identificar candidatos de contexto implica descubrir áreas potenciales de enfoque en un sistema complejo. Esto implica analizar el sistema para identificar sus componentes esenciales y sus interacciones, agrupándolos en áreas lógicas para simplificar el proceso de diseño e implementación. El objetivo principal es mejorar la escalabilidad, el rendimiento y la facilidad de mantenimiento del sistema.
		![Candidates context](https://cdn.discordapp.com/attachments/1149587894416183327/1149589993363361792/Eventstorming_7.jpg)
		- 4.1.1.2 Domain Message Flows Modeling. 
		- 4.1.1.3 Bounded Context Canvases. 
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
	- **Bounded Context 7: Profile Management**
![Bounded Context 7](https://media.discordapp.net/attachments/912089666939916348/1149126633735848047/Bounded_Context_Canvas_by_Nick_Tune_1.jpg?width=1310&height=669)
	- **Bounded Context 8: Suscription and Payment**
![Bounded Context 8](https://media.discordapp.net/attachments/912089666939916348/1149126634570514513/Bounded_Context_Canvas_by_Nick_Tune_4.jpg?width=1353&height=669)
	- **Bounded Context 9: IOT Asset Management**
![Bounded Context 9](https://media.discordapp.net/attachments/912089666939916348/1149126634834771978/Bounded_Context_Canvas_by_Nick_Tune_5.jpg?width=1338&height=669)


- 4.1.2. Context Mapping. 
		
	El Context Mapping es una metodología empleada en el desarrollo de software para comprender y representar gráficamente las conexiones entre los usuarios, los conceptos y los equipos que forman parte de un proyecto.

	- 4.1.3. Software Architecture. 
		- 4.1.3.1. Software Architecture System Landscape Diagram. ![Landscape Diagram](https://media.discordapp.net/attachments/1143666758042013892/1149092447788486677/landscape.drawio.png?width=1025&height=405) 
		- 4.1.3.2. Software Architecture Context Level Diagrams. ![Context diagram](https://media.discordapp.net/attachments/1143666758042013892/1149089602737537094/Context.drawio.png?width=954&height=473)
		- 4.1.3.2. Software Architecture Container Level Diagrams. ![Container DIagram](https://media.discordapp.net/attachments/1143666758042013892/1149106586892111892/container.drawio.png?width=454&height=473)
		- 4.1.3.3. Software Architecture Deployment Diagrams. ![Deployment Diagram](https://media.discordapp.net/attachments/1149587894416183327/1149594351039684608/C4-Deployme.drawio_1.png?width=702&height=473) 

- **4.2. Tactical-Level Domain-Driven Design.**

	El Tactical-Level Domain-Driven Design es una metodología de diseño de software que se enfoca en la representación del dominio y la estructuración de objetos en niveles específicos, que abarcan desde la lógica empresarial hasta la aplicación y la infraestructura.
	- **4.2.1. Bounded Context: User Acount Manager**
		- **4.2.1.1. Domain Layer.** 
			- Nombre: User
			- Categoria: Entity
			- Propósito: Almacenar datos de nuestros usuarios
			- Atributos :

				| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
				|-----------|--------------|-------------|----------------------------------------------|
				| id        | int          | private     | Id de identidad                              |
				| suscripcionId        | int          | private     | Id del la suscripcion             |
				| firstName | string       | private     | Almacena el nombre del usuario               |
				| lastName  | string       | private     | Almacena el apellido del usuario             |
				| cellphone  | string       | private     | Almacena el número telefónico del usuario        |
				| email     | string       | private     | Almacena el email del usuario                |
				| password  | string       | private     | Almacena la contraseña de acceso del usuario |
				| userType  | UserType     | private     | Almacena el tipo de usuario                  |
			- Métodos:
				| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
				|--------------|--------------|-------------|-----------------------------------------------|
				| User         | void         | public      | Constructor de la identidad                   |
				| getFullName  | string       | public      | Obtiene el nombre completo del usuario        |
				| getType      | string       | public      | Retorna el tipo de usuario                    |

			- Nombre: UserType
			- Categorìa: Enum
			- Propòsito: Proveer los tipos de usuario
			- Atributos: 
				| Nombre       | Tipo de dato | Visibilidad |
				|--------------|--------------|-------------|
				| FARMER       | string       | public      |
				| SPECIALIST   | string       | public      |
				| ADM          | string       | public      |
			- Nombre: IUserRepository
			- Categoorìa: Repository
			- Propòsito: Persistir usuarios
		- **4.2.1.2 Interface layer**
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
		- **4.2.1.3 Application Layer**
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
			
			- Nombre: ModifyUser.handler
			- Categorìa: Handler
			- Propòsito: Handler para modificar un usuario
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| ModifyUser.handler | void         | public      | Constructor             |
				| execute  | void         | public      | Permite modificar datos del usuario |	

			- Nombre: ModifiUser.command
			- Categorìa: Command
			- Propòsito: Command para modificar un usuario
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| ModifyUser.command | void         | public      | Constructor          	|
			
			- Nombre: DeleteUser.handler
			- Categorìa: Handler
			- Propòsito: Handler para eliminar un usuario
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| DeleteUser.handler | void         | public      | Constructor             |
				| execute  | void         | public      | Permite elminar datos del usuario |	

			- Nombre: ModifiUser.command
			- Categorìa: Command
			- Propòsito: Command para modificar un usuario
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| DeleteUser.command | void         | public      | Constructor          	|
			
		- **4.2.1.4 Infrastructure Layer**
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
		- **4.2.1.5. Bounded Context Software Architecture Component Level Diagrams**
			El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes User](https://cdn.discordapp.com/attachments/1143666758042013890/1152020288670814288/image.png)
		- **4.2.1.6 Bounded Context Software Architecture Code Level Diagrams**
			Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código				
			- **4.2.1.6.1 Bounded Context Domain Layer Class Diagrams**
				Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
				![Diagrama clases User](https://cdn.discordapp.com/attachments/1143666758042013890/1152420088914391070/image.png)
			- **4.2.1.6.2 Bounded Context Database Diagrams**
				Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos. Este diagrama muestra la relación entre la tabla Shipments y la tabla Comments.
	- **4.2.2. Bounded Context: Plant Management**
		- **4.2.2.1. Domain Layer.** 
			- Nombre: Plant
			- Categoria: Entity
			- Propósito: Almacenar datos de las plantas
			- Atributos :

				| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
				|-----------|--------------|-------------|----------------------------------------------|
				| id | int       | private     | Id de identidad               |
				| plantName        | string          | private     | Nombre de la planta                         |
				| plantDescription        | string          | private     | Descripción de la planta         |

			- Métodos:
				| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
				|--------------|--------------|-------------|-----------------------------------------------|
				| Plant       | void         | public      | Constructor de la identidad                   |
				| getPlantName  | string       | public      | Obtiene el nombre de la planta       |
				| getDescription      | string       | public      | Retorna la desripción                 |

		
			- Nombre: IPlantRepository
			- Categoría: Repository
			- Propósito: Persistir las plantas
			- Métodos: 
				| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
				|--------------|--------------|-------------|-----------------------------------------------|
				| IPlantRepository       | ISuscriptionRepository         | public      | Constructor de la identidad                   |
				| add  | void       | public      | Crear una planta      |
				| updatePlant     | void       | public      |Permite actualizar los datos de una planta|
				|deletePlant|void|public|Permite eliminar una planta|
				| ListPlants|array|public|Devuelve una lista de todas las plantas|
				|FindByName|promise<PlantResource>|public|Devuelve una planta por el nombre|
				|FindById|promise<PlantResource|publicDevuelve una planta por el Id|
		

		- **4.2.2.2 Interface layer**
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

		- **4.2.2.3 Application Layer**
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
			
			
		- **4.2.2.4 Infrastructure Layer**
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
				
		- **4.2.2.5. Bounded Context Software Architecture Component Level Diagrams**
			El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes sUSCRIPTION](https://cdn.discordapp.com/attachments/1143666758042013890/1152477663966011422/image.png)
		- **4.2.2.6 Bounded Context Software Architecture Code Level Diagrams**
			Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código				
			- **4.2.2.6.1 Bounded Context Domain Layer Class Diagrams**
				Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
				![Diagrama clases Suscription](https://cdn.discordapp.com/attachments/1143666758042013890/1152481306656120885/image.png)
			- **4.2.2.6.2 Bounded Context Database Diagrams**
				Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos. Este diagrama muestra la relación entre la tabla Shipments y la tabla Comments.

	- **4.2.3. Bounded Context: Suscription Management**
		- **4.2.2.1. Plan.** 
			- Nombre: Plan
			- Categoria: Value Object
			- Propósito: Almacenar datos de los planes del servicio
			- Atributos :

				| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
				|-----------|--------------|-------------|----------------------------------------------|
				| planType | PlanType       | private     | Almacena el tipo de plan               |
				| costoMes        | double          | private     | Costo del plan                          |

			- Métodos:
				| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
				|--------------|--------------|-------------|-----------------------------------------------|
				| Plan       | void         | public      | Constructor de la identidad                   |
				| getType  | string       | public      | Obtiene el tipo de plan       |
				| getCosto      | double       | public      | Retorna el costo del plan                 |

			- Nombre: PlanType
			- Categorìa: Enum
			- Propòsito: Proveer los tipos de planes
			- Atributos: 
				| Nombre       | Tipo de dato | Visibilidad |
				|--------------|--------------|-------------|
				| FREE       | string       | public      |
				| MONTHLY   | string       | public      |
				| ANUAL          | string       | public      |
			
			- Nombre: Suscription
			- Categoría: Entity
			- Proósito: Almacenar los datos de la suscripción del usuario
			- Atributos: 
				| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
				|-----------|--------------|-------------|----------------------------------------------|
				| id        | int          | private     | Id de identidad                              |
				| planId | int       | private     | Almacena el Id del plan               |
				| dayPay      | date        | private     |    Día de pago                       |
			- Métodos:
				| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
				|-----------|--------------|-------------|----------------------------------------------|
				| Suscription       | Suscription       | public     | Constructor de clase                   |
				| getPlanId | int       | public     | Devuelve el tipo de plan               |
				| getDayPay      | date        | public     |    Devuelve el dia de pago                      |
			- Métodos:
			- Nombre: ISuscriptionRepository
			- Categoría: Repository
			- Propósito: Persistir las suscripciones
			- Métodos: 
				| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
				|--------------|--------------|-------------|-----------------------------------------------|
				| ISuscriptionRepository       | ISuscriptionRepository         | public      | Constructor de la identidad                   |
				| add  | void       | public      | Crear una suscripción      |
				| updateDayPay      | void       | public      | Permite actualizar la fecha de pago de la suscripción                |
				| updatePlan|Plan|public|Permite actualizar el tipo de plan de la suscripción|
				|	deletePlan|void|public|Permite eliminar planes|
		

		- **4.2.1.2 Interface layer**
			- Nombre: Suscription.controller
			- Categorìa: Controller
			- Propòsito: Controlar registro de suscripciones
			- Mètodos:
				| Nombre     | Tipo de dato | Visibilidad | Descripción                             |
				|------------|--------------|-------------|-----------------------------------------|
				| Register   | Promise      | public      | Registra un nuevo plan               |
				| ModifyPayDay | Promise      | public      | Permite modificar los datos del usuario |
				|ModifyPlan|Promise|public|Permite modificar el plan|
				| DeleteSuscription | Promise      | public      | Permite eliminar una suscripción             |
		- **4.2.1.3 Application Layer**
			- Nombre: AssignSuscription.handler
			- Categorìa: Handler
			- Propòsito: Handler para asignar una suscripcion
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| AssignSuscription.handler | void         | public      | Constructor             |
				| execute  | void         | public      | Permite registrar al usuario |	

			- Nombre: AssignSuscription.command
			- Categorìa: Command
			- Propòsito: Command para asignar una suscripción
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| AssignSuscriptionr.command | void         | public      | Constructor          	|

			
			
		- **4.2.1.4 Infrastructure Layer**
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
				
		- **4.2.1.5. Bounded Context Software Architecture Component Level Diagrams**
			El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes sUSCRIPTION](https://cdn.discordapp.com/attachments/1143666758042013890/1152477663966011422/image.png)
		- **4.2.1.6 Bounded Context Software Architecture Code Level Diagrams**
			Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código				
			- **4.2.1.6.1 Bounded Context Domain Layer Class Diagrams**
				Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
				![Diagrama clases Suscription](https://cdn.discordapp.com/attachments/1143666758042013890/1152481306656120885/image.png)
			- **4.2.1.6.2 Bounded Context Database Diagrams**
				Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos. Este diagrama muestra la relación entre la tabla Shipments y la tabla Comments.
		
	- **4.2.4. Bounded Context: Crop Management**
		- **4.2.2.1. Crop.** 
			- Nombre: Crop
			- Categoria: Entity
			- Propósito: Almacenar los datos de los cultivos
			- Atributos :

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
				| ModifyLastUpdate|void|private|Modifica la última fecha de actualización|

			- Nombre: Report
			- Categoría: Entity
			- Propósito: Almacenar los reportes de los cultivos
			- Atributos:
				| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
				|-----------|--------------|-------------|----------------------------------------------|
				| Id | int       | private     | Id de identidad               |
				| createAt|date|private|Fecha de creacion|
				| imageSrc|string|private|Enlace a la imagen del cultivo al momento de crear el reporte|
				|Description|string|private|Descripción de como se encuentra el cultivo al momento de generar el reporte|
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


		- **4.2.4.2 Interface layer**
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
		- **4.2.1.3 Application Layer**
			- Nombre: RegisterCrop.handler
			- Categorìa: Handler
			- Propòsito: Handler para registrar un cultivo
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| RegisterCrop.handler | void         | public      | Constructor             |
				| execute  | void         | public      | Permite registrar un cultivo |	

			- Nombre: RegisterCrop.command
			- Categorìa: Command
			- Propòsito: Command para asignar una suscripción
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| RegisterCrop.command | void         | public      | Constructor          	|


			- Nombre: AddReport.handler
			- Categorìa: Handler
			- Propòsito: Handler para registrar un reporte de cultivo
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| AddReport.handler | void         | public      | Constructor             |
				| execute  | void         | public      | Permite registrar un cultivo |	

			- Nombre: AddReport.command
			- Categorìa: Command
			- Propòsito: Command para asignar una suscripción
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| AddReport.command | void         | public      | Constructor          	|

			- Nombre: ActivateMonitoring.handler
			- Categorìa: Handler
			- Propòsito: Handler para activar el monitoreo de un cultivo
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| ActivateMonitoring.handler | void         | public      | Constructor     |
				| execute  | void         | public      | Permite activar el monitoreo |	

			- Nombre: ActivateMonitoring.command
			- Categorìa: Command
			- Propòsito: Command para activar el monitoreo de un cultivo
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| ActivateMonitoring.command | void         | public      | Constructor      |
			
			- Nombre: DisplayInformation.handler
			- Categorìa: Handler
			- Propòsito: Handler para mostrar la información del cultivo en tiempo real
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| DisplayInformation.handler | void         | public      | Constructor     |
				| execute  | void         | public      | Permite mostrar información en tiempo real |	

			- Nombre: DisplayInformation.command
			- Categorìa: Command
			- Propòsito: Command para mostrar la información del cultivo en tiempo real
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| DisplayInformation.command | void         | public      | Constructor      |
			
			- Nombre: DeleteCrop.handler
			- Categorìa: Handler
			- Propòsito: Handler para eliminar un cultivo
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| DeleteCrop.handler | void         | public      | Constructor     |
				| execute  | void         | public      | Permite mostrar información en tiempo real |	

			- Nombre: DeleteCrop.command
			- Categorìa: Command
			- Propòsito: Command para mostrar la información del cultivo en tiempo real
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| DeleteCrop.command | void         | public      | Constructor      |

			
		- **4.2.1.4 Infrastructure Layer**
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
				
		- **4.2.1.5. Bounded Context Software Architecture Component Level Diagrams**
			El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes sUSCRIPTION](https://cdn.discordapp.com/attachments/1143666758042013890/1152477663966011422/image.png)
		- **4.2.1.6 Bounded Context Software Architecture Code Level Diagrams**
			Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código				
			- **4.2.1.6.1 Bounded Context Domain Layer Class Diagrams**
				Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
				![Diagrama clases Suscription](https://cdn.discordapp.com/attachments/1143666758042013890/1152481306656120885/image.png)
			- **4.2.1.6.2 Bounded Context Database Diagrams**
				Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos. Este diagrama muestra la relación entre la tabla Shipments y la tabla Comments.

	- **4.2.4. Bounded Context: Project Management**
		- **4.2.4.1. Domain Layer.** 
			- Nombre: Project
			- Categoria: Entity
			- Propósito: Almacenar los datos de los proyectos
			- Atributos :

				| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
				|-----------|--------------|-------------|----------------------------------------------|
				| Id | int       | private     | Id de identidad               |
				| cropId        | int          | private     | Id del cultivo asignado         |
				|createAt|date|private|Fecha de creación|
				|updateAt|date|private|Última fecha de actualización|
				
			- Métodos:
				| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
				|--------------|--------------|-------------|-----------------------------------------------|
				| Plan       | Crop         | public      | Constructor de la identidad                   |
				| update  | void       | public      | Actualiza el plan       |
			
			- Nombre: Step
			- Categoría: Entity
			- Propósito: Almacenar los pasos de un proyecto
			- Atributos:
				| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
				|-----------|--------------|-------------|----------------------------------------------|
				| Id | int       | private     | Id de identidad               |
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
		
		- **4.2.4.2 Interface layer**
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

		- **4.2.4.3 Application Layer**
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

			
		- **4.2.4.4 Infrastructure Layer**
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

				
		- **4.2.1.5. Bounded Context Software Architecture Component Level Diagrams**
			El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes sUSCRIPTION](https://cdn.discordapp.com/attachments/1143666758042013890/1152477663966011422/image.png)
		- **4.2.1.6 Bounded Context Software Architecture Code Level Diagrams**
			Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código				
			- **4.2.1.6.1 Bounded Context Domain Layer Class Diagrams**
				Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
				![Diagrama clases Suscription](https://cdn.discordapp.com/attachments/1143666758042013890/1152481306656120885/image.png)
			- **4.2.1.6.2 Bounded Context Database Diagrams**
				Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos. Este diagrama muestra la relación entre la tabla Shipments y la tabla Comments.
	- **4.2.4. Bounded Context: Notification**
		- **4.2.4.1. Domain Layer.** 
			- Nombre: Notification
			- Categoria: Entity
			- Propósito: Almacenar los datos de las notificaciones
			- Atributos :

				| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
				|-----------|--------------|-------------|----------------------------------------------|
				| Id | int       | private     | Id de identidad               |
				| userId        | int          | private     | Id del usuario         |
				|createAt|date|private|Fecha de creación|
				|importance|NotificationImportane|private|Importancia de la notificación|
				|title|string|private|Título de la notificación|
				|body|string|private|Cuerpo de la notificación|
				
			- Métodos:
				| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
				|--------------|--------------|-------------|-----------------------------------------------|
				| Notification       | Constructor        | public      | Constructor de la identidad                   |
				| getTitle  | string   | public      | Obtiene el titulo de la notificacion |
				|getBody|string|public|Obtiene el cuerpo de la notificación|
			
			- Nombre: NotificationImportance
			- Categoría: Entity
			- Propósito: Almacenar los pasos de un proyecto
			- Atributos:
				| Nombre    | Tipo de dato | Visibilidad | Descripción                                  |
				|-----------|--------------|-------------|----------------------------------------------|
				| Id | int       | private     | Id de identidad               |
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
		
		- **4.2.4.2 Interface layer**
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

		- **4.2.4.3 Application Layer**
			- Nombre: NotificationSendeed.event-handler
			- Categorìa: Event Handler
			- Propòsito: Gestionar el envío de una notificación
			- Mètodos: 
				| Nombre   | Tipo de dato | Visibilidad | Descripción                       |
				|----------|--------------|-------------|-----------------------------------|
				| handle | void         | public      | Constructor             |


			
		- **4.2.4.4 Infrastructure Layer**
			- Nombre: NotificationRepository
			- Categoría: Repository
			- Propósito: Persistir las notificaciones
			- Métodos: 
				| Nombre       | Tipo de dato | Visibilidad | Descripción                                   |
				|--------------|--------------|-------------|-----------------------------------------------|
				| NotificationRepository       | CropRepository         | public      | Constructor de la identidad |
				| add  | void       | public      | Crear una notificación     |
				| DeleteProyect|void|public|Permite eliminar un proyecto|

				
		- **4.2.1.5. Bounded Context Software Architecture Component Level Diagrams**
			El diagrama de componentes C4 nos permite visualizar como se estructura un sistema basàndonos en sus componentesy relaciones. Los componentes son representados por bloques y las relaciones mediante flechas. ![Diagrama de componentes sUSCRIPTION](https://cdn.discordapp.com/attachments/1143666758042013890/1152477663966011422/image.png)
		- **4.2.1.6 Bounded Context Software Architecture Code Level Diagrams**
			Los diagramas de nivel de código en la arquitectura de software son una herramienta de representación utilizada para mostrar la estructura interna de un sistema de software con un alto grado de detalle, abarcando clases, métodos y sus interconexiones. Estos esquemas resultan beneficiosos para adquirir una comprensión de cómo se vinculan las diversas componentes de un sistema de software y cómo se lleva a cabo la implementación de las funciones a nivel de código				
			- **4.2.1.6.1 Bounded Context Domain Layer Class Diagrams**
				Los diagramas de estratificación de dominio facilitan la representación visual de la disposición de las capas dentro de la arquitectura de software en el ámbito del negocio. Cada capa de dominio se ilustra como un bloque, y las conexiones entre estas capas se indican mediante flechas o líneas.
				![Diagrama clases Suscription](https://cdn.discordapp.com/attachments/1143666758042013890/1152481306656120885/image.png)
			- **4.2.1.6.2 Bounded Context Database Diagrams**
				Un diagrama de base de datos es una representación visual de la estructura de una base de datos. Son útiles para entender la estructura de una base de datos y para visualizar cómo se relacionan las diferentes tablas de una base de datos. Este diagrama muestra la relación entre la tabla Shipments y la tabla Comments.		
