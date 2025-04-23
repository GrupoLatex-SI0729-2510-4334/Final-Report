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
| **User**           | user_id                  | Identificador único del usuario                                                 | UUID / Integer           |
| **User**           | name                     | Nombre completo del usuario                                                     | String                   |
| **User**           | email                    | Dirección de correo electrónico única                                           | String (Email)           |
| **User**           | password                 | Contraseña cifrada del usuario                                                  | String                   |
| **User**           | role                     | Tipo de usuario (artist, promoter, admin)                                       | Enum                     |
| **User**           | registration_date        | Fecha de creación de la cuenta                                                  | DateTime                 |
| **ArtistProfile**  | profile_id               | Identificador único del perfil artístico                                        | UUID / Integer           |
| **ArtistProfile**  | stage_name               | Nombre artístico o de la banda                                                  | String                   |
| **ArtistProfile**  | music_genre              | Género musical principal                                                        | String                   |
| **ArtistProfile**  | biography                | Breve presentación del artista                                                  | String                   |
| **ArtistProfile**  | multimedia_links         | Enlaces a redes sociales o muestras                                             | Array[String]            |
| **ArtistProfile**  | average_rating           | Puntaje promedio otorgado por locales                                           | Float                    |
| **PromoterProfile**| promoter_profile_id      | Identificador del perfil de promotor                                            | UUID / Integer           |
| **PromoterProfile**| venue_name               | Nombre del local o espacio cultural                                             | String                   |
| **PromoterProfile**| address                  | Dirección del local                                                             | String                   |
| **PromoterProfile**| description              | Descripción del espacio y sus características                                   | String                   |
| **PromoterProfile**| capacity                 | Capacidad máxima del espacio                                                    | Integer                  |
| **PromoterProfile**| average_rating           | Puntaje promedio otorgado por artistas                                          | Float                    |
| **Event**          | event_id                 | Identificador único del evento                                                  | UUID / Integer           |
| **Event**          | title                    | Nombre del evento                                                               | String                   |
| **Event**          | description              | Detalles del evento                                                             | String                   |
| **Event**          | event_date               | Fecha y hora de realización                                                     | DateTime                 |
| **Event**          | preferred_genre          | Género musical preferido para la presentación                                   | String                   |
| **Event**          | status                   | Estado del evento (published, with applications, confirmed, completed)          | Enum                     |
| **Postulation**    | postulation_id           | Identificador de la postulación                                                 | UUID / Integer           |
| **Postulation**    | message                  | Mensaje del artista al promotor                                                 | String                   |
| **Postulation**    | status                   | Estado de la postulación (pending, accepted, rejected)                          | Enum                     |
| **Postulation**    | postulation_date         | Fecha de envío de la postulación                                                | DateTime                 |
| **Contract**       | contract_id              | Identificador del contrato digital                                              | UUID / Integer           |
| **Contract**       | pdf_file                 | Ruta o enlace al documento del contrato firmado                                 | String                   |
| **Contract**       | signed_by_artist         | Estado de firma por el artista                                                  | Boolean                  |
| **Contract**       | signed_by_promoter       | Estado de firma por el promotor                                                 | Boolean                  |
| **Contract**       | signing_date             | Fecha en que se completó la firma                                               | DateTime                 |
| **TechRider**      | rider_id                 | Identificador del rider técnico                                                 | UUID / Integer           |
| **TechRider**      | requirements             | Lista de requerimientos técnicos                                                | String                   |
| **TechRider**      | approved                 | Estado de aprobación por parte del promotor                                     | Boolean                  |
| **TechRider**      | observations             | Comentarios del promotor                                                        | String                   |
| **Payment**        | payment_id               | Identificador único del pago                                                    | UUID / Integer           |
| **Payment**        | amount                   | Monto acordado para el artista                                                  | Decimal                  |
| **Payment**        | status                   | Estado del pago (pending, escrow, released)                                     | Enum                     |
| **Payment**        | payment_date             | Fecha en que se realizó el pago                                                 | DateTime                 |

### 4.8. Database Design

#### 4.8.1. Database Diagram
