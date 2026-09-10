# Capítulo IV: Product Design

## 4.1. Style Guidelines

El sistema de diseño de AgroFlet se fundamenta en principios de claridad, confianza y accesibilidad universal. Dado que la plataforma será utilizada por actores con diversos niveles de alfabetización digital (desde coordinadores logísticos en oficinas hasta conductores en zonas rurales), la interfaz debe priorizar la legibilidad, la intuición y la consistencia visual en todos los puntos de contacto.

### 4.1.1. General Style Guidelines

La identidad visual de AgroFlet se fundamenta en los elementos conceptuales del logotipo oficial, el cual fusiona un pin de geolocalización, una hoja representativa del sector agrícola y un circuito de ruta logística. El tono de comunicación es profesional, directo y resolutivo, diseñado para transmitir confianza B2B en el ecosistema logístico.

La identidad visual de AgroFlet se fundamenta en principios de claridad, confianza y eficiencia operativa, alineados con el ecosistema agro-logístico.

**4.1.1.1. Branding**

Para AgroFlet, el branding se diseñó para mostrar confianza corporativa y eficiencia operativa, abarcando el sector de la logística agroalimentaria. Los tres elementos conceptuales del isotipo (el pin de ubicación, la hoja y la carretera en forma de circuito) representan la trazabilidad en tiempo real, el origen agrícola de la carga y la digitalización del transporte terrestre que nuestra plataforma web promete mediante sus funcionalidades principales. En el tema de colores, el color verde representa la frescura de los alimentos perecibles y la sostenibilidad, mientras que el azul marino corporativo representa la seguridad y formalidad B2B, contrastando de buena manera con los detalles naranjas que dinamizan la ruta. El diseño incluye el imagotipo y el nombre del producto dividido cromáticamente ("Agro" y "Flet") para que sea fácil de leer y asociar rápidamente con nuestro modelo de negocio.

<br>

<p align="center">
  <img src="assets/images/LogoOfi.png" alt="Agroflet1" alt="logo" title="logo-Agroflet1" width="600">
</p>



**4.1.1.1. Typography:**

La tipografía de AgroFlet ha sido definida con el objetivo de mantener una interfaz clara, profesional y legible en contextos donde los usuarios necesitan consultar y gestionar información relacionada con el transporte agrícola de manera rápida. Esto incluye el registro de envíos, consulta del estado de las operaciones, revisión de incidencias, posiciones reportadas, rutas planificadas, notificaciones y gestión de recursos de transporte. La familia tipográfica principal de la plataforma es Inter, seleccionada por su alta legibilidad en interfaces digitales y su versatilidad para establecer distintos niveles de jerarquía visual. Su uso se mantiene de manera consistente tanto en la aplicación web como en los componentes informativos asociados a AgroFlet.
Se emplean diferentes pesos de Inter según la importancia del contenido, permitiendo diferenciar títulos, encabezados, textos principales, información auxiliar y etiquetas sin recurrir a una cantidad excesiva de estilos tipográficos.

La jerarquía tipográfica de AgroFlet se organiza de la siguiente manera:

* **Page Title / H1:** Inter Bold, 32 px
* **Section Heading / H2:** Inter SemiBold, 24 px
* **Subheading / H3:** Inter SemiBold, 20 px
* **Body Text:** Inter Regular, 16 px
* **Small / Auxiliary Text:** Inter Regular, 14 px
* **Labels / Caption:** Inter Regular, 12 px

El interlineado se establece aproximadamente entre 1.3 y 1.5 veces el tamaño de la fuente, favoreciendo la lectura tanto en bloques de contenido como en interfaces que presentan información operativa. Esta configuración permite mantener una separación visual adecuada entre títulos, datos de los envíos, estados, formularios y mensajes del sistema. La consistencia tipográfica contribuye a que el usuario pueda identificar rápidamente la importancia de cada elemento. Por ejemplo, el título de una operación utiliza una jerarquía mayor, mientras que información complementaria como “Última actualización: 09:30” utiliza un tamaño menor para evitar competir visualmente con los datos principales.

<br>

<p align="center">
  <img src="assets/images/Thypografía-Agroflet.jpeg" alt="typography" title="typography" width="1500">
  <em>Nota. Sistema tipográfico utilizado en la identidad visual de Agroflet.</em>
</p>


**4.1.1.2. Paleta de Colores:**

La paleta de colores de AgroFlet ha sido definida con el propósito de transmitir una identidad visual moderna, confiable y relacionada con el entorno agrícola y logístico. El sistema combina colores propios de la marca con tonos estructurales, fondos neutros y colores semánticos que permiten diferenciar acciones, estados e información dentro de la plataforma.

El **Primary Green (`#27AE60`)** constituye uno de los principales colores de identidad de AgroFlet. El verde representa la relación de la plataforma con el sector agrícola, la sostenibilidad y el entorno productivo. Se utiliza principalmente en elementos de identidad, iconografía destacada y determinados componentes visuales.

Para las acciones principales se utiliza el **Action Green (`#176B3A`)**, un tono de mayor contraste pensado para elementos interactivos como botones principales, confirmaciones y acciones relevantes dentro de la aplicación. Su utilización permite distinguir las acciones disponibles sin depender únicamente del color para comunicar su función.

El **Navy (`#0B3B60`)** se emplea principalmente en títulos, navegación y elementos estructurales. Este tono aporta contraste al verde principal y busca transmitir confianza, estabilidad y profesionalismo dentro del contexto logístico.

Como color complementario se utiliza el **Accent Orange (`#F39C12`)**, reservado para elementos de énfasis, indicadores y determinadas acciones que requieren atención sin representar necesariamente una situación de error.

Los colores principales de AgroFlet son:

* **Primary Green:** `#27AE60` — identidad de marca y elementos destacados.
* **Action Green:** `#176B3A` — botones y acciones principales.
* **Navy:** `#0B3B60` — navegación, encabezados y elementos estructurales.
* **Accent Orange:** `#F39C12` — elementos de énfasis e indicadores.

Para fondos y superficies se utilizan principalmente tonos claros que facilitan la organización de la información:

* **White:** `#FFFFFF` — fondo principal.
* **Background Light:** `#F8F9FA` — superficies, tarjetas y formularios.
* **Blue Tint:** `#EAF4FF` — secciones informativas o áreas destacadas.

AgroFlet también incorpora colores semánticos para comunicar los resultados de determinadas operaciones. El **Success Green (`#059669`)** representa procesos completados correctamente; el **Warning Orange (`#F59E0B`)** se utiliza para advertencias o situaciones que requieren atención; y el **Error Red (`#D32F2F`)** identifica errores, cancelaciones o incidencias críticas.

El color no se utiliza como único mecanismo para comunicar un estado. Los indicadores se complementan con texto, iconografía y etiquetas, permitiendo que el significado pueda ser interpretado incluso cuando el usuario no diferencia correctamente determinados colores.

Por ejemplo, un envío no se identifica únicamente mediante un indicador verde, sino mediante una combinación como icono + “En tránsito”. De la misma manera, una incidencia crítica utiliza un icono, una descripción y el color correspondiente.

El uso consistente de esta paleta permite establecer una jerarquía visual clara, diferenciar acciones y estados y, al mismo tiempo, reforzar la identidad gráfica de AgroFlet.

<br>

<p align="center">
  <img src="assets/images/cOLORS-Agroflet.jpeg" alt="color palette" title="color palette" width="2000">
   <em>Nota. Sistema cromático utilizado en la identidad visual de AgroFlet.</em>
</p>


**4.1.1.3. Spacing:**

El sistema de espaciado de AgroFlet se basa en una cuadrícula de 4 píxeles, permitiendo mantener consistencia entre los diferentes componentes de la interfaz. A partir de esta unidad base se utilizan principalmente valores de 4, 8, 12, 16, 24 y 32 píxeles, dependiendo de la relación existente entre los elementos y del nivel de separación requerido.

Los espacios de **4 px** se emplean entre elementos estrechamente relacionados, como un icono y su etiqueta. Los **8 px** permiten separar controles o elementos pertenecientes al mismo grupo, mientras que los **12 px** se utilizan en componentes pequeños o separaciones internas frecuentes.

Los **16 px** se emplean principalmente como espaciado interno de tarjetas, formularios y grupos de información. Los **24 px** permiten establecer una separación visual más clara entre componentes o subsecciones, mientras que los **32 px** se utilizan para dividir bloques principales dentro de una vista.

La escala de espaciado utilizada en AgroFlet es:

* **4 px:** separación mínima.
* **8 px:** elementos relacionados.
* **12 px:** componentes pequeños.
* **16 px:** separación interna de componentes.
* **24 px:** tarjetas y secciones.
* **32 px:** bloques principales.

Este sistema facilita la organización visual de información relacionada con operaciones logísticas, como tarjetas de envíos, formularios de registro, información del vehículo, conductor, incidencias y estados de transporte.

Asimismo, permite evitar la saturación visual y mantener una experiencia predecible entre las distintas vistas de la plataforma, especialmente cuando el usuario necesita revisar una cantidad considerable de información operativa.

<br>

<p align="center">
  <img src="assets/images/spacing-Agroflet.jpeg" alt="spacing system" title="spacing system" width="1500">
  <em>Nota. Sistema de espaciado utilizado en la interfaz de AgroFlet.</em>
</p>


**4.1.1.4. Iconography:**

La iconografía de AgroFlet sigue un estilo simple, lineal, reconocible y consistente, orientado a facilitar la identificación rápida de las principales funciones de la plataforma. Los iconos funcionan como apoyo visual para elementos de navegación, acciones, formularios, estados y diferentes procesos relacionados con la coordinación del transporte agrícola.

Se priorizan iconos de apariencia limpia, evitando ilustraciones excesivamente complejas que puedan aumentar la carga visual de la interfaz. Los iconos mantienen proporciones y estilos similares dentro de cada contexto de uso, contribuyendo a generar una experiencia visual uniforme.

Entre los principales elementos representados mediante iconografía se encuentran:

* **Inicio / Dashboard**
* **Envíos**
* **Vehículos**
* **Conductores**
* **Notificaciones**
* **Buscar**
* **Registrar envío**
* **Rutas**
* **Configuración**
* **Perfil**

Los iconos asociados a acciones principales pueden utilizar los tonos verdes de AgroFlet, mientras que los elementos secundarios emplean colores neutros o el **Navy (`#0B3B60`)**. Los estados críticos pueden utilizar el **Error Red (`#D32F2F`)** y las advertencias el **Accent Orange (`#F39C12`)**.

Los iconos no reemplazan por completo al contenido textual en las operaciones importantes. Cuando una acción puede resultar ambigua, se acompaña de una etiqueta descriptiva, por ejemplo “Registrar envío”, “Notificaciones”, “Configuración” o “Ver detalles”.

Este enfoque reduce la carga cognitiva del usuario y permite reconocer más rápidamente las acciones disponibles, especialmente en vistas que contienen múltiples operaciones, vehículos, conductores o notificaciones.

<br>

<p align="center">
  <img src="assets/images/Iconografía-Agroflet.jpeg" alt="iconography system" title="iconography system" width="1500">
  <em>Nota. Sistema de iconografía utilizado en la interfaz de AgroFlet.</em>
</p>


**4.1.1.5. Tone of Communication and Applied Language:**

El tono de comunicación de AgroFlet es claro, profesional, respetuoso, sereno y orientado a la acción, priorizando la precisión sobre la certeza absoluta. Dado que la plataforma gestiona operaciones agrícolas, se evitan tecnicismos innecesarios y expresiones absolutas cuando solo se cuenta con datos estimados o reportados previamente.

* Se utilizan términos precisos como “Ruta planificada”, “Posición reportada” o “Llegada estimada”.
* Los mensajes de error describen primero el problema y luego la solución (por ejemplo, *"Ubicación no disponible. Última actualización: 09:30"*).
* La interfaz prioriza instrucciones breves y se encuentra disponible tanto en español latinoamericano como en inglés, manteniendo la misma claridad en ambos idiomas.

Algunos ejemplos clave del lenguaje empleado en la plataforma son:

* **Acciones:** “Registrar envío”, “Iniciar traslado”, “Registrar incidencia”, “Ver detalles”.
* **Estados y datos:** “Posición reportada”, “Ruta planificada”, “Ubicación no disponible”, “Operación entregada”.

Este enfoque reduce la ambigüedad y genera confianza tanto en los despachadores como en los compradores que consultan el estado de las operaciones.

<br>

<p align="center">
  <img src="assets/images/Tono-Comunicacion-Agroflet.jpeg" alt="tone of communication" title="tone of communication" width="1500">
</p>

<p align="center">
  <em>Nota. Tono de comunicación y lenguaje aplicado en la interfaz de AgroFlet.</em>
</p>

### 4.1.2. Web Style Guidelines

En el diseño visual de AgroFlet se adopta una línea gráfica moderna, profesional y funcional, enfocada en la eficiencia operativa y la claridad de la información logística. La jerarquía visual se construye mediante el uso de tipografías bien definidas (familia Inter), tamaños diferenciados y colores de alto contraste (verde agrícola y azul marino corporativo) que permiten identificar rápidamente los elementos más importantes, como los estados de los fletes. Los botones interactivos y componentes basados en Material Design y PrimeVue presentan estados visuales claros (normal, hover y activo), brindando retroalimentación inmediata al usuario. El uso de tarjetas (cards) con bordes suaves y sombras sutiles contribuye a una interfaz limpia y organizada, evitando distracciones innecesarias durante el monitoreo de rutas. Asimismo, los componentes visuales están diseñados para mantener consistencia en toda la plataforma, facilitando la navegación y reduciendo la curva de aprendizaje del usuario (productores y compradores mayoristas). Finalmente, cada elemento del diseño ha sido pensado para cumplir un propósito funcional dentro de la experiencia de gestión de flotas, asegurando que la interfaz no solo sea atractiva, sino también eficiente en contextos donde la rapidez y la precisión son esenciales. Además, el diseño considera principios de diseño responsive, asegurando que la interfaz mantenga su funcionalidad y claridad en distintos dispositivos y tamaños de pantalla, tanto en la aplicación web como en el Landing Page.

## 4.2. Information Architecture

### 4.2.1. Organization Systems

Para nuestra plataforma se opta por una organización visual jerárquica con elementos secuenciales. Esto permite que el usuario identifique fácilmente los puntos clave, organizando el contenido en categorías principales como "Dashboard", "Flota", "Historial de Operaciones" y "Configuración", y en subcategorías dentro de cada una. Así, la información logística y los datos de rastreo se presentan de forma clara y sin sobrecargar la pantalla.

Además, en ciertas secciones se incorporan flujos secuenciales que guían al usuario paso a paso para completar tareas o llegar a páginas específicas (por ejemplo, el registro de una nueva unidad de transporte o el reporte de una incidencia en ruta). Esta estructura facilita aplicar principios de arquitectura de información como claridad, accesibilidad, navegación enfocada y facilidad de uso. Finalmente, gracias a la investigación previa y la definición de los User Personas, se asegura que el contenido de cada categoría sea relevante y útil para el usuario.

<p align="center">
  <img src="assets/images/arquitectura de landing agroflett.jpeg" title="arquiinfooo" width="600">
</p>
<p align="center">
  Nota: Diagrama de organización de información del landing page.<br>
</p>

<strong>Acceso al diagrama de la Arquitectura de Información (Miro):</strong><br>
https://miro.com/app/board/uXjVHpjtvic=/?share_link_id=251750996606

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

### Wireframes Desktop de la Landing Page

**Landing Wireframe Desktop 1**

![Landing Wireframe Desktop 1](assets/images/Landing_Desktop1.png)

**Landing Wireframe Desktop 2**

![Landing Wireframe Desktop 2](assets/images/Landing_Desktop2.png)

**Landing Wireframe Desktop 3**

![Landing Wireframe Desktop 3](assets/images/Landing_Desktop3.png)

**Landing Wireframe Desktop 4**

![Landing Wireframe Desktop 4](assets/images/Landing_Desktop4.png)

**Landing Wireframe Desktop 5**

![Landing Wireframe Desktop 5](assets/images/Landing_Desktop5.png)

**Landing Wireframe Desktop 6**

![Landing Wireframe Desktop 6](assets/images/Landing_Desktop6.png)

**Landing Wireframe Desktop 7**

![Landing Wireframe Desktop 7](assets/images/Landing_Desktop7.png)

### Wireframes Mobile de la Landing Page

**Landing Wireframe Mobile 1**

![Landing Wireframe Mobile 1](assets/images/Landing_MobileW1.png)

**Landing Wireframe Mobile 2**

![Landing Wireframe Mobile 2](assets/images/Landing_MobileW2.png)

**Landing Wireframe Mobile 3**

![Landing Wireframe Mobile 3](assets/images/Landing_MobileW3.png)

**Landing Wireframe Mobile 4**

![Landing Wireframe Mobile 4](assets/images/Landing_MobileW4.png)

**Landing Wireframe Mobile 5**

![Landing Wireframe Mobile 5](assets/images/Landing_MobileW5.png)

**Landing Wireframe Mobile 6**

![Landing Wireframe Mobile 6](assets/images/Landing_MobileW6.png)

**Landing Wireframe Mobile 7**

![Landing Wireframe Mobile 7](assets/images/Landing_MobileW7.png)

**Link de figma:** [Ver en Figma](https://www.figma.com/design/gKyUHMHD9eKJ3KUjmugVd1/Landing-Page---AgroFlet?node-id=0-1&t=iTO54ThcvYOIGSXQ-1)

### 4.3.2. Landing Page Mock-up

El Mock-up de alta fidelidad integra el isotipo de AgroFlet, la paleta de colores oficial (Azul Marino y Verde AgroFlet) y tipografía Inter. Se evidencia la aplicación de atributos ARIA para accesibilidad (a11y) y selectores de idioma.

### Mockups Desktop de la Landing Page

**Landing Mockup Desktop 1**

![Landing Mockup Desktop 1](assets/images/Landing_DesktopM1.png)

**Landing Mockup Desktop 2**

![Landing Mockup Desktop 2](assets/images/Landing_DesktopM2.png)

**Landing Mockup Desktop 3**

![Landing Mockup Desktop 3](assets/images/Landing_DesktopM3.png)

**Landing Mockup Desktop 4**

![Landing Mockup Desktop 4](assets/images/Landing_DesktopM4.png)

**Landing Mockup Desktop 5**

![Landing Mockup Desktop 5](assets/images/Landing_DesktopM5.png)

**Landing Mockup Desktop 6**

![Landing Mockup Desktop 6](assets/images/Landing_DesktopM6.png)

**Landing Mockup Desktop 7**

![Landing Mockup Desktop 7](assets/images/Landing_DesktopM7.png)

### Mockups Mobile de la Landing Page

**Landing Mockup Mobile 1**

![Landing Mockup Mobile 1](assets/images/Landing_MobileM1.png)

**Landing Mockup Mobile 2**

![Landing Mockup Mobile 2](assets/images/Landing_MobileM2.png)

**Landing Mockup Mobile 3**

![Landing Mockup Mobile 3](assets/images/Landing_MobileM3.png)

**Landing Mockup Mobile 4**

![Landing Mockup Mobile 4](assets/images/Landing_MobileM4.png)

**Landing Mockup Mobile 5**

![Landing Mockup Mobile 5](assets/images/Landing_MobileM5.png)

**Landing Mockup Mobile 6**

![Landing Mockup Mobile 6](assets/images/Landing_MobileM6.png)

**Landing Mockup Mobile 7**

![Landing Mockup Mobile 7](assets/images/Landing_MobileM7.png)

**Link de figma:** [Ver en Figma](https://www.figma.com/design/gKyUHMHD9eKJ3KUjmugVd1/Landing-Page---AgroFlet?node-id=0-1&t=iTO54ThcvYOIGSXQ-1)

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
