# Capítulo IV: Product Design

## 4.1. Style Guidelines

El sistema de diseño de AgroFlet se fundamenta en principios de claridad, confianza y accesibilidad universal. Dado que la plataforma será utilizada por actores con diversos niveles de alfabetización digital (desde coordinadores logísticos en oficinas hasta conductores en zonas rurales), la interfaz debe priorizar la legibilidad, la intuición y la consistencia visual en todos los puntos de contacto.

### 4.1.1. General Style Guidelines

La identidad visual de AgroFlet se fundamenta en los elementos conceptuales del logotipo oficial, el cual fusiona un pin de geolocalización, una hoja representativa del sector agrícola y un circuito de ruta logística. El tono de comunicación es profesional, directo y resolutivo, diseñado para transmitir confianza B2B en el ecosistema logístico.

La identidad visual de AgroFlet se fundamenta en principios de claridad, confianza y eficiencia operativa, alineados con el ecosistema agro-logístico.

**Branding**

Para AgroFlet, el branding se diseñó para mostrar confianza corporativa y eficiencia operativa, abarcando el sector de la logística agroalimentaria. Los tres elementos conceptuales del isotipo (el pin de ubicación, la hoja y la carretera en forma de circuito) representan la trazabilidad en tiempo real, el origen agrícola de la carga y la digitalización del transporte terrestre que nuestra plataforma web promete mediante sus funcionalidades principales. En el tema de colores, el color verde representa la frescura de los alimentos perecibles y la sostenibilidad, mientras que el azul marino corporativo representa la seguridad y formalidad B2B, contrastando de buena manera con los detalles naranjas que dinamizan la ruta. El diseño incluye el imagotipo y el nombre del producto dividido cromáticamente ("Agro" y "Flet") para que sea fácil de leer y asociar rápidamente con nuestro modelo de negocio.

<p align="center">
  <img src="assets/images/LogoOfi.png" alt="Agroflet1" title="Agroflet1" width="600">
</p>

**Tipografía:**
Se adopta la familia tipográfica **Inter** (sans-serif) por su alta legibilidad en interfaces densas y tablas de datos. Se establecen jerarquías estrictas: *Headings* (H1-H3) en pesos *SemiBold* y *Body* en peso *Regular*.

<p align="center">
  <img src="assets/images/Inter sans serif.jpeg" alt="typography" title="typography" width="600">
</p>

**Paleta de Colores:**
La paleta de colores de aGROFLET se compone de 5 colores y sus variantes. Los colores, en conjunto, permiten mostrar una claridad en el diseño de las dos aplicaciones.

<p align="center">
  <img src="assets/images/Agroflet coolors.png" alt="coolors" title="coolors" width="600">
</p>

* *Primary (Verde AgroFlet):* `#27AE60`. Transmite sostenibilidad, frescura agrícola y acciones de éxito.
* *Secondary (Azul Marino Corporativo):* `#0B3B60`. Utilizado en tipografía principal, menús de navegación (*Sidebar*) y elementos que requieren transmitir seguridad y formalidad institucional.
* *Accent (Naranja Ruta):* `#F39C12`. Utilizado para resaltar rutas activas, estados pendientes o alertas de nivel medio.
* *Error/Crítico:* `#D32F2F`. Exclusivo para incidencias graves, bloqueos o retrasos críticos.
* *Neutrales:* Escala de grises desde `#F8F9FA` (fondos) hasta `#212529` (texto base).



### 4.1.2. Web Style Guidelines

El diseño del *Landing Page* y la aplicación web se rige por los lineamientos de **Material Design**, asegurando consistencia e interactividad predecible. La implementación técnica del *frontend* utilizará el *framework* Vue.js junto con la biblioteca de componentes **PrimeVue**.

* **Superficies y Elevación:** Uso de tarjetas (*Cards*) con sombras sutiles para agrupar datos, facilitando la lectura de los detalles del flete o perfiles de conductores.
* **Interactividad:** Botones primarios con alto contraste para *Call-to-Actions* (ej. "Reportar Incidencia") y botones tipo *Ghost* para acciones secundarias.
* **Responsividad:** Sistema de grilla fluida de 12 columnas. Diseño *Desktop-First* para el control logístico en oficinas, con adaptabilidad total a dispositivos móviles para consultas rápidas en campo.

## 4.2. Information Architecture

### 4.2.1. Organization Systems

AgroFlet implementa una arquitectura híbrida adaptada a la complejidad logística:

* **Organización Jerárquica:** Utilizada en el *Dashboard*. La información fluye desde indicadores globales (flota activa, alertas) hacia lo particular (listado de viajes y detalle individual).
* **Organización Matricial:** Utilizada en el Historial de Operaciones. Los usuarios cruzan dimensiones de datos (fechas, placas, tipos de producto, estados) para auditar despachos.

### 4.2.2. Labeling Systems

Para cumplir con los estándares de internacionalización (i18n) y garantizar una curva de aprendizaje mínima, se emplea el *Ubiquitous Language* del dominio agro-logístico.

* **Etiquetas de Navegación:** "Dashboard", "Flota", "Historial", "Configuración".
* **Etiquetas de Acción:** Verbos en infinitivo precisos. Ej. "Registrar Unidad", "Asignar Conductor", "Registrar Incidencia".
* **Etiquetas de Estado:** Representan la máquina de estados. Ej. "En Tránsito", "Entregado", "Retrasado", "Cancelado".

### 4.2.3. SEO Tags and Meta Tags

Para maximizar la indexación del *Landing Page* en buscadores B2B, se definen las siguientes etiquetas:

* **Title:** `AgroFlet | Monitoreo y Trazabilidad de Transporte Agrícola en Perú`
* **Meta Description:** `Plataforma web para monitorear en tiempo casi real el transporte terrestre de alimentos perecibles. Reduce mermas y gestiona tu flota logística eficientemente.`
* **Meta Keywords:** `logística agrícola, transporte de alimentos, monitoreo GPS camiones, trazabilidad agroalimentaria, AgroFlet, gestión de flotas Perú`
* **Meta Author:** `AgroFlet Team`

### 4.2.4. Searching Systems

* **Búsqueda Global:** Barra persistente superior para localizar operaciones por ID, placa de la unidad o DNI del conductor.
* **Filtrado Facetado:** En el módulo de historial, filtros combinados (fecha, origen, destino, estado) con actualización en tiempo real en la *Data Table* de PrimeVue.

### 4.2.5. Navigation Systems

* **Global Navigation:** Menú lateral (*Sidebar*) colapsable.
* **Contextual Navigation:** *Breadcrumbs* (migas de pan) para orientar al usuario (ej. `Dashboard > Historial de Operaciones > Viaje #1024`).
* **Local Navigation:** Pestañas (*Tabs*) en vistas detalladas para separar "Información General", "Mapa de Ruta" e "Incidencias".

## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe

El wireframe establece la estructura de la página de aterrizaje en escala de grises. Se prioriza la propuesta de valor en la sección *Hero*, seguida de los beneficios, planes de suscripción y un formulario de contacto. Elaborado utilizando Figma.

> `[Insertar captura de imagen del Wireframe del Landing Page elaborado en Figma]`

### 4.3.2. Landing Page Mock-up

El Mock-up de alta fidelidad integra el isotipo de AgroFlet, la paleta de colores oficial (Azul Marino y Verde AgroFlet) y tipografía Inter. Se evidencia la aplicación de atributos ARIA para accesibilidad (a11y) y selectores de idioma.

> `[Insertar captura de imagen del Mock-up del Landing Page elaborado en Figma]`

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes

Los wireframes de la aplicación web estructuran las vistas protegidas, distribuyendo espacialmente los componentes del *Dashboard* (área de mapa al 70%, lista de operaciones al 30%). Elaborado utilizando Figma.

> `[Insertar capturas de imagen de los Wireframes de la App elaborados en Figma]`

### 4.4.2. Web Applications Wireflow Diagrams

Diagrama que ilustra la progresión lineal de pantallas (User Goal). Muestra el flujo desde la selección de una operación activa en el *Dashboard* hasta la apertura del modal para reportar una incidencia. Elaborado utilizando FigJam / LucidChart.

> `[Insertar captura de imagen del Wireflow]`

### 4.4.3. Web Applications Mock-ups

Interfaces de alta fidelidad construidas aplicando los componentes de la biblioteca PrimeVue (Material Design). Se visualizan las *Data Tables*, tarjetas de resumen, marcadores del mapa y modales de registro con jerarquía de color.

> `[Insertar capturas de imagen de los Mock-ups de la App elaborados en Figma]`

### 4.4.4. Web Applications User Flow Diagrams

Diagrama que mapea las decisiones algorítmicas del usuario (Happy Path y Unhappy Paths). Incluye validaciones lógicas, como el intento de asignar un conductor que ya se encuentra "En Tránsito". Elaborado utilizando FigJam / LucidChart.

> `[Insertar captura de imagen del User Flow]`

## 4.5. Web Applications Prototyping

El prototipo interactivo permite validar heurísticas de usabilidad antes del desarrollo de la aplicación web. Se configuran transiciones, apertura de modales (ej. "Registrar Incidencia") y navegación en el *Sidebar*.

> `[Insertar screenshot del prototipo en Figma]`
> **Enlace al Video Demostrativo:** `[Insertar URL de Microsoft Stream del recorrido del prototipo]`

## 4.6. Domain-Driven Software Architecture

### 4.6.1. Design-Level EventStorming

Aplicando *Domain-Driven Design*, se identificaron los siguientes sub-dominios (Bounded Contexts):

* **Fleet Management:** Gestión de `Vehicle` y `Driver`.
* **Shipment Tracking:** Control del ciclo de vida de `Shipment` y registro de `Incident`.
* **Identity and Access Management:** Autenticación y perfiles de `User`.

> `[Insertar captura de imagen del EventStorming (Miro / FigJam)]`

### 4.6.2. Software Architecture Context Level Diagram

El Nivel 1 del Modelo C4 describe las interacciones globales. Elaborado utilizando Structurizr.

```plantuml
@startuml
!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Context.puml

Person(producer, "Despachador", "Coordina envíos de carga agrícola.")
Person(buyer, "Comprador Mayorista", "Supervisa la recepción de envíos.")

System(agroflet, "AgroFlet System", "Plataforma de trazabilidad logística y monitoreo.")

System_Ext(mapsApi, "Servicio Externo de Mapas", "Provee geolocalización y trazado de rutas (ej. Google Maps).")
System_Ext(emailApi, "Servicio de Correos", "Envía notificaciones transaccionales y alertas.")

Rel(producer, agroflet, "Registra y monitorea operaciones", "HTTPS")
Rel(buyer, agroflet, "Consulta ETA y ubicación", "HTTPS")
Rel(agroflet, mapsApi, "Obtiene geolocalización", "REST API")
Rel(agroflet, emailApi, "Envía alertas de incidencias", "REST API")
@enduml

```

> `[Reemplazar bloque de código por la exportación visual de Structurizr o PlantUML]`

### 4.6.3. Software Architecture Container Level Diagrams

El Nivel 2 del Modelo C4 desglosa los contenedores desplegables.

```plantuml
@startuml
!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Container.puml

Person(user, "Usuario (Despachador/Comprador)")

System_Boundary(c1, "AgroFlet") {
    Container(web_app, "Single-Page Application", "Vue.js, PrimeVue", "Provee la interfaz cliente responsive.")
    Container(api, "RESTful API", "ASP.NET Core, C#", "Provee la lógica de negocio y endpoints mediante Swagger.")
    ContainerDb(db, "Relational Database", "MySQL", "Almacena usuarios, flotas, viajes e incidencias.")
}

System_Ext(mapsApi, "Servicio de Mapas", "Map API")

Rel(user, web_app, "Navega y visualiza datos", "HTTPS")
Rel(web_app, api, "Consume Endpoints RESTful", "JSON/HTTPS")
Rel(api, db, "Lee y escribe registros", "Entity Framework Core / TCP")
Rel(web_app, mapsApi, "Carga capa geoespacial", "HTTPS")
@enduml

```

> `[Reemplazar bloque de código por la exportación visual]`

### 4.6.4. Software Architecture Component Level Diagrams

El Nivel 3 del Modelo C4 detalla la estructura interna del contenedor RESTful API utilizando ASP.NET Core.

> `[Insertar diagrama de Componentes evidenciando Controllers (ej. ShipmentsController), Services (ILogisticsService) y Repositories (UnitOfWork)]`

## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams

Diseño orientado a objetos en C#, aplicando encapsulamiento para proteger la integridad de las reglas de negocio financieras y logísticas. Elaborado utilizando UML.

```plantuml
@startuml
package "AgroFlet.Domain.Entities" {
    class User {
        + Id : Guid
        + FirstName : string
        + LastName : string
        + Email : string
        + Role : RoleType
    }

    class Vehicle {
        + Id : Guid
        + LicensePlate : string
        + CapacityTons : decimal
        + Status : VehicleStatus
    }

    class Driver {
        + Id : Guid
        + FullName : string
        + Dni : string
        + LicenseNumber : string
    }

    class Shipment {
        + Id : Guid
        + CargoDescription : string
        + Origin : string
        + Destination : string
        + Status : ShipmentStatus
        + DepartureTime : DateTime
        + ETA : DateTime
        + StartTransit() : void
        + ReportIncident(Incident) : void
        + MarkAsDelivered() : void
    }

    class Incident {
        + Id : Guid
        + Description : string
        + Severity : IncidentSeverity
        + ImpactHours : int
        + ReportedAt : DateTime
    }

    Shipment "1" *-- "0..*" Incident : Registra >
    Shipment "1" -- "1" Vehicle : Utiliza >
    Shipment "1" -- "1" Driver : Conducido por >
    User "1" -- "0..*" Shipment : Monitorea >
}
@enduml

```

> `[Reemplazar bloque de código por la exportación visual del Diagrama de Clases]`

## 4.8. Database Design

### 4.8.1. Database Diagrams

El diagrama Entidad-Relación (ERD) modela la persistencia en el motor relacional MySQL. Se aseguran las llaves foráneas (FK) y la integridad de los datos logísticos.

```plantuml
@startuml
entity "Users" as users {
  * Id : CHAR(36) <<PK>>
  --
  FirstName : VARCHAR(100)
  LastName : VARCHAR(100)
  Email : VARCHAR(150) <<UK>>
  PasswordHash : VARCHAR(255)
  Role : VARCHAR(50)
}

entity "Vehicles" as vehicles {
  * Id : CHAR(36) <<PK>>
  --
  LicensePlate : VARCHAR(15) <<UK>>
  CapacityTons : DECIMAL(10,2)
  Status : VARCHAR(50)
}

entity "Drivers" as drivers {
  * Id : CHAR(36) <<PK>>
  --
  FullName : VARCHAR(150)
  Dni : VARCHAR(8) <<UK>>
  LicenseNumber : VARCHAR(20)
}

entity "Shipments" as shipments {
  * Id : CHAR(36) <<PK>>
  --
  VehicleId : CHAR(36) <<FK>>
  DriverId : CHAR(36) <<FK>>
  CargoDescription : VARCHAR(255)
  Origin : VARCHAR(150)
  Destination : VARCHAR(150)
  DepartureTime : DATETIME
  ETA : DATETIME
  Status : VARCHAR(50)
}

entity "Incidents" as incidents {
  * Id : CHAR(36) <<PK>>
  --
  ShipmentId : CHAR(36) <<FK>>
  Description : TEXT
  Severity : VARCHAR(50)
  ReportedAt : DATETIME
}

shipments }o--|| vehicles
shipments }o--|| drivers
incidents }o--|| shipments
@enduml

```

> `[Reemplazar bloque de código por el diagrama ERD generado en MySQL Workbench o LucidChart]`



# Capítulo IV: Product Design

## 4.1. Style Guidelines

### 4.1.1. General Style Guidelines

### 4.1.2. Web Style Guidelines

## 4.2. Information Architecture

### 4.2.1. Organization Systems

### 4.2.2. Labeling Systems

### 4.2.3. SEO Tags and Meta Tags

### 4.2.4. Searching Systems

### 4.2.5. Navigation Systems

## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe

### 4.3.2. Landing Page Mock-up

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes

### 4.4.2. Web Applications Wireflow Diagrams

### 4.4.3. Web Applications Mock-ups

### 4.4.4. Web Applications User Flow Diagrams

## 4.5. Web Applications Prototyping

## 4.6. Domain-Driven Software Architecture

### 4.6.1. Design-Level EventStorming

### 4.6.2. Software Architecture Context Level Diagram

### 4.6.3. Software Architecture Container Level Diagrams

### 4.6.4. Software Architecture Component Level Diagrams

## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams

## 4.8. Database Design

### 4.8.1. Database Diagrams
