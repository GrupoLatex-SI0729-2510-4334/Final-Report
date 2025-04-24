## Capítulo IV: Product Design

### 4.1. Style Guidelines

#### 4.1.1. General Style Guidelines

#### 4.1.2. Web Style Guidelines

### 4.2. Information Architecture

#### 4.2.1. Organization Systems

#### 4.2.2. Labeling Systems

#### 4.2.3. SEO Tags and Meta Tags

#### 4.2.4. Searching Systems

#### 4.2.5. Navigation Systems

### 4.3. Landing Page UI Design

#### 4.3.1. Landing Page Wireframe

#### 4.3.2. Landing Page Mock-up

### 4.4. Web Applications UX/UI Design

#### 4.4.1. Web Applications Wireframes.

#### 4.4.2. Web Applications Wireflow Diagrams

#### 4.4.3. Web Applications Mock-ups

#### 4.4.4. Web Applications User Flow Diagrams

### 4.5. Web Applications Prototyping

### 4.6. Domain-Driven Software Architecture

#### 4.6.1. Software Architecture Context Diagrams

#### 4.6.2. Software Architecture Container Diagrams

#### 4.6.3. Software Architecture Components Diagrams

### 4.7. Software Object-Oriented Design

#### 4.7.1. Class Diagrams

#### 4.7.2. Class Dictionary

| **Class**          | **Attribute Name**       | **Descripción**                                                                 | **Tipo de Dato**        |
|--------------------|--------------------------|----------------------------------------------------------------------------------|--------------------------|
| **User**           | user_id                  | Identificador único del usuario                                                 | Integer           |
| **User**           | name                     | Nombre completo del usuario                                                     | String                   |
| **User**           | email                    | Dirección de correo electrónico única                                           | String (Email)           |
| **User**           | password                 | Contraseña cifrada del usuario                                                  | String                   |
| **User**           | registration_date        | Fecha de creación de la cuenta                                                  | DateTime                 |
| **User**           |is_active	                | Indica si la cuenta está activa o desactivada	                                  | Boolean                  |
| **User**           |	phone_number	          | Número telefónico como método de contacto alternativo	                          | String                   |
| **ArtistProfile**  | profile_id               | Identificador único del perfil artístico                                        | Integer           |
| **ArtistProfile**  | stage_name               | Nombre artístico o de la banda                                                  | String                   |
| **ArtistProfile**  | music_genre              | Género musical principal                                                        | String                   |
| **ArtistProfile**  | biography                | Breve presentación del artista                                                  | String                   |
| **ArtistProfile**  | multimedia_links         | Enlaces a redes sociales o muestras                                             | Array[String]            |
| **ArtistProfile**  | average_rating           | Puntaje promedio otorgado por locales                                           | Float                    |
| **ArtistProfile**  |	profile_picture         |	Imagen destacada del artista o banda	                                          | String            |
| **ArtistProfile**  |	location                |	Ciudad o distrito donde suelen presentarse                                      |	String                   |
| **ArtistProfile**  |	tags	                  | Palabras clave para facilitar la búsqueda del artista	                          | Array[String]            |
| **PromoterProfile**| promoter_profile_id      | Identificador del perfil de promotor                                            | Integer           |
| **PromoterProfile**| venue_name               | Nombre del local o espacio cultural                                             | String                   |
| **PromoterProfile**| address                  | Dirección del local                                                             | String                   |
| **PromoterProfile**| description              | Descripción del espacio y sus características                                   | String                   |
| **PromoterProfile**| capacity                 | Capacidad máxima del espacio                                                    | Integer                  |
| **PromoterProfile**| average_rating           | Puntaje promedio otorgado por artistas                                          | Float                    |
| **PromoterProfile**|	social_links	          | Enlaces a redes sociales del local                                              |	Array[String]            |
| **PromoterProfile**|	photo_gallery	          | Imágenes del local para mostrarlo mejor en la plataforma                        |	Array[URL]               |
| **PromoterProfile**|	location                |	Ubicación geográfica del local (distrito, ciudad, país)                         |	String                   |
| **Event**          | event_id                 | Identificador único del evento                                                  | Integer           |
| **Event**          | title                    | Nombre del evento                                                               | String                   |
| **Event**          | description              | Detalles del evento                                                             | String                   |
| **Event**          | event_date               | Fecha y hora de realización                                                     | DateTime                 |
| **Event**          | preferred_genre          | Género musical preferido para la presentación                                   | String                   |
| **Event**          |	tickets_link            |	Enlace a plataforma externa de venta de entradas	                              | String                   |
| **Event**          |	rehearsal_required	    | Indica si se requiere ensayo previo                                             |	Boolean                  |
| **Postulation**    | postulation_id           | Identificador de la postulación                                                 | Integer           |
| **Postulation**    | message                  | Mensaje del artista al promotor                                                 | String                   |
| **Postulation**    | postulation_date         | Fecha de envío de la postulación                                                | DateTime                 |
| **Postulation**    |	rehearsal_confirmed	    | Indica si se ha confirmado un ensayo previo                                     |	Boolean                  |
| **Postulation**    |	feedback                |	Comentarios del promotor hacia el artista                                       |	String                   |
| **Contract**       | contract_id              | Identificador del contrato digital                                              | Integer           |
| **Contract**       | pdf_file                 | Ruta o enlace al documento del contrato firmado                                 | String                   |
| **Contract**       | signed_by_artist         | Estado de firma por el artista                                                  | Boolean                  |
| **Contract**       | signed_by_promoter       | Estado de firma por el promotor                                                 | Boolean                  |
| **Contract**       | signing_date             | Fecha en que se completó la firma                                               | DateTime                 |
| **TechRider**      | rider_id                 | Identificador del rider técnico                                                 | Integer           |
| **TechRider**      | requirements             | Lista de requerimientos técnicos                                                | String                   |
| **TechRider**      | approved                 | Estado de aprobación por parte del promotor                                     | Boolean                  |
| **TechRider**      | observations             | Comentarios del promotor                                                        | String                   |
| **TechRider**      |	uploaded_files          |	Archivos técnicos cargados (planos, documentos, etc.)                           |	Array[URL]               |
| **TechRider**      |	status_updated_at       |	Fecha de última actualización del rider	                                        |DateTime                  |
| **Payment**        | payment_id               | Identificador único del pago                                                    | Integer           |
| **Payment**        | amount                   | Monto acordado para el artista                                                  | Decimal                  |
| **Payment**        | payment_date             | Fecha en que se realizó el pago                                                 | DateTime                 |
| **Payment**        |	invoice_file	          | Enlace o ruta del comprobante de pago (boleta/factura)	                        | String / URL             |
| **UserRole**        | role_id               | Identificador del rol de usuario	                                                    | Integer           |
| **UserRole**        | role_name	                  | Nombre del rol (artist, promoter, admin)	                                                  | String                  |
| **EventStatus**        | status_id	             | Identificador del estado del evento	                                                 | DateTime                 |
| **EventStatus**        |	status_name		          | Estado del evento (published, with confirmed, etc.)                        | String             |
| **PostulationStatus**        | status_id	             | Identificador del estado de la postulación	                                                 | DateTime                 |
| **PostulationStatus**        |	status_name			          | Estado de la postulación (pending, accepted, rejected)	                        | String             |
| **PaymentStatus**        | status_id	             | Identificador del estado del pago	                                                 | DateTime                 |
| **PaymentStatus**        |	status_name			          | Estado del pago (pending, escrow, released)		                        | String             |
| **PaymentMethod**        | method_id	             | Identificador del método de pago	                                                 | DateTime                 |
| **PaymentMethod**        |	method_name			          | Método (yape, plin, tarjeta, transferencia, etc.)		                        | String             |
### 4.8. Database Design

#### 4.8.1. Database Diagram
