## Capítulo III: Requirements Specification

### 3.1. To-Be Scenario Mapping

### 3.2. User Stories

### 3.3. Impact Mapping
<br><img src="/assets/Impact Mapping - Toca Aqui.png"><br>

### 3.4. Product Backlog
| Orden | User Story Id | Título                                             | Descripción                                                                                             | Story Points |
|-------|---------------|----------------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------|
| 1     | US001         | Visualización clara del propósito de la plataforma | Como visitante, quiero entender rápidamente qué es TocaAquí y cómo funciona, para saber si es relevante para mí como artista o local. | 1            |
| 2     | US002         | Visualización de planes para artistas y locales    | Como visitante, quiero ver claramente los diferentes planes disponibles para artistas y locales, para decidir cuál se adapta mejor a mis necesidades. | 2            |
| 3     | US003         | Visualización del equipo de desarrollo en la landing | Como visitante curioso, quiero conocer al equipo que desarrolla TocaAquí, para sentir mayor confianza en la solución. | 1            |
| 4     | US004         | Acceso rápido a registro desde botones CTA          | Como visitante interesado, quiero encontrar botones claros para registrarme como artista o local, para comenzar a usar la plataforma con un clic. | 1            |
| 5     | US005         | Visualización adecuada en móviles y pantallas pequeñas | Como visitante, quiero que el sitio se adapte bien a mi celular o tablet, para tener una buena experiencia sin importar el dispositivo. | 3            |
| 6     | US006         | Navegación accesible desde menú fijo               | Como visitante, quiero contar con un menú que permanezca visible mientras navego, para acceder fácilmente a cualquier sección de la página. | 2            |
| 7     | US007         | Acceso a la versión en inglés del sitio            | Como visitante extranjero, quiero ver la página en inglés, para comprender toda la información sin barreras de idioma. | 3            |
| 8     | US008         | Envío de un mensaje a través del formulario de contacto | Como visitante con dudas, quiero enviar un mensaje desde el formulario de contacto, para comunicarme fácilmente con el equipo de TocaAquí. | 2            |
| 9     | US009         | Selección del tipo de usuario desde la landing      | Como visitante interesado, quiero seleccionar si soy artista o promotor desde la landing, para empezar mi registro adecuadamente. | 2            |
| 10    | US010         | Registro como artista en la plataforma             | Como artista nuevo, quiero registrarme en TocaAquí seleccionando mi rol, para acceder a mi panel personalizado. | 3            |
| 11    | US011         | Registro como administrador de local               | Como promotor o administrador de un espacio, quiero registrarme con mi rol, para acceder a herramientas de gestión de eventos. | 3            |
| 12    | US012         | Acceso al dashboard del artista                    | Como artista registrado, quiero ingresar a un panel con herramientas específicas para músicos, para gestionar mis eventos y perfil fácilmente. | 3            |
| 13    | US013         | Acceso al dashboard del local                      | Como administrador de local, quiero visualizar un panel con mis shows y herramientas clave, para organizar fácilmente mis eventos. | 3            |
| 14    | US014         | Publicación de eventos musicales                    | Como promotor, quiero publicar fechas disponibles con condiciones específicas, para recibir postulaciones de bandas que cumplan mis criterios. | 3            |
| 15    | US015         | Búsqueda de eventos compatibles con mi perfil       | Como artista, quiero ver eventos recomendados según mi género musical y ubicación, para postular solo a los que se alinean con mi estilo. | 3            |
| 16    | US016         | Postulación rápida a un evento desde la plataforma  | Como artista, quiero postularme a un evento en pocos pasos, para agilizar mi proceso de presentación. | 2            |
| 17    | US017         | Revisión de postulaciones y selección de artista    | Como administrador de local, quiero ver postulaciones y elegir la mejor opción, para asegurar un show alineado a mi público. | 2            |
| 18    | US018         | Gestión y edición de mi perfil artístico           | Como artista, quiero crear y editar mi perfil con bio, estilo musical y multimedia, para mostrarme profesionalmente a los locales. | 2            |
| 19    | US019         | Evaluación del artista luego del evento             | Como administrador de local, quiero calificar a las bandas post show, para contribuir a su reputación en la comunidad. | 2            |
| 20    | US020         | Subida y validación del rider técnico              | Como artista confirmado, quiero subir mi rider técnico, para que el promotor lo revise y apruebe antes del evento. | 2            |
| 21    | US021         | Validación del rider técnico por parte del promotor | Como promotor, quiero revisar el rider técnico del artista y enviar comentarios, para coordinar la logística del show. | 2            |
| 22    | US022         | Visualización de pagos recibidos y pendientes      | Como artista, quiero revisar mis pagos pendientes, liberados y el historial de ingresos, para tener control sobre mis ganancias. | 2            |
| 23    | US023         | Validación del show y ejecución del pago           | Como promotor, quiero confirmar que un evento se realizó correctamente, para liberar el pago al artista desde el sistema escrow. | 2            |
| 24    | TS001         | Registro de usuario (artista o promotor) a través de un RESTful API        | Como desarrollador, quiero implementar el registro de usuarios a través de un RESTful API, para que puedan acceder a la plataforma según su rol. | 3            |
| 25    | TS002         | Inicio de sesión mediante RESTful API               | Como desarrollador, quiero implementar el login a través de un RESTful API, para autenticar a los usuarios y dar acceso al dashboard correspondiente. | 3            |
| 26    | TS003         | Publicar evento desde un RESTful API               | Como desarrollador, quiero permitir que un local publique un evento a través de un RESTful API, para mostrarlo en la sección de eventos disponibles. | 3            |
| 27    | TS004         | Postulación del artista a un evento vía RESTful API           | Como desarrollador, quiero permitir que un artista postule a un evento mediante un RESTful API, para registrar su interés formalmente. | 3            |
| 28    | TS005         | Firma del contrato digital mediante RESTful API              | Como desarrollador, quiero permitir que artista y local firmen un contrato desde la plataforma usando un RESTful API, para formalizar el acuerdo. | 3            |
| 29    | TS006         | Validación del rider técnico por el promotor vía RESTful API          | Como desarrollador, quiero permitir que los promotores validen o rechacen el rider técnico mediante un RESTful API, para coordinar la logística del evento. | 2            |
| 30    | TS007         | Confirmación del evento y liberación de pago vía RESTful API | Como desarrollador, quiero que el promotor confirme la realización del evento mediante un RESTful API, para activar la liberación del pago al artista. | 3            |
| 31    | TS008         | Liberación automática del pago por escrow mediante RESTful API | Como desarrollador, quiero implementar la lógica de liberación de pagos por escrow a través de un RESTful API, para que el artista reciba su dinero al concluir el evento. | 3            |
| 32    | TS009         | Subir rider técnico mediante RESTful API            | Como desarrollador, quiero permitir que los artistas suban su rider técnico a través de un RESTful API, para que los promotores lo validen antes del evento. | 2            |
| 33    | TS010         | Publicación de fechas disponibles del local vía RESTful API        | Como desarrollador, quiero permitir que el promotor registre sus fechas disponibles mediante un RESTful API, para que los artistas puedan postular. | 2            |
| 34    | TS011         | Visualización de postulaciones del artista vía RESTful API       | Como desarrollador, quiero permitir que el artista vea sus postulaciones enviadas a través de un RESTful API, para que pueda seguir su estado. | 2            |
| 35    | TS012         | Evaluación post-evento mediante RESTful API        | Como desarrollador, quiero permitir que artistas y locales se evalúen mutuamente a través de un RESTful API, para construir la reputación dentro de la plataforma. | 2            |
| 36    | TS013         | Carga y edición del perfil artístico vía RESTful API        | Como desarrollador, quiero permitir que el artista cree y edite su perfil mediante un RESTful API, para mantener su información profesional actualizada. | 2            |
