# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration

**Software Documentation and Project Management:**
- **Github:** Plataforma de control de versiones que facilitará la colaboración y revisión de cambios de cada miembro del equipo. Ruta de referencia: https://github.com/

**Requirements Management:**

- **Trello:** Herramienta utilizada para gestionar el flujo de trabajo de proyectos principalmente basados en marcos de trabajos ágiles. Será empleado para visualizar y actualizar el estado actual de las tareas e historias de usuario pertenecientes al sprint a desarrollar. Ruta de referencia: https://trello.com/es

**Product UX/UI Design:**

- **Figma:** Plataforma de elaboración de diseño de interfaces y elaboración de prototipos interactivos para las versiones de Landing Page, Desktop y Mobile Web Application. Ruta de referencia: https://www.figma.com/login

- **UX Pressia:** Diseño de User Personas, Empathy Maps, Journey Maps e Impact Mapping. Ruta de referencia: https://uxpressia.com/

- **Miro:** Empleado para el diseño de los As-Is y To-Be Scenario Maps. Ruta de referencia: 

- **Lucidchart:** Aplicación para diagramar flujos. Empleado para el diseño de Wireflows, User-Flows y el Diagrama de
  Clases asociado a la aplicación. Ruta de referencia: https://www.lucidchart.com/pages/es

- **Structurizr DSL:** Empleado para la creación de diagramas de software, utilizando el modelo C4. Ruta de referencia: https://structurizr.com/

**Software Development:**

- **Visual Studio Code:** Entorno de desarrollo integrado elegido para la elaboración de la Landing Page: https://code.visualstudio.com/
  
- **HTML:** Lenguaje de etiquetado para páginas web. Será empleado para el desarrollo de la presentación de la landing Page. Ruta de referencia: https://www.w3schools.com/html/html5_syntax.asp 
  
- **CSS:** Tecnología para dar estilo a las páginas web, permitiendo el diseño visual. Ruta de referencia: https://google.github.io/styleguide/htmlcssguide.html
  
- **JavaScript:** Lenguaje de programación orientado a objetos utilizado para implementar funcionalidades en la Landing Page. Ruta de referencia: https://developer.mozilla.org/es/docs/Web/JavaScript

**Software Deployment:**

- **Github Pages:** Plataforma que facilita el despliegue sencillo de páginas web directamente desde repositorios de GitHub. Ruta de referencia: https://pages.github.com/

### 5.1.2. Source Code Management

**Repositorio de Github:** https://github.com/GrupoLatex-SI0729-2510-4334/Final-Report

**Repositorio de Landing Page:** https://grupolatex-si0729-2510-4334.github.io/Landing-Page/

Para nuestra estrategia de gestión de versiones con Git, nos hemos inspirado en el artículo "A successful Git branching model" de Vincent Driessen, adoptando el modelo de ramificación GitFlow. Este enfoque nos permite establecer claramente las convenciones de ramificación que aplicaremos en nuestro proyecto.

**Flujo de trabajo GitFlow:**

<img src="/assets/FlujoDeTrabajo_Gitflow.png">

**Estructura de Ramas (Branches):**

- **Main branch (Rama principal):** Rama base del proyecto donde se almacenan las versiones estables y listas para producción. Solo se integran cambios que hayan sido debidamente revisados y validados en otras ramas.

- **Develop branch (Rama de desarrollo):** Rama que sirve como espacio de trabajo colaborativo donde se integran las actualizaciones y cambios realizados por el equipo. Aquí se mantiene el código en constante evolución antes de ser lanzadas.

- **Release branches (Ramas de lanzamiento):** Se utilizan para facilitar la preparación de nuevas versiones del producto. Estas ramas parten de develop y permiten realizar ajustes finales. Las versiones se nombran siguiendo el esquema de versionado semántico (Semantic Versioning 2.0.0): release/vX.Y.Z.

- **Feature branches (Ramas de funcionalidad):** Se utiliza para desarollar nuevas funcionalidades o mejoras específicas en su propia rama independiente, separada de la rama principal de desarrollo. Una vez completada, se integrará a develop. Estas ramas seguirán una convención de nombres del tipo: feature/nombre-de-la-funcionalidad.

- **Hotfix branches (Ramas de corrección):** Creadas para resolver errores urgentes detectados que pueden afectar en la experiencia de usuario. Permiten la implementación de soluciones rápidas directamente sobre la rama principal. Se sigue la siguiente nomenclatura: hotfix/nombre-del-problema.

**Versionamiento Semántico:** 
<br>Para nombrar las Releases, se aplicará el sistema de versionamiento semántico (Semantic Versioning 2.0.0), donde:
- **X:** Versión principal, se incrementa cuando se realizan cambios significativos en la funcionalidad del software que podrían afectar su estructura.
- **Y:** Versión secundaria, se ajusta para la adición o eliminación de características sin modificar la estructura principal del software.
- **Z:** Versión de parche, se usa para pequeñas correcciones y mejoras que no afectan la funcionalidad principal.

**Convenciones de Commits:** 
<br>Para los mensajes de los commits realizados, se utilizará la especificación Conventional Commits basada en Angular Commit Guidelines. La estructura a seguir será la siguiente:
<br> `git commit -m "<type>[optional scope]:<title>" -m"<description">`

### 5.1.3. Source Code Style Guide & Coding Conventions
Para el correcto uso de lenguajes de programación, se adaptarán buenas prácticas respecto a las convenciones estándares para coding que garantizarán el correcto desarrollo de la solución.

**HTML:**

- A pesar que HTML permite mezclar letras mayúsculas y minúsculas en los nombres de los elementos, se recomienda usar nombres de elementos en minúsculas.
- Todos los elementos deben estar correctamente cerrados.
  <br> `<p>This is a paragraph.</p>`
- Los nombres de etiquetas y atributos deben ir en minúscula.
  <br> `href`
- Se recomienda entrecomillar los valores de los atributos.
  <br> `<table class="striped">`

**CSS:**

- Los nombres de clases deben seguir la convención kebab-case. Ejemplo: `.ads-sample`
- Los selectores deben ser claros y específicos.
- Se debe mantener una estructura ordenada con propiedades agrupadas por tipo (layout, tipografía, colores, etc.).
- Se recomienda separar los selectores y declaraciones en líneas independientes.

**Gherkin:**

- Los escenarios deben escribirse en lenguaje natural estructurado: Given, When, Then.
- Los nombres de los escenarios deben ser claros, concisos y expresivos del comportamiento esperado.
- Se deben evitar detalles técnicos en las descripciones.
- La escritura debe orientarse a la colaboración entre roles técnicos y no técnicos.

**Angular:**

- Convenciones de estructura de archivos `hero.component.ts|html|css|spec`
- Aplicar el método Principio de responsabilidad única (SRP)a todos los componentes, servicios y otros símbolos, garantiza que la aplicación sea más limpia, más fácil de leer y mantener, y más comprobable.
- Se deben separar los nombres de archivos con puntos y guiones.
- La nomenclatura de servicios debe estar acopmañado del sufijo: `.service.ts`

**Java:**

- Nombres de clases en PascalCase `UserService`.
- Métodos y atributos en camelCase `getUserData()`.
- Uso de anotaciones como `@RestController`, `@Service`, `@Repository` para definir roles.
- Estructura clara del proyecto basada en paquetes por capas.
  
**JavaScript:**

- Los nombres de clases deben escribirse usando camelCase. Suelen ser sustantivos o frases nominales. Ejemplo: `Character`
- Los nombres de funciones y variables deben seguir lowerCamelCase. Suelen ser verbos o frases verbales. Ejemplo: `sendMessage`
- Cada declaración de variable (de campo o local) declara solo una variable. Ejemplo: `int a`

**TypeScript:**

- Los literales de cadena ordinarios se delimitan con comillas simples ('').
- Organización del código en módulos y componentes reutilizables.
- Los nombres de clases deben seguir PascalCase y los métodos camelCase.
- Se pueden crear instancias de errores mediante `throw new Error('')`.

**Spring Boot:**

- Definición de componentes siguiendo los principios de Spring: `@RestController`, `@Service`, `@Repository`, `@Entity`.
- Aplicar la convención de configuración mínima: principios de "convention over configuration".
- Organización de proyectos en módulos claramente separados (API, Services, Repository, Config).

### 5.2. Landing Page, Services & Applications Implementation
#### 5.2.1. Sprint 1
##### 5.2.1.1. Sprint Planning 1

| **Sprint #**                      | **Sprint 1**                                                                 |
|----------------------------------|------------------------------------------------------------------------------|
| **Sprint Planning Background**   |                                                                              |
| **Date**                         | 19/04/2025                                                                   |
| **Time**                         | 09:00 PM                                                                     |
| **Location**                     | Servidor de Discord del Equipo                                               |
| **Prepared By**                  | Diego Cabrera                                                             |
| **Attendees (to planning meeting)** | Diego Cabrera / Andrea Santur / Alessandra Becerra / Joaquin Pedraza / Pedro Nanfuñay |
| **Sprint 1 Review Summary**      |   En este sprint, el equipo se enfocó en establecer la base del proyecto: se creó, diseñó y lanzó la primera versión operativa de la landing page, incorporando elementos esenciales como la descripción del servicio, los planes de suscripción, formularios de contacto y soporte multilenguaje. Además, se realizaron tareas de UX, como la elaboración de User Personas, Journey Maps y la definición de la arquitectura de información.     |
| **Sprint 1 Retrospective Summary** |      Los miembros del equipo señalaron que la colaboración y el trabajo en conjunto fueron efectivos. Resaltaron logros en la integración de herramientas como UXPressia, Figma y en el diseño responsivo. Como oportunidad de mejora, se propuso optimizar la gestión del tiempo en las subtareas y definir criterios de aceptación más claros desde el comienzo.   |
| **Sprint Goal & User Stories**   |        Finalizar la etapa de descubrimiento e investigación, validación de usuarios, análisis de la competencia, diseño de la arquitectura de la información y la estructura básica de la landing.      |
| **Sprint 1 Goal**                |   El objetivo fue crear una landing page completa y alineada con la visión del proyecto “TocaAquí”, garantizando que fuera funcional, responsiva, accesible y visualmente atractiva para artistas y locales. Además, este sprint estableció las bases para la experiencia de usuario, con entregables como User Personas, Empathy Maps, Wireframes y Style Guides.       |
| **Sprint 1 Velocity**            | 4 Velocity                                                                   |
| **Sum of Story Points**          | 6 Story Points                                                               |

##### 5.2.1.2. Aspect Leaders and Collaborators

| Team Member              | GitHub Username     | Landing Page | Diseño UI/UX | HTML/CSS | JavaScript | Documentación |
|--------------------------|---------------------|--------------|---------------|----------|-------------|----------------|
| Andrea Santur           | andreli-star        | C            | C             | C        | L           | C              |
| Diego Cabrera           | OscarAntayhuaCastillo | L            | C             | C        | C           | L              |
| Alessandra Becerra           | aleeBecerra        | C            | C             | L        | C           | C              |
| Joaquin Pedraza            | JoaquinPedraza1             | C            | C             | C        | L           | C              |
| Pedro Nanfuñay          | PedroJ18        | C            | L             | C        | C           | C              |

##### 5.2.1.3. Sprint Backlog 1

| **User Story Id** | **User Story Title** | **Work-Item/Task Id** | **Work-Item/Task Title** | **Description** | **Estimation** | **Assigned To** | **Status** |
|:-----------------:|:--------------------:|:---------------------:|:-----------------------:|:---------------:|:--------------:|:--------------:|:----------:|
| US01 | Visualización clara del propósito de la plataforma	 | T01 | Diseño general de la landing page | Creación y redacción del propósito de nuestra plataforma | 5h | Diego Cabrera | Done |
| US02 | Visualización de planes para artistas y locales | T02 | Visualización de las subscripciones | Creación de los planes de pago de TocaAquí | 3h | Andrea Santur | Done |
| US03 | Visualización del equipo de desarrollo en la landing | T03 | Redacción de la sección de "Sobre Nosotros" | Creación de la sección de presentación del equipo | 2h | Joaquin Pedraza | Done |
| US04 | 	Acceso rápido a registro desde botones CTA | T04 | Presentación del formulario | Creación del formulario a ser rellenado por el artista o por el promotor | 3h | Alessandra Becerra | Done |

### 5.3 Validation Interviews
#### 5.3.1 Diseño de entrevistas

**Objetivo de la entrevista:**

Validar la usabilidad y efectividad de la landing page de TocaAquí y de los flujos de usuario (user flows) asegurando que cada flujo sea intuitivo, claro y funcional para los usuarios y su interaccion con la plataforma.

**Segmento: Músicos Independientes**

**Objetivo:Evaluar si el diseño, el flujo de registro, las herramientas de gestión musical y la claridad en la propuesta de valor ayudan al músico a comprender y usar la plataforma eficientemente..**
-*Explicación de los alcances de la demostración*
- Landing Page
- *Prinipales tareas en la aplicación*

-*Navegacion a través de la plataforma web*
-*Flujos de usuario (user flows):*
1. El usuario ingresa a landing page 
2. Registro y creación de perfil musical.
3. Visualización de fechas disponibles y postulación a eventos.
4. Firma de contratos digitales y gestión de pagos mediante escrow.
5. Gestión logística del evento desde su cuenta.
6. Revisión de evaluaciones post-evento.

-*Formato de Registro de la Entrevista*
*Datos del Entrevistado:
- Nombre y apellidos
- Edad
- Ciudad de residencia
- Dispositivo utilizado (laptop)

-*Preguntas principales:* <br>
- ¿Qué te pareció la apariencia general de la landing page de TocaAquí? ¿Te transmitió confianza y profesionalismo como músico independiente?

- ¿Captaste rápidamente la propuesta de valor de TocaAquí? ¿Te quedó claro desde el inicio cómo puede ayudarte a conseguir más presentaciones?

- ¿La plataforma te permite visualizar fácilmente fechas disponibles para tocar? ¿Sientes que podrías gestionar tus shows sin complicaciones?

- ¿La sección 'Sobre Nosotros' y el equipo de desarrollo te generaron confianza para unirte a la comunidad?

- ¿Qué opinas de los planes que se ofrecen? ¿Notas diferencias claras entre el Básico, Medio y Premium?

- ¿Te gustaría ver ejemplos reales de bandas o solistas que ya usaron TocaAquí para cerrar presentaciones?

- ¿Te sentiste motivado a registrarte en la plataforma después de leer la landing page? ¿Qué te animaría aún más a hacerlo?

**Segmento: Promotores**

**Objetivo: Determinar si los promotores encuentran la plataforma útil y eficiente para publicar eventos, recibir postulaciones, gestionar aspectos técnicos y tomar decisiones informadas sobre artistas..**

-*Explicación de los alcances de la demostración*
- Landing Page
-  Prinipales tareas en la aplicación

-*Navegacion a través de la plataforma web*
-*Flujos de usuario (user flows):*
1. El usuario ingresa a landing page 
2. Registro y configuración de perfil como promotor.
3. Publicación de fechas disponibles para eventos.
4. Revisión y selección de postulaciones de artistas.
5.Validación de requerimientos técnicos de los artistas.
6. Evaluación de artistas post-evento.
-*Formato de Registro de la Entrevista*
-*Datos del Entrevistado:*

- Nombre y apellidos
- Edad
- Ciudad de residencia
- Dispositivo utilizado (smartphone, tablet, laptop)

-*Preguntas principales:* <br>
- ¿La Landing Page de TocaAquí transmite confianza para que un promotor como tú publique sus eventos? ¿Qué mejorarías?

- ¿La navegación de la plataforma te pareció intuitiva para iniciar la publicación de un nuevo evento?

- ¿El flujo de publicación de eventos incluye toda la información que tú necesitas detallar (rider técnico, condiciones, ubicación)?

- ¿Te resultó útil y funcional la parte donde validas los requerimientos técnicos de cada artista?

- ¿Qué opinas del sistema de contratos digitales y pagos protegidos? ¿Te genera confianza para cerrar acuerdos?

- ¿La interfaz te permite visualizar bien el estado de tus eventos y las gestiones logísticas en curso?

- ¿Qué aspecto de la plataforma crees que podría hacerle mejoras para los próximos eventos?

### 5.3.2. Registro de Entrevistas.
  
A continuación presentamos los resultados de las entrevistas de validación realizadas a los musicos independientes y promotores, nuestros segmentos objetivos.

### Segmento : Músicos Independientes
**Entrevista 1**    
<table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th><strong>Dato</strong></th>
      <th><strong>Información</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Nombre completo</td><td>Alexander Gabriel Montoya Torres</td></tr>
    <tr><td>Edad</td><td>19 años</td></tr>
    <tr><td>Distrito</td><td>San Miguel</td></tr>
    <tr><td>Inicio de la entrevista</td><td>00:00</td></tr>
    <tr><td>Duración de la entrevista</td><td>06:40</td></tr>
    <tr><td>Foto captura</td><td><img src="/assets/AlexanderValidacion.png" alt="Alexander captura"></td></tr>
    <tr><td>Visualización de la Landing Page</td><td>Le gustó mucho el diseño general, resaltando los colores negro, amarillo y blanco. Considera que transmite confianza y profesionalismo. La información está organizada de forma clara y entendible.</td></tr>
    <tr><td>Exploración de funcionalidades clave</td><td>Considera práctico el calendario de fechas para organizar presentaciones y valora la facilidad de comunicación con promotores. Sugiere mostrar ejemplos de bandas que ya usaron la plataforma.</td></tr>
    <tr><td>Flujos de registro y navegación inicial</td><td>Positiva. Se siente motivado a registrarse. Sugiere mejorar el perfil de usuario agregando más detalles para hacerlo más completo.</td></tr>
    <tr><td>Publicación de eventos y postulación</td><td>Valoró la funcionalidad de la agenda de shows y la posibilidad de gestionar fechas y logística de forma sencilla.</td></tr>
    <tr><td>Planes y diferencias de servicios</td><td>Entiende las diferencias entre los planes, pero sugiere que funcionalidades como escrow automático y automatización logística también estén en el plan medio.</td></tr>
  </tbody>
</table>
[URL de la entrevista](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202310988_upc_edu_pe/ESDM8thHRehIhtIRW0xccVkBOmuRNRItcUYWGiqwzNCL4Q?e=76Uw2x)

**Entrevista 2**
<table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th><strong>Dato</strong></th>
      <th><strong>Información</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Nombre completo</td><td>Bryan Dennis Huamán Salas</td></tr>
    <tr><td>Edad</td><td>20 años</td></tr>
    <tr><td>Distrito</td><td>Surco</td></tr>
    <tr><td>Inicio de la entrevista</td><td>06:40</td></tr>
    <tr><td>Duración de la entrevista</td><td>06:00</td></tr>
    <tr><td>Foto captura</td><td><img src="/assets/BryanValidacion.png" alt="Bryan captura"></td></tr>
    <tr><td>Visualización de la Landing Page</td><td>La apariencia le transmitió confianza y profesionalismo, pero comentó que el fondo dificultaba la lectura por el exceso de brillo. Sugiere ajustar el color o contraste.</td></tr>
    <tr><td>Exploración de funcionalidades clave</td><td>Percibe que la plataforma ofrece opciones interesantes como contacto con locales y fechas disponibles, aunque desea ver más herramientas visuales asociadas a la música.</td></tr>
    <tr><td>Flujos de registro y navegación inicial</td><td>Entendió bien los accesos iniciales y considera que podría gestionar sus shows sin mayores complicaciones.</td></tr>
    <tr><td>Publicación de eventos y postulación</td><td>Aprecia que haya formas claras de contacto y postulación, aunque no profundizó mucho en esta parte inicial.</td></tr>
    <tr><td>Planes y diferencias de servicios</td><td>Entiende las diferencias entre Básico, Medio y Premium, pero sugiere agregar más beneficios para hacerlo más atractivo.</td></tr>
  </tbody>
</table>
[URL de la entrevista](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202310988_upc_edu_pe/ESDM8thHRehIhtIRW0xccVkBOmuRNRItcUYWGiqwzNCL4Q?e=76Uw2x)

**Entrevista 3**
<table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th><strong>Dato</strong></th>
      <th><strong>Información</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Nombre completo</td><td>Benjamín Peraltilla Herrera </td></tr>
    <tr><td>Edad</td><td>18 años</td></tr>
    <tr><td>Distrito</td><td>Breña</td></tr>
    <tr><td>Inicio de la entrevista</td><td>00:00</td></tr>
    <tr><td>Duración de la entrevista</td><td>06:40</td></tr>
    <tr><td>Foto captura</td><td><img src="/assets/BenjaminValidacion.png" alt="Benjamín captura"></td></tr>
    <tr><td>Visualización de la Landing Page</td><td>La landing page le pareció llamativa, especialmente por el uso de colores, y le transmitió confianza y profesionalismo.</td></tr>
    <tr><td>Exploración de funcionalidades clave</td><td>Entendió rápidamente la propuesta de valor: músicos se presentan y promotores los descubren de manera clara y directa.</td></tr>
    <tr><td>Flujos de registro y navegación inicial</td><td>Se mostró motivado a registrarse tras explorar la landing page. Consideró que la sección "Sobre nosotros" y ver los desarrolladores aumentó su confianza. Sugiere mostrar ejemplos de usuarios anteriores para reforzar la confianza.</td></tr>
    <tr><td>Publicación de eventos y postulación</td><td>No observó claramente cómo gestionar fechas disponibles, pero entendió que la plataforma facilita encontrar oportunidades para tocar.</td></tr>
    <tr><td>Planes y diferencias de servicios</td><td>Valoró positivamente los diferentes planes (básico, medio y premium) y consideró que los precios son adecuados en comparación al mercado.</td></tr>
  </tbody>
</table>
[URL de la entrevista](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202310988_upc_edu_pe/ESDM8thHRehIhtIRW0xccVkBOmuRNRItcUYWGiqwzNCL4Q?e=76Uw2x)

### Segmento : Promotores

**Entrevista 1** 

<table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th><strong>Dato</strong></th>
      <th><strong>Información</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Nombre completo</td><td>William Agustín Ventura Saldaña</td></tr>
    <tr><td>Edad</td><td>27 años</td></tr>
    <tr><td>Distrito</td><td>Surco</td></tr>
    <tr><td>Inicio de la entrevista</td><td>00:00</td></tr>
    <tr><td>Duración de la entrevista</td><td>06:40</td></tr>
    <tr><td>Foto captura</td><td><img src="/assets/AgustinValidacion.png" alt="Agustín captura"></td></tr>
    <tr><td>Visualización de la Landing Page</td><td>Indicó que la landing page es llamativa y vistosa, transmitiendo confianza especialmente para eventos grandes. Sin embargo, comentó que para personas que buscan algo más discreto podría no ser tan atractiva.</td></tr>
    <tr><td>Exploración de funcionalidades clave</td><td>Comentó que el sistema de validación de requerimientos técnicos de cada artista es útil y genera confianza. También mencionó que el sistema de contratos digitales y pagos protegidos refuerza esta sensación.</td></tr>
    <tr><td>Flujos de registro y navegación inicial</td><td>Opinó que la navegación para iniciar la publicación de un evento es bastante intuitiva y fácil de comprender.</td></tr>
    <tr><td>Publicación de eventos y postulación</td><td>Indicó que la plataforma incluye la mayoría de la información necesaria, como planes y datos de contacto, lo que genera confianza para la gestión de eventos.</td></tr>
    <tr><td>Planes y diferencias de servicios</td><td>Se mostró conforme con las diferencias entre los planes y necesidades, que proporciona."</td></tr>
  </tbody>
</table>
[URL de la entrevista](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202310988_upc_edu_pe/ESDM8thHRehIhtIRW0xccVkBOmuRNRItcUYWGiqwzNCL4Q?e=76Uw2x)

**Entrevista 2**
<table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th><strong>Dato</strong></th>
      <th><strong>Información</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Nombre completo</td><td>David Manuel Torres Meneses</td></tr>
    <tr><td>Edad</td><td>20 años</td></tr>
    <tr><td>Distrito</td><td>Los Olivos</td></tr>
    <tr><td>Inicio de la entrevista</td><td>00:00</td></tr>
    <tr><td>Duración de la entrevista</td><td>06:40</td></tr>
    <tr><td>Foto captura</td><td><img src="/assets/DavidValidacion.png" alt="David captura"></td></tr>
    <tr><td>Visualización de la Landing Page</td><td>Genera alta confianza. La landing page es vista como una herramienta de apoyo fundamental para los promotores. Transmite seriedad y permite sentirse respaldado al momento de agendar o publicar eventos rápidamente.</td></tr>
    <tr><td>Exploración de funcionalidades clave</td><td>Se percibe como didáctica, intuitiva y muy llamativa. Las funcionalidades como la publicación de eventos, la selección en calendario, y el detalle de beneficios son claros y accesibles, facilitando el trabajo del promotor.</td></tr>
    <tr><td>Flujos de registro y navegación inicial</td><td>Flujo intuitivo y funcional. La navegación inicial permite empezar de forma rápida la programación de eventos, seleccionar fechas, lugares y condiciones fácilmente. Además, la validación de requerimientos técnicos por artista mejora la experiencia.</td></tr>
    <tr><td>Publicación de eventos y postulación</td><td>Completo y práctico. Se incluyen todos los requisitos necesarios para publicar eventos: rider técnico, condiciones, ubicación, validaciones de logística y características específicas de cada artista. Se destaca la facilidad para planificar y administrar eventos múltiples.</td></tr>
    <tr><td>Planes y diferencias de servicios</td><td>Aunque actualmente la plataforma es satisfactoria, el entrevistado sugiere mejorar ofreciendo beneficios tipo "Premium" y alianzas estratégicas, que otorguen ventajas tanto a nivel nacional como internacional para promotores frecuentes.</td></tr>
  </tbody>
</table>
[URL de la entrevista](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202310988_upc_edu_pe/ESDM8thHRehIhtIRW0xccVkBOmuRNRItcUYWGiqwzNCL4Q?e=76Uw2x)

**Entrevista 3**
<table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th><strong>Dato</strong></th>
      <th><strong>Información</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Nombre completo</td><td>Ela Moreno</td></tr>
    <tr><td>Edad</td><td>25 años</td></tr>
    <tr><td>Distrito</td><td>Molino</td></tr>
    <tr><td>Inicio de la entrevista</td><td>06:40</td></tr>
    <tr><td>Duración de la entrevista</td><td>06:00</td></tr>
    <tr><td>Foto captura</td><td><img src="/assets/ElaValidacion.png" alt="Ela captura"></td></tr>
    <tr><td>Visualización de la Landing Page</td><td>Le transmitió confianza y profesionalismo. Destacó que el diseño es atractivo, fácil de manejar y que la idea de la plataforma le pareció innovadora.</td></tr>
    <tr><td>Exploración de funcionalidades clave</td><td>Consideró muy útiles las herramientas como el calendario, contratos digitales, validación técnica y gestor de logística. Mencionó que ayudan a ahorrar mucho tiempo.</td></tr>
    <tr><td>Flujos de registro y navegación inicial</td><td>Opinó que la navegación y el flujo son intuitivos y fáciles de entender. No presentó dificultades al comprender cómo registrarse o postular a eventos.</td></tr>
    <tr><td>Publicación de eventos y postulación</td><td>Consideró que el flujo de publicación contiene toda la información necesaria para gestionar un evento y que el sistema facilita la comunicación entre músicos y promotores.</td></tr>
    <tr><td>Planes y diferencias de servicios</td><td>Mencionó que los planes le parecieron buenos y claros. Notó las diferencias y valoró positivamente la existencia de diferentes opciones para distintos tipos de usuarios.</td></tr>
    <tr><td>Sugerencias de mejora</td><td>Sugirió que podría detallarse más información sobre los organizadores de los eventos para generar aún más confianza en los postulantes.</td></tr>
  </tbody>
</table>
[URL de la entrevista](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202310988_upc_edu_pe/ESDM8thHRehIhtIRW0xccVkBOmuRNRItcUYWGiqwzNCL4Q?e=76Uw2x)



  ### 5.3.3. Evaluaciones según herurísticas.

**UX Heuristics & Principles Evaluation**
**Usability – Inclusive Design – Information Architecture**

**CARRERA**: Ingeniería de Software  
**CURSO**: Desarrollo de Aplicaciones Open Source  
**SECCIÓN**: [4334]  
**PROFESORES**: Todos  
**AUDITOR**: Grupo TocaAquí  
**CLIENTE(S)**: Todos

**SITE o APP A EVALUAR**: TocaAquí 

**TAREAS A EVALUAR**

1. Visualización de beneficios y funcionalidades de la plataforma
2. Acceso a la sección de contacto
3. Navegación desde el menú
4. Acceso a los botones de registro por tipo de usuario
5. Cambio de idioma
6. Visualización de testimonios u opiniones



**EVALUACIÓN SEGÚN HEURÍSTICAS**

| # | Heurística | Observación | Severidad (0-4) | Recomendación |
|---|------------|-------------|----------------|---------------|
| 1 | Visibilidad del estado del sistema | No hay indicador visual que confirme que se ha accedido a una sección distinta (por ejemplo, About o Contacto). | 2 | Añadir efectos de scroll o resaltado del menú activo. |
| 2 | Correspondencia entre el sistema y el mundo real | El lenguaje utilizado en botones es claro y amigable ("Únete como artista/promotor"). | 0 | Ninguna. Excelente elección de lenguaje. |
| 3 | Control y libertad del usuario | No hay opción para retroceder fácilmente a la parte superior desde secciones inferiores. | 1 | Añadir un botón “Volver arriba” o scroll automático al hacer clic en el logo. |
| 4 | Consistencia y estándares | Buen uso de íconos y colores consistentes en toda la página. | 0 | Ninguna. |
| 5 | Reconocimiento antes que recuerdo | Secciones como “Equipo” y “Beneficios” están claramente rotuladas. | 0 | Ninguna. |
| 6 | Flexibilidad y eficiencia de uso | El sitio está adaptado a dispositivos móviles (responsive). | 1 | Optimizar el menú para que sea tipo "hamburguesa" en móvil. |
| 7 | Diseño estético y minimalista | El diseño es limpio y moderno, no sobrecarga al usuario. | 0 | Ninguna. |
| 8 | Ayuda y documentación | No hay sección de ayuda visible o guía para nuevos usuarios. | 2 | Incluir una sección tipo “¿Cómo funciona?” con pasos o video explicativo. |


**Evaluación adicional: Inclusive Design**

| Aspecto | Observación | Recomendación |
|---------|-------------|---------------|
| Contraste de colores | El contraste entre texto blanco y fondo es legible, pero el fondo de algunos botones puede mejorar. | Asegurar un contraste mínimo de 4.5:1 en todos los elementos. |
| Tamaño de fuente | Tamaño adecuado en la mayoría de elementos, pero puede ser pequeño en móvil. | Aumentar ligeramente el tamaño en dispositivos pequeños. |
| Inclusión de íconos con texto | Los botones y secciones se entienden sin necesidad de íconos. | Considerar incluir íconos para facilitar el reconocimiento visual. |


# Conclusiones
- TocaAquí responde a una necesidad real en la industria musical independiente, es decir, el proyecto surge como solución a los problemas de informalidad, falta de oportunidades y desorganización que afectan a músicos emergentes y promotores de eventos. Esta plataforma propone profesionalizar el vínculo entre artistas y espacios culturales mediante tecnología segura, accesible y eficiente.

- A través de entrevistas y análisis de segmentos objetivos, se identificó que tanto músicos como promotores demandan herramientas que faciliten la contratación directa, la coordinación logística y el aseguramiento de pagos, confirmando la pertinencia de la solución planteada.

- Aplicando el proceso de Lean UX se establecieron hipótesis, problemas y soluciones que priorizan una experiencia sencilla, intuitiva y confiable. Esto garantiza que la plataforma no solo resuelva problemas técnicos, sino también genere valor emocional y profesional a sus usuarios.

- A diferencia de plataformas existentes que solo ofrecen contactos o promoción de eventos, TocaAquí integra contratación formal, pagos vía escrow, validación técnica y promoción colaborativa, construyendo un ecosistema confiable para el desarrollo de la escena musical emergente.

- La implementación exitosa de TocaAquí no solo beneficiará a músicos y promotores, sino que también contribuirá a dinamizar el circuito cultural independiente, impulsando la profesionalizació
# Bibliografía

- Asociación Peruana de Managers Musicales. (2020). Encuesta sobre el impacto de la pandemia en músicos independientes. Cocktail. https://cocktail.pe/mas-del-80-de-musicos-independientes-padecen-economicamente-durante-la-pandemia/
- Ramos Espinoza, M. A. (2021). Música independiente en Lima: mapeo de un circuito cultural desde las lógicas de sus agentes (Tesis de licenciatura, Pontificia Universidad Católica del Perú). PUCP. https://tesis.pucp.edu.pe/items/ab79feff-9493-4f8e-9aa8-81d3e50ec57d/full
- Soriano, P. D. (2020). Eventos musicales para contribuir a la oferta cultural en el Centro Histórico de Lima. Universidad de San Martín de Porres. https://repositorio.usmp.edu.pe/bitstream/handle/20.500.12727/7073/SORIANO_PD.pdf?sequence=1
