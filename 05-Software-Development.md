# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

La Gestión de Configuración de Software (SCM) es la disciplina que permite identificar, controlar, versionar y auditar los distintos componentes de un sistema durante todo su ciclo de vida. Su aplicación asegura la trazabilidad de los cambios realizados sobre el código fuente, la documentación y los artefactos de diseño, reduciendo la probabilidad de errores de integración y facilitando el trabajo colaborativo del equipo.

En el caso de **AgroFlet**, la solución está compuesta por una Landing Page informativa, una Frontend Web Application y un RESTful API de elaboración interna. Durante el **Sprint 1** se priorizó la implementación, validación y despliegue de la primera versión de la **Landing Page**, desarrollada con HTML5, CSS3 y JavaScript (ES6+), manteniendo un comportamiento 100 % responsive y sin dependencias de frameworks externos.

### 5.1.1. Software Development Environment Configuration

A continuación se listan los productos de software utilizados por el equipo, organizados por tipo de actividad del ciclo de vida. Para cada herramienta se indica su propósito dentro de AgroFlet y la ruta de referencia o descarga.

**1. Project Management**

*Descripción:*

La gestión del proyecto permite organizar las actividades necesarias para alcanzar los objetivos del Sprint, asignar responsables, dar seguimiento al avance y mantener la comunicación entre los integrantes del equipo.


**Google Meet:**

Google Meet es la herramienta de videoconferencia empleada para las ceremonias formales de Scrum: Sprint Planning, Daily Meetings y Sprint Review. Permite la coordinación sincrónica del equipo y el registro audiovisual de las sesiones de revisión.

https://meet.google.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_GoogleMeet.png" alt="Google Meet" title="Google Meet" width="250">
</p>

**WhatsApp:**

Se emplean como canales de comunicación asincrónica para coordinar avances diarios, resolver bloqueos puntuales y notificar la apertura de Pull Requests pendientes de revisión.

https://whatsapp.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_whatsapp.png" alt="whatsapp" title="Whatsapp" width="250">
</p>

**2. Requirements Management**

**UXPressia:**

UXPressia se utiliza para la elaboración de los User Personas, Empathy Maps, Journey Maps e Impact Maps presentados en los capítulos anteriores, facilitando la identificación de necesidades de los segmentos objetivo (despachadores, transportistas y compradores mayoristas).

https://uxpressia.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_UXPressia.png" alt="UXPressia" title="UXPressia" width="250">
</p>

**Miro:**

Miro es la pizarra colaborativa utilizada para el Lean UX Canvas, el EventStorming y el diagrama de Arquitectura de la Información del Landing Page.

https://miro.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_Miro.png" alt="Miro" title="Miro" width="250">
</p>

**3. Product UX/UI Design**

**Figma:**

Figma es la herramienta de diseño colaborativo en la nube empleada para elaborar los wireframes, mockups y prototipos de la Landing Page y de la Web Application, así como para documentar el Design System de AgroFlet (paleta de marca y tipografía Inter). Los diseños allí definidos son la referencia directa de la implementación en HTML5 y CSS3.

https://www.figma.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_Figma.png" alt="Figma" title="Figma" width="250">
</p>

**Lucidchart:**

Lucidchart se utiliza para la elaboración de Wireflows, User Flows, diagramas UML y el Database Design de la solución.

https://www.lucidchart.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_Lucidchart.png" alt="Lucidchart" title="Lucidchart" width="250">
</p>

**Structurizr:**

Structurizr se utiliza para la elaboración de los diagramas de arquitectura de software bajo el modelo C4 (Context, Container y Component Level Diagrams) presentados en el Capítulo IV.

https://structurizr.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_Structurizr.png" alt="Structurizr" title="Structurizr" width="250">
</p>

**4. Software Development**

**Visual Studio Code:**

Visual Studio Code es el editor principal del equipo. Se utiliza para desarrollar los archivos `index.html`, `styles.css`, `app.js` y los diccionarios de internacionalización del proyecto. La configuración de formato se estandariza mediante el archivo `.editorconfig` incluido en la raíz del repositorio.

https://code.visualstudio.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_VSCode.jpg" alt="Visual Studio Code" title="Visual Studio Code" width="250">
</p>

**HTML5 / CSS3 / JavaScript (ES6+):**

Constituyen las tecnologías base de la Landing Page desplegada en el Sprint 1. HTML5 aporta la estructura semántica y accesible; CSS3 implementa el sistema de diseño mediante Custom Properties, CSS Grid y Flexbox bajo un enfoque Mobile-First; y JavaScript aporta la interactividad del lado del cliente sin dependencias externas.

<p align="center">
  <img src="assets/images/Cap5_Logo_HTML_CSS_JS.png" alt="HTML5 CSS3 JavaScript" title="HTML5 / CSS3 / JavaScript" width="250">
</p>

**Vue.js:**

Vue.js es el framework de JavaScript seleccionado para el desarrollo de la Frontend Web Application (dashboard de monitoreo). Su implementación está planificada para los siguientes Sprints.

https://vuejs.org/

<p align="center">
  <img src="assets/images/Cap5_Logo_VueJS.png" alt="Vue.js" title="Vue.js" width="250">
</p>

**PrimeVue:**

PrimeVue es la biblioteca de componentes de interfaz para Vue.js con la que se implementarán las Data Tables, formularios y componentes de navegación del dashboard, de acuerdo con el diseño definido en el Capítulo IV.

https://primevue.org/

<p align="center">
  <img src="assets/images/Cap5_Logo_PrimeVue.png" alt="PrimeVue" title="PrimeVue" width="250">
</p>

**ASP.NET Core:**

ASP.NET Core es el framework utilizado para el desarrollo del RESTful API de AgroFlet, responsable de la lógica de negocio de los bounded contexts *Fleet Management*, *Shipment Tracking* e *Identity and Access Management*.

https://dotnet.microsoft.com/apps/aspnet

<p align="center">
  <img src="assets/images/Cap5_Logo_AspNetCore.png" alt="ASP.NET Core" title="ASP.NET Core" width="250">
</p>

**C#:**

C# es el lenguaje de programación empleado en la implementación de los Web Services mediante ASP.NET Core y Entity Framework Core.

https://dotnet.microsoft.com/languages/csharp

<p align="center">
  <img src="assets/images/Cap5_Logo_CSharp.png" alt="C#" title="C#" width="250">
</p>

**Entity Framework Core:**

Entity Framework Core es el ORM utilizado para la persistencia de usuarios, unidades de transporte, operaciones e incidencias desde el RESTful API hacia la base de datos relacional.

https://learn.microsoft.com/ef/core/

<p align="center">
  <img src="assets/images/Cap5_Logo_EFCore.png" alt="Entity Framework Core" title="Entity Framework Core" width="250">
</p>

**MySQL Server:**

MySQL es el sistema de gestión de base de datos relacional (RDBMS) definido en el Container Level Diagram del modelo C4 para almacenar la información operativa de la plataforma.

https://www.mysql.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_MySQL.jpg" alt="MySQL Server" title="MySQL Server" width="250">
</p>

**Git:**

Git es el sistema de control de versiones distribuido utilizado localmente por cada integrante para registrar cambios, crear ramas y sincronizar el código fuente con el repositorio remoto.

https://git-scm.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_Git.png" alt="Git" title="Git" width="250">
</p>

**GitHub:**

GitHub es la plataforma de colaboración donde se alojan los repositorios del proyecto. Sobre ella se aplican el flujo GitFlow, las revisiones mediante Pull Requests y el registro de contribuciones por integrante.

https://github.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_GitHub.jpg" alt="GitHub" title="GitHub" width="250">
</p>

**5. Software Deployment**

**GitHub Pages:**

GitHub Pages es el servicio de hosting estático utilizado para publicar la versión `v1.0.0` de la Landing Page de AgroFlet directamente desde la rama `main` del repositorio. El archivo `.nojekyll` incluido en la raíz del proyecto deshabilita el procesamiento por Jekyll y garantiza la carga correcta de los directorios de assets.

https://pages.github.com/

<p align="center">
  <img src="assets/images/Cap5_Logo_GitHubPages.jpg" alt="GitHub Pages" title="GitHub Pages" width="250">
</p>

**Proveedor de hosting en la nube para ASP.NET Core:**

Para el despliegue del RESTful API se utilizará un proveedor de hosting en la nube compatible con ASP.NET Core y MySQL. El proveedor definitivo se determinará en función de los requerimientos de disponibilidad y costo del proyecto.

<p align="center">
  <img src="assets/images/Cap5_Logo_CloudHosting.png" alt="Cloud Hosting" title="Cloud Hosting Provider" width="250">
</p>

**6. Software Documentation**

**Markdown + Visual Studio Code:**

Markdown es el formato utilizado para la elaboración del `README.md` del repositorio y de los capítulos del Project Report. Visual Studio Code permite editar y previsualizar dichos archivos antes de publicarlos en GitHub.

<p align="center">
  <img src="assets/images/Cap5_Logo_Markdown.png" alt="Markdown" title="Markdown + Visual Studio Code" width="250">
</p>

**Swagger / OpenAPI:**

Swagger se utilizará para documentar los endpoints del RESTful API mediante la especificación OpenAPI, permitiendo visualizar e interactuar con los servicios desde una interfaz web. Su uso corresponde a los Sprints en los que se implemente el backend.

https://swagger.io/

<p align="center">
  <img src="assets/images/Cap5_Logo_Swagger.jpg" alt="Swagger / OpenAPI" title="Swagger / OpenAPI" width="250">
</p>

El entorno seleccionado permite mantener coherencia entre el diseño elaborado en Figma y la implementación web desarrollada por el equipo: Visual Studio Code, Live Server y Chrome DevTools facilitan la construcción y validación local del producto; Git y GitHub aseguran la trazabilidad de los cambios; GitHub Pages permite publicar la solución; y la combinación de Gherkin y Cucumber documenta y ejecuta las pruebas de aceptación asociadas a los requerimientos funcionales.

---

### 5.1.2. Source Code Management

La administración del código fuente es un pilar del trabajo colaborativo del equipo. En este apartado se define el modelo organizativo y de control de versiones aplicado mediante GitHub y el flujo de trabajo GitFlow, junto con las convenciones de nombrado de ramas, estructura de mensajes de commit y versionado semántico de los lanzamientos.

**1. Establecimiento de repositorios en GitHub**

La solución distribuida de AgroFlet se organiza en repositorios independientes, separando las responsabilidades de cada producto:

*Landing Page:* repositorio dedicado al sitio web informativo y promocional del producto. Contiene la totalidad de los recursos estáticos (HTML5, CSS3, JavaScript, diccionarios de internacionalización e imágenes) orientados a comunicar la propuesta de valor de AgroFlet a los segmentos objetivo. En este mismo repositorio se alojarán los archivos `.feature` de las pruebas de aceptación asociadas al landing.

*Frontend Web Application:* repositorio destinado a la aplicación web del lado del cliente desarrollada con Vue.js y PrimeVue. Contiene las vistas, componentes y la lógica de consumo del RESTful API.

*Web Services:* repositorio que aloja la lógica del backend implementada con ASP.NET Core y Entity Framework Core, incluyendo las pruebas unitarias, de integración y de aceptación.

*Project Report:* repositorio destinado a la redacción y versionamiento de los capítulos del informe del proyecto en formato Markdown.

**Enlaces a los repositorios:**

* Repositorio de Landing Page: `[https://github.com/<organizacion>/agroflet-landing-page]`
* Repositorio de Frontend Web Application: Disponible en futuras entregas
* Repositorio de Web Services: Disponible en futuras entregas
* Repositorio del Project Report: `[https://github.com/<organizacion>/agroflet-project-report]`

**2. Estructura del repositorio de la Landing Page**

La organización de directorios sigue una arquitectura modular y desacoplada, separando estilos, scripts, diccionarios de idioma y recursos gráficos:

```text
agroflet-landing-page/
├── assets/
│   ├── css/
│   │   └── styles.css              # Design tokens, layouts y componentes
│   ├── i18n/
│   │   ├── es.json                 # Diccionario de traducción en español
│   │   └── en.json                 # Diccionario de traducción en inglés
│   ├── js/
│   │   └── app.js                  # Interactividad, validaciones, i18n y carrusel
│   └── images/
│       ├── logo.jpg                # Identidad visual oficial
│       └── team/                   # Fotografías de los integrantes
│           ├── adriano.jpg
│           ├── bernie.png
│           ├── cesar.jpg
│           ├── christoper.jpeg
│           └── jose.png
├── docs/
│   └── Terms-and-conditions.html   # Términos y condiciones del servicio
├── .editorconfig                   # Formato consistente entre editores
├── .gitignore                      # Exclusión de archivos temporales
├── .nojekyll                       # Compatibilidad con GitHub Pages
├── index.html                      # Landing Page principal
├── LICENSE                         # Licencia MIT
└── README.md                       # Documentación técnica del repositorio
```



**3. Workflow de control de versiones (GitFlow)**

Para gestionar la integración de nuevas características y coordinar los cambios del equipo se emplea el modelo **GitFlow**, que define ramas con propósitos estrictos y permite el desarrollo en paralelo sin afectar la estabilidad del producto publicado.

| Nombre de la rama | Descripción |
| --- | --- |
| **Main Branch** (`main`) | Rama base que refleja el estado de producción. Solo recibe código validado y aprobado para despliegue. Es la rama publicada por GitHub Pages. |
| **Develop Branch** (`develop`) | Rama de integración del equipo. Unifica el código de las funcionalidades en curso antes de preparar un lanzamiento. |
| **Feature Branches** (`feature/*`) | Ramas temporales creadas desde `develop` para desarrollar funcionalidades de forma aislada. <br> **Convención:** `feature/nombre-de-la-funcionalidad` |
| **Release Branches** (`release/*`) | Ramas de estabilización previas al pase a producción: pruebas finales, documentación y corrección de fallos menores. <br> **Convención:** `release/vX.Y.Z` |
| **Hotfix Branches** (`hotfix/*`) | Ramas de emergencia creadas desde `main` para corregir fallos críticos en producción. Se fusionan en `main` y en `develop`. <br> **Convención:** `hotfix/descripcion-del-parche` |

*Ramas utilizadas durante el Sprint 1:*

```text
feature/header-navigation
feature/hero-section
feature/plans-section
feature/testimonials-carousel
feature/solve-section
feature/team-section
feature/videos-section
feature/auth-modal
feature/i18n
feature/footer-legal
feature/responsive-layout
release/v1.0.0
```

Las funcionalidades desarrolladas en ramas `feature/*` se integran a `develop` mediante Pull Requests con al menos una revisión cruzada (Code Review). Una vez validado el Sprint, la versión se estabiliza en una rama `release/*` y posteriormente se fusiona en `main`, lo que dispara la publicación automática en GitHub Pages.

**4. Versionado Semántico (Semantic Versioning 2.0.0)**

AgroFlet adopta el estándar **Semantic Versioning 2.0.0** bajo el formato `MAJOR.MINOR.PATCH`:

* **Major:** cambios profundos que rompen la compatibilidad con versiones anteriores.
* **Minor:** incorporación de nuevas funcionalidades manteniendo la compatibilidad.
* **Patch:** correcciones de errores o mejoras que no alteran la funcionalidad general.

Ejemplos de aplicación en el proyecto:

* `v1.0.0`: primera versión desplegada de la Landing Page (Sprint 1).
* `v1.1.0`: incorporación del formulario de contacto y nuevas secciones informativas.
* `v1.0.1`: corrección de comportamiento del menú responsive en dispositivos móviles.

**5. Convenciones de mensajes de commit (Conventional Commits)**

Todos los mensajes de commit siguen la especificación **Conventional Commits**, redactados en inglés e iniciados con un prefijo que indica la naturaleza del cambio:

* `feat:` incorpora una funcionalidad nueva (ej. `feat: implement testimonials carousel`).
* `fix:` corrige un error o comportamiento anómalo (ej. `fix: correct mobile navigation behavior`).
* `docs:` modifica exclusivamente documentación (ej. `docs: update landing page README`).
* `style:` aplica ajustes de formato o estilos sin alterar la lógica (ej. `style: improve responsive card layout`).
* `refactor:` reestructura código existente sin añadir funcionalidades ni corregir errores.
* `test:` agrega o corrige pruebas (ej. `test: add gherkin scenarios for landing navigation`).
* `chore:` tareas de mantenimiento y configuración (ej. `chore: add .nojekyll for GitHub Pages`).

---

### 5.1.3. Source Code Style Guide & Coding Conventions

En esta sección se definen las normativas de codificación aplicadas al desarrollo de la solución, con el objetivo de estandarizar la escritura de HTML, CSS, JavaScript y C#, asegurando código legible, mantenible y escalable.

Como regla transversal, **toda la nomenclatura técnica (identificadores, clases, variables, funciones, métodos y comentarios) se redacta exclusivamente en inglés**. El equipo se alinea con las siguientes guías de la industria:

* HTML Style Guide and Coding Conventions (W3Schools)
* Google HTML/CSS Style Guide
* Google JavaScript Style Guide
* MDN JavaScript Guidelines
* BEM Methodology (Block, Element, Modifier)
* C# Coding Conventions (Microsoft)
* Microsoft ASP.NET Core Coding Guidelines

**Principios transversales**

* **Idioma:** todo el nombrado técnico y la documentación interna se redactan en inglés.
* **DRY (Don't Repeat Yourself):** se evita la duplicidad mediante clases reutilizables y variables CSS centralizadas.
* **KISS (Keep It Simple, Stupid):** se prioriza la simplicidad y claridad de la lógica.
* **Indentación:** consistente y estandarizada mediante el archivo `.editorconfig` (2 espacios, UTF-8, LF, eliminación de espacios finales).

---

**HTML**

Se utiliza HTML5 para definir la estructura semántica y accesible de la Landing Page.

*Convenciones de formato y estructura:*

* **Indentación:** 2 espacios por nivel; no se utilizan tabulaciones.
* **Etiquetas y atributos:** siempre en minúsculas (ej. `<section>`, `<article>`).
* **Comillas:** dobles para todos los valores de atributos (ej. `class="container"`).
* **Documento base:** declaración `<!DOCTYPE html>` en la primera línea y atributo de idioma `<html lang="es">`.
* **Semántica:** uso prioritario de `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>` sobre el uso indiscriminado de `<div>`.
* **Nomenclatura:** identificadores y clases redactados en inglés (`#hero`, `#plans`, `#testimonials`, `#what-we-solve`, `#team`, `#videos`).
* **Accesibilidad:** atributo `alt` obligatorio en imágenes informativas y `aria-label` en controles cuyo propósito no resulta evidente (ej. `aria-label="Cambiar idioma"`, `aria-label="Abrir menú"`, `aria-expanded`).
* **Internacionalización:** los nodos traducibles se marcan mediante el atributo `data-i18n`, lo que permite actualizar el contenido sin recargar la página.

Ejemplo aplicado en el proyecto:

```html
<section id="testimonials" class="testimonials section section--dark">
  <div class="container">
    <div class="section__header">
      <span class="section__tag" data-i18n="testimonials.tag">Testimonios</span>
      <h2 class="section__title" data-i18n="testimonials.title">Lo que dicen nuestros usuarios</h2>
    </div>
  </div>
</section>
```

<p align="center">
  <img src="assets/images/Cap5_Convenciones_HTML.png" alt="Convenciones HTML aplicadas en index.html" title="HTML Conventions" width="700">
</p>

---

**CSS**

Se utiliza CSS3 puro para controlar la presentación visual, bajo un enfoque modular y responsivo (Mobile-First).

*Convenciones de formato y arquitectura:*

* **Indentación:** 2 espacios por nivel.
* **Sintaxis:** espacio antes de la llave de apertura `{`, llave de cierre `}` en una línea propia y cada declaración terminada en punto y coma `;`.
* **Nomenclatura BEM:** clases escritas como bloque, elemento y modificador (`.plan-card`, `.plan-card__title`, `.plan-card--featured`; `.header`, `.header__nav`, `.header__logo`).
* **Design Tokens:** las variables globales de marca se centralizan en `:root` mediante Custom Properties.
* **Orden de propiedades:** posicionamiento, modelo de caja, tipografía, aspecto visual y animaciones.
* **Especificidad:** se evita anidar selectores más de tres niveles y se restringe el uso de `!important`.
* **Responsive:** media queries incrementales con puntos de corte en `768px` y `1024px`, más ajustes específicos en `max-width: 767px` y `480px`.
* **Accesibilidad:** se respeta la preferencia del sistema mediante `@media (prefers-reduced-motion: reduce)`.

Ejemplo aplicado en el proyecto:

```css
:root {
  /* Brand Colors */
  --green:        #27AE60;
  --navy:         #0B3B60;
  --orange:       #F39C12;
  --font-family:  'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
}

.plan-card {}
.plan-card__title {}
.plan-card--featured {}
```

<p align="center">
  <img src="assets/images/Cap5_Convenciones_CSS.png" alt="Design tokens y nomenclatura BEM en styles.css" title="CSS Conventions" width="700">
</p>

---

**JavaScript**

Se aplica JavaScript moderno (ECMAScript ES6+) para la interactividad del lado del cliente, sin frameworks ni dependencias externas.

*Convenciones de formato y nomenclatura:*

* **Indentación:** 2 espacios.
* **Modo estricto:** el código se ejecuta dentro de `'use strict';` y se inicializa con `document.addEventListener('DOMContentLoaded', ...)`.
* **Nomenclatura:** `camelCase` para variables y funciones (`setLanguage`, `openAuthModal`, `saveUserSession`, `clearUserSession`); `PascalCase` para clases y componentes; `UPPER_SNAKE_CASE` para constantes globales.
* **Declaración de variables:** `const` por defecto, `let` únicamente para variables reasignables; se prohíbe `var`.
* **Igualdad estricta:** uso obligatorio de `===` y `!==`.
* **Manejo de eventos:** exclusivamente mediante `addEventListener`, evitando atributos de evento en el HTML.
* **Organización:** el archivo se estructura en bloques lógicos numerados y comentados (internacionalización, scroll del header, menú móvil, partículas del hero, contadores, carrusel de testimonios, modales, validaciones y sesión).
* **APIs del navegador:** uso de `IntersectionObserver` para animaciones al hacer scroll y de `localStorage` para persistir preferencias de idioma y la sesión demostrativa.

Ejemplos de funciones implementadas:

```javascript
setLanguage(lang);
openAuthModal(mode, preselectedPlan);
closeAuthModal();
saveUserSession(userData);
clearUserSession();
validateEmail(email);
getPasswordStrength(password);
```

<p align="center">
  <img src="assets/images/Cap5_Convenciones_JS.png" alt="Convenciones JavaScript aplicadas en app.js" title="JavaScript Conventions" width="700">
</p>

---

**C# (.NET Core)**

Estas convenciones se aplicarán durante la implementación del RESTful API en los siguientes Sprints, siguiendo las guías oficiales de Microsoft.

*Convenciones de formato y nomenclatura:*

* **Indentación:** 4 espacios.
* **Llaves:** estilo Allman (cada llave en su propia línea).
* **Nomenclatura:** `PascalCase` para clases, métodos y propiedades públicas (`ShipmentsController`, `GetActiveShipments`); prefijo `I` para interfaces (`IShipmentRepository`); `camelCase` para parámetros y variables locales; guion bajo inicial para campos privados (`_dbContext`).
* **Longitud de línea:** máximo 120 caracteres.
* **Inyección de dependencias:** servicios y repositorios inyectados por constructor, evitando instanciaciones directas de lógica de negocio.
* **Controladores ligeros:** la lógica de negocio se delega a la capa de Services.
* **Asincronismo:** los métodos de acceso a datos o I/O son asíncronos y llevan el sufijo `Async` (`GetShipmentByIdAsync`).
* **LINQ:** uso de métodos de extensión para manipular colecciones de forma declarativa.

> Durante el Sprint 1 no se ha implementado código C#, por lo que esta sección constituye la definición normativa que regirá el desarrollo del RESTful API en los Sprints posteriores.

---

### 5.1.4. Software Deployment Configuration

En esta sección se detalla el proceso de configuración y despliegue definido para los productos que componen la solución de AgroFlet.

**1. Landing Page (GitHub Pages)**

* **Plataforma de hosting:** GitHub Pages.
* **Origen del despliegue:** contenido estático de la rama `main` del repositorio de la Landing Page, directorio raíz (`/root`).
* **Archivo de compatibilidad:** `.nojekyll` en la raíz del proyecto, que evita el procesamiento del sitio por Jekyll y garantiza la carga correcta de `assets/`.

*Procedimiento de despliegue aplicado:*

1. Integrar los cambios aprobados de las ramas `feature/*` hacia `develop` mediante Pull Requests con revisión cruzada.
2. Crear la rama `release/v1.0.0` a partir de `develop`.
3. Validar localmente la versión mediante Live Server y Chrome DevTools (desktop y responsive).
4. Integrar la rama de release en `main`.
5. Crear el tag correspondiente según Semantic Versioning (`v1.0.0`).
6. Ingresar a `Settings > Pages` en el repositorio de GitHub.
7. Seleccionar la opción `Deploy from a branch`.
8. Seleccionar la rama `main`.
9. Seleccionar la carpeta `/root` como directorio de origen.
10. Guardar la configuración y esperar la ejecución del workflow de publicación.
11. Validar la URL pública generada, verificando la carga de estilos, scripts, imágenes, el cambio de idioma y el enlace a `docs/Terms-and-conditions.html`.

* **Repositorio:** `[https://github.com/AGROFLET/Agroflet-landing-page]`
* **Versión desplegada:** `v1.0.0`
* **URL de producción:** `[https://agroflet.github.io/Agroflet-landing-page/]`

**Evidencia de la configuración:**

<p align="center">
  <img src="assets/images/Cap5_Deploy_GitHubPages_Config.png" alt="Configuración de GitHub Pages" title="Settings > Pages" width="700">
</p>

<p align="center">
  <img src="assets/images/Cap5_Deploy_Workflow.png" alt="Workflow de despliegue ejecutado" title="GitHub Actions - pages build and deployment" width="700">
</p>

**2. Frontend Web Application**

* **Tecnología:** Vue.js + PrimeVue.
* **Proceso previsto:** integración de ramas `feature/*` hacia `develop` mediante Pull Requests; al fusionar en `main` se ejecuta el proceso de construcción (`npm install` y `npm run build`), se inyectan las variables de entorno de producción (URL base del API) y se publica el directorio `dist/` resultante.
* **Estado actual:** pendiente de implementación. Planificado para los siguientes Sprints.

**3. Web Services (RESTful API)**

* **Tecnología:** ASP.NET Core, C# y Entity Framework Core sobre MySQL.
* **Proceso previsto:** los Pull Requests hacia `develop` deben aprobar las pruebas unitarias y de integración; tras la fusión en `main`, el proyecto se compila con `dotnet publish -c Release` y el artefacto se despliega en el proveedor de nube seleccionado, configurando de forma segura la cadena de conexión y las claves de los tokens JWT. La documentación de endpoints queda expuesta mediante Swagger/OpenAPI.
* **Estado actual:** pendiente de implementación. Planificado para los siguientes Sprints.

---

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1

Durante el Sprint 1 el equipo se concentró en la implementación y despliegue de la primera versión funcional y responsive de la Landing Page de AgroFlet, así como en la elaboración de la documentación técnica del repositorio.

#### 5.2.1.1. Sprint Planning 1

| Sprint # | Sprint 1 |
| :--- | :--- |
| **Sprint Planning Background** | |
| Date | 08/09/2026 |
| Time | 8:00 PM |
| Location | Google Meet (reunión virtual) |
| Prepared By | Alca Morán, César Alejandro |
| Attendees (to planning meeting) | Alca Morán, César Alejandro<br>Centeno León, Adriano Samir<br>Rivas Méndez, Bernie Aarón<br>Rivas Castillo, Christoper Steven<br>Tello Lima, Jose Alejandro |
| **Sprint 1 Review Summary** | Durante este primer ciclo el equipo consolidó los artefactos de UX definidos en los capítulos anteriores (User Personas, Journey Maps, Arquitectura de la Información, wireframes y mockups) y los tradujo en una implementación web funcional. Se desarrolló y desplegó la primera versión de la Landing Page de AgroFlet, la cual comunica la propuesta de valor orientada a la trazabilidad del transporte agrícola, presenta las funcionalidades proyectadas de la plataforma, los planes de suscripción, los testimonios de los segmentos objetivo, el equipo fundador y el contenido institucional. Se incorporaron navegación responsive, internacionalización español/inglés, carrusel interactivo de testimonios y modales demostrativos de registro e inicio de sesión. |
| **Sprint 1 Retrospective Summary** | El equipo evaluó positivamente la distribución del trabajo mediante ramas `feature/*`, que permitió desarrollar secciones de forma aislada y redujo los conflictos de integración sobre `index.html` y `styles.css`. Se identificó como principal aprendizaje la necesidad de mantener coherencia entre las funcionalidades descritas en el Project Report y aquellas efectivamente implementadas en el producto: la User Story UH28 (formulario de contacto) fue reprogramada para el Sprint 2 al no haberse implementado un `<form>` de contacto en esta versión, manteniéndose únicamente los canales de contacto en el footer. Como oportunidad de mejora se acordó unificar la carga de los diccionarios de internacionalización desde `assets/i18n/` y afinar la estimación de los puntos de historia. |
| **Sprint Goal & User Stories** | |
| **Sprint 1 Goal** | *Our focus is on* publicar la primera versión funcional y responsive de la Landing Page de AgroFlet, que comunica la propuesta de valor del producto, sus funcionalidades proyectadas, los planes de suscripción, el equipo y el contenido institucional, con navegación responsive e internacionalización español/inglés.<br>*We believe it delivers* a los productores agrícolas, transportistas fletistas y compradores mayoristas una comprensión clara y accesible de la solución y del plan de suscripción que les corresponde, sin necesidad de contacto previo con el equipo comercial.<br>*This will be confirmed when* un visitante puede, desde la URL pública de producción y en cualquiera de los dos idiomas, recorrer las secciones mediante el menú, comparar los tres planes y llegar al llamado a la acción de su segmento en no más de tres interacciones, tanto en navegador de escritorio como en dispositivo móvil. |
| **Sprint 1 Velocity** | 24 |
| **Sum of Story Points** | 24 |

**Nota:** Cuadro resumen que detalla la planificación, las metas establecidas, los resultados obtenidos y las métricas de esfuerzo correspondientes al Sprint 1 de AgroFlet.

#### 5.2.1.2. Aspect Leaders and Collaborators

| Team Member | GitHub Username | Landing Page (código) | Diseño UI/UX | Documentación | Deployment |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Alca Morán, César Alejandro | `almocesar` | Líder | Colaborador | Colaborador | Colaborador |
| Centeno León, Adriano Samir | `Adri11-dk` | Colaborador | Colaborador | Líder | Colaborador |
| Rivas Méndez, Bernie Aarón | `ARivas3008` | Colaborador | Líder | Colaborador | Colaborador |
| Rivas Castillo, Christoper Steven | `C0DERTOPH` | Colaborador | Colaborador | Colaborador | Colaborador |
| Tello Lima, Jose Alejandro | `j4ndrow` | Colaborador | Colaborador | Colaborador | Líder |

**Distribución por aspecto técnico del Sprint 1:**

| Aspecto | Líder | Colaboradores |
| :--- | :--- | :--- |
| Landing Page UX/UI | Rivas Méndez, Bernie Aarón | Tello Lima, Jose Alejandro / Alca Morán, César Alejandro |
| HTML Structure & Semántica | Alca Morán, César Alejandro | Centeno León, Adriano Samir / Rivas Castillo, Christoper Steven |
| CSS & Responsive Design | Rivas Méndez, Bernie Aarón | Alca Morán, César Alejandro / Rivas Castillo, Christoper Steven |
| JavaScript Interactions | Rivas Castillo, Christoper Steven | Alca Morán, César Alejandro / Centeno León, Adriano Samir |
| Internationalization (i18n) | Centeno León, Adriano Samir | Rivas Castillo, Christoper Steven / Tello Lima, Jose Alejandro |
| Documentation (README & Report) | Centeno León, Adriano Samir | Tello Lima, Jose Alejandro / Rivas Méndez, Bernie Aarón |
| Deployment (GitHub Pages) | Tello Lima, Jose Alejandro | Alca Morán, César Alejandro / Centeno León, Adriano Samir |

**Nota:** Distribución de responsabilidades durante el Sprint 1, indicando el liderazgo y la colaboración en las principales áreas de trabajo. Los usuarios de GitHub consignados deben coincidir con las cuentas registradas como Contributors del repositorio.

#### 5.2.1.3. Sprint Backlog 1

| User Story Id | User Story Title | Work Item / Task Id | Work Item / Task Title | Description | Estimation (h) | Assigned To | Status |
| :--- | :--- | :--- | :--- | :--- | :---: | :--- | :---: |
| UH24 | Visualización de la propuesta de valor en el landing page | T01 | Estructuración base en HTML5 e implementación del Hero | Creación del esqueleto semántico del documento (`header`, `main`, `section`, `footer`) e implementación de la sección principal con el nombre de la plataforma, el titular de propuesta de valor, contadores estadísticos animados y llamados a la acción diferenciados. | 4 | Alca Morán, César Alejandro | Finalizada |
| UH25 | Consulta de funcionalidades principales desde el landing page | T02 | Implementación de la sección informativa de funcionalidades | Maquetación de la grilla de tarjetas de la sección "La App", con seis funcionalidades clave, ícono SVG representativo y descripción breve para cada una. | 3 | Rivas Castillo, Christoper Steven | Finalizada |
| UH26 | Consulta de planes y precios en el landing page | T03 | Maquetación de la sección de planes de suscripción | Implementación de las tarjetas de los planes Básico, Estándar y Profesional, con unidades incluidas, funcionalidades habilitadas, cinta de plan destacado y botón de llamado a la acción por segmento. | 3 | Rivas Méndez, Bernie Aarón | Finalizada |
| UH27 | Consulta de testimonios de usuarios en el landing page | T04 | Desarrollo del carrusel interactivo de testimonios | Implementación del carrusel con cinco testimonios (nombre, rol y procedencia), navegación circular, indicadores, rotación automática con pausa en interacción y soporte de gestos táctiles y arrastre con mouse. | 4 | Rivas Castillo, Christoper Steven | Finalizada |
| UH29 | Navegación fluida entre secciones del landing page | T05 | Implementación de navegación responsive y scroll suave | Desarrollo del header fijo con cambio de estado al hacer scroll, resaltado del ítem activo, menú hamburguesa para dispositivos móviles y desplazamiento suave mediante anchors sin recargar la página. | 3 | Alca Morán, César Alejandro | Finalizada |
| UH30 | Visualización del landing page en múltiples idiomas | T06 | Implementación del sistema de internacionalización ES/EN | Integración de los diccionarios de traducción y del selector de idioma del encabezado, actualización dinámica de todos los nodos marcados con `data-i18n` (incluidos placeholders y mensajes de validación) y persistencia de la preferencia en `localStorage`. | 4 | Centeno León, Adriano Samir | Finalizada |
| UH24 | Visualización de la propuesta de valor en el landing page | T07 | Configuración del diseño responsive (Mobile-First) | Definición de los design tokens en `:root` y de las media queries en 480 px, 768 px y 1024 px para garantizar la correcta visualización en smartphones, tablets y escritorio. | 3 | Rivas Méndez, Bernie Aarón | Finalizada |
| UH24 | Visualización de la propuesta de valor en el landing page | T08 | Desarrollo de la sección del equipo y sección de videos | Implementación de las tarjetas de perfil de los cinco integrantes del equipo fundador y de las tarjetas de acceso a los videos institucionales mediante modal con reproducción embebida. | 2 | Tello Lima, Jose Alejandro | Finalizada |
| UH24 | Visualización de la propuesta de valor en el landing page | T09 | Implementación del footer institucional y documento legal | Desarrollo del pie de página con enlaces de navegación, canales de contacto y accesos legales, e implementación del documento de Términos y Condiciones en `docs/Terms-and-conditions.html`. | 2 | Centeno León, Adriano Samir | Finalizada |
| UH24 | Visualización de la propuesta de valor en el landing page | T10 | Despliegue de la versión v1.0.0 en GitHub Pages | Configuración del repositorio, creación del archivo `.nojekyll`, habilitación de GitHub Pages desde la rama `main` y validación de la URL pública de producción. | 2 | Tello Lima, Jose Alejandro | Finalizada |
| UH28 | Envío de mensaje de contacto desde el landing page | T11 | Implementación del formulario de contacto | Desarrollo de un formulario de contacto con validación de campos obligatorios y confirmación de envío. | 3 | Rivas Méndez, Bernie Aarón | Finalizada |

**Nota:** Tabla que vincula las User Stories del EPIC-09 abordadas durante el Sprint 1 con sus respectivas tareas técnicas, el esfuerzo estimado en horas, el responsable asignado y el estado de cada asignación. La tarea T11, asociada a la User Story UH28, se mantiene en estado *In Process* y se reprograma para el Sprint 2, dado que la versión `v1.0.0` de la Landing Page expone los canales de contacto en el footer pero aún no incorpora un formulario de contacto.

#### 5.2.1.4. Development Evidence for Sprint Review

Esta sección expone la evidencia técnica del progreso alcanzado durante el Sprint con relación a los productos definidos en el alcance. Durante el Sprint 1 se implementó la primera versión funcional de la Landing Page de AgroFlet utilizando HTML5, CSS3 y JavaScript (ES6+), sin frameworks ni dependencias externas.

Las principales funcionalidades desarrolladas incluyen:

* navegación responsive con header fijo, resaltado de sección activa y menú hamburguesa;
* sección principal (Hero) con propuesta de valor, contadores estadísticos animados y sistema de partículas optimizado;
* sección de planes de suscripción (Básico, Estándar y Profesional);
* carrusel interactivo de testimonios con soporte táctil, arrastre y rotación automática;
* sección informativa de funcionalidades proyectadas de la plataforma;
* presentación del equipo fundador;
* sección de videos con modal de reproducción embebida y corte automático al cerrar;
* internacionalización español/inglés con persistencia en `localStorage`;
* formularios demostrativos de registro e inicio de sesión con validación en tiempo real e indicador de fortaleza de contraseña;
* modales informativos de Términos de Uso, Política de Privacidad y Preguntas Frecuentes;
* sistema de notificaciones tipo *toast*;
* diseño adaptable para escritorio, tablet y dispositivos móviles.

> La autenticación incluida en esta versión es exclusivamente demostrativa: se ejecuta en el cliente mediante JavaScript y `localStorage`, y no se encuentra integrada con el RESTful API de AgroFlet.

**Registro de commits del Sprint 1:**

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| agroflet-landing-page | `feature/header-navigation` | `77a83d2` | feat: implement responsive header and navigation | Added fixed header, scroll state, active section tracking and mobile burger menu. | `17/09/2026` |
| agroflet-landing-page | `feature/hero-section` | `690c3cc` | feat: implement hero section with animated counters | Added value proposition hero, animated statistics counters and particle background. | `17/09/2026` |
| agroflet-landing-page | `feature/plans-section` | `3d602c7` | feat: add subscription plans section | Implemented Basic, Standard and Professional plan cards with segmented call to action. | `17/09/2026` |
| agroflet-landing-page | `feature/testimonials-carousel` | `8a42a8c` | feat: add testimonials carousel | Implemented touch and drag enabled carousel with auto rotation and dot indicators. | `17/09/2026` |
| agroflet-landing-page | `feature/solve-section` | `487b350` | feat: implement platform features section | Added responsive grid with six key platform features and SVG icons. | `17/09/2026` |
| agroflet-landing-page | `feature/team-section` | `e1f9f0d` | feat: create team and videos presentation | Added founding team profile cards and institutional video modal. | `17/09/2026` |
| agroflet-landing-page | `feature/auth-modal` | `3b97e89` | feat: implement demo authentication modal | Added sign up and sign in forms with live validation and password strength indicator. | `17/09/2026` |
| agroflet-landing-page | `feature/i18n` | `5f2486c` | feat: implement bilingual landing page | Added ES/EN dictionaries, language toggle and localStorage persistence. | `17/09/2026` |
| agroflet-landing-page | `feature/footer-legal` | `fe83b67` | feat: add footer and terms and conditions page | Implemented institutional footer and legal document under docs directory. | `17/09/2026` |
| agroflet-landing-page | `feature/responsive-layout` | `c4cc20d` | style: improve responsive card layout | Adjusted design tokens and media queries for mobile, tablet and desktop breakpoints. | `18/09/2026` |
| agroflet-landing-page | `develop` | `a7677c2` | docs: update landing page documentation | Updated README with project structure, features and local execution instructions. | `18/09/2026` |
| agroflet-landing-page | `main` | `fc13b72` | chore: prepare release v1.0.0 and trigger deployment | Merged release branch and triggered GitHub Pages deployment. | `18/09/2026` |


**Evidencia del código HTML:**

<p align="center">
  <img src="assets/images/Cap5_Dev_HTML.png" alt="Evidencia del código HTML de la Landing Page" title="Development Evidence - HTML5" width="700">
</p>

**Evidencia de los estilos CSS:**

<p align="center">
  <img src="assets/images/Cap5_Dev_CSS.png" alt="Evidencia del código CSS de la Landing Page" title="Development Evidence - CSS3" width="700">
</p>

**Evidencia del código JavaScript:**

<p align="center">
  <img src="assets/images/Cap5_Dev_JS.png" alt="Evidencia del código JavaScript de la Landing Page" title="Development Evidence - JavaScript" width="700">
</p>

**Evidencia de los diccionarios de internacionalización:**

<p align="center">
  <img src="assets/images/Cap5_Dev_i18n.png" alt="Diccionarios de internacionalización es.json y en.json" title="Development Evidence - i18n" width="700">
</p>

**Evidencia de commits y Pull Requests en GitHub:**

<p align="center">
  <img src="assets/images/Cap5_Dev_Commits.png" alt="Historial de commits del repositorio" title="Development Evidence - Commits" width="700">
</p>

<p align="center">
  <img src="assets/images/Cap5_Dev_PullRequests.png" alt="Pull Requests del Sprint 1" title="Development Evidence - Pull Requests" width="700">
</p>

#### 5.2.1.5. Execution Evidence for Sprint Review

Se verificó la ejecución de la Landing Page de AgroFlet en navegador de escritorio y mediante las herramientas responsive de Google Chrome DevTools, validando los siguientes comportamientos:

* navegación mediante anchors con desplazamiento suave y resaltado de la sección activa;
* apertura y cierre del menú responsive en dispositivos móviles;
* adaptación del contenido en resoluciones de escritorio, tablet y smartphone;
* cambio de idioma español/inglés sin recarga de página y persistencia de la preferencia;
* funcionamiento del carrusel de testimonios mediante botones, indicadores, gestos táctiles y arrastre;
* apertura de los modales de registro, inicio de sesión, video y documentos legales;
* validación en tiempo real de los campos de registro e inicio de sesión demostrativo;
* presentación correcta del contenido institucional y del documento de Términos y Condiciones.

**Evidencia visual:**

**1. Sección principal (Hero) — propuesta de valor**

*Desarrollado por: Alca Morán, César Alejandro*

<p align="center">
  <img src="assets/images/Cap5_Exec_Hero_Desktop.png" alt="Sección Hero de la Landing Page" title="Hero Section - Desktop" width="700">
</p>

**2. Planes de suscripción**

*Desarrollado por: Rivas Méndez, Bernie Aarón*

<p align="center">
  <img src="assets/images/Cap5_Exec_Planes_Desktop.png" alt="Sección de planes de suscripción" title="Plans Section - Desktop" width="700">
</p>

**3. Testimonios de usuarios**

*Desarrollado por: Rivas Castillo, Christoper Steven*

<p align="center">
  <img src="assets/images/Cap5_Exec_Testimonios_Desktop.png" alt="Carrusel de testimonios" title="Testimonials Section - Desktop" width="700">
</p>

**4. Funcionalidades de la plataforma (La App)**

*Desarrollado por: Rivas Castillo, Christoper Steven*

<p align="center">
  <img src="assets/images/Cap5_Exec_LaApp_Desktop.png" alt="Sección de funcionalidades de la plataforma" title="Solve Section - Desktop" width="700">
</p>

**5. Equipo y videos institucionales**

*Desarrollado por: Tello Lima, Jose Alejandro*

<p align="center">
  <img src="assets/images/Cap5_Exec_Equipo_Desktop.png" alt="Sección del equipo de AgroFlet" title="Team Section - Desktop" width="700">
</p>

<p align="center">
  <img src="assets/images/Cap5_Exec_Videos_Desktop.png" alt="Sección de videos institucionales" title="Videos Section - Desktop" width="700">
</p>

**6. Footer institucional y Términos y Condiciones**

*Desarrollado por: Centeno León, Adriano Samir*

<p align="center">
  <img src="assets/images/Cap5_Exec_Terminos.png" alt="Footer institucional" title="Footer - Desktop" width="700">
</p>

<p align="center">
  <img src="assets/images/Cap5_Exec_Terminos.png" alt="Documento de Términos y Condiciones" title="Terms and Conditions" width="700">
</p>

**7. Internacionalización (ES / EN)**

*Desarrollado por: Centeno León, Adriano Samir*

<p align="center">
  <img src="assets/images/Cap5_Exec_Idioma_ES.png" alt="Landing Page en español" title="i18n - Español" width="700">
</p>

<p align="center">
  <img src="assets/images/Cap5_Exec_Idioma_EN.png" alt="Landing Page en inglés" title="i18n - English" width="700">
</p>

**8. Modales demostrativos de registro e inicio de sesión**

*Desarrollado por: Alca Morán, César Alejandro*

<p align="center">
  <img src="assets/images/Cap5_Exec_Modal_Registro.png" alt="Modal de registro demostrativo" title="Auth Modal - Sign Up" width="700">
</p>

<p align="center">
  <img src="assets/images/Cap5_Exec_Validaciones.png" alt="Validaciones del formulario de registro" title="Form Validation" width="700">
</p>

**9. Vista móvil y validación responsive**

*Desarrollado por: Rivas Méndez, Bernie Aarón*

<p align="center">
  <img src="assets/images/Cap5_Exec_Mobile_Hero.png" alt="Vista móvil de la Landing Page" title="Mobile Execution" width="350">
</p>

<p align="center">
  <img src="assets/images/Cap5_Exec_Mobile_Menu.png" alt="Menú responsive en dispositivo móvil" title="Responsive Menu" width="350">
</p>

<p align="center">
  <img src="assets/images/Cap5_Exec_DevTools_Responsive.png" alt="Validación responsive en Chrome DevTools" title="Chrome DevTools - Responsive" width="700">
</p>


#### 5.2.1.6. Services Documentation Evidence for Sprint Review

Durante el Sprint 1, la Landing Page de AgroFlet no consume todavía el RESTful API de la plataforma ni servicios externos orientados a los procesos logísticos.

Las funcionalidades interactivas de registro e inicio de sesión presentes en esta versión corresponden a una demostración ejecutada íntegramente en el cliente mediante JavaScript y `localStorage`, tal como se declara en la sección 5.2.1.4. Del mismo modo, las cifras mostradas en los contadores del Hero y los testimonios son contenido estático de presentación.

La integración con los servicios RESTful internos (endpoints de autenticación, gestión de flotas, operaciones de transporte e incidencias especificados como Technical Stories en el Capítulo III) se incorporará en los siguientes Sprints desde la Frontend Web Application desarrollada con Vue.js.

Por lo tanto, en este Sprint no corresponde presentar documentación OpenAPI o Swagger como evidencia de consumo de servicios desde la Landing Page. En las siguientes entregas esta sección se actualizará para incluir:

* la relación completa de los endpoints implementados;
* el verbo HTTP asociado a cada acción (GET, POST, PUT, PATCH, DELETE) y la sintaxis de las llamadas;
* el detalle de los parámetros requeridos y la explicación estructurada de las respuestas;
* capturas de pantalla de la interacción funcional con la API mediante Swagger UI con datos de muestra;
* el enlace al repositorio de Web Services y los identificadores de los commits asociados a la documentación.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

La versión `v1.0.0` de la Landing Page de AgroFlet fue publicada exitosamente utilizando GitHub Pages. Dado que el alcance de esta iteración se limitó a la presentación web estática, aún no se han configurado entornos de despliegue para la Frontend Web Application ni para los Web Services.

**Actividades de despliegue realizadas:**

**1. Configuración del repositorio de código fuente**

* Se creó un repositorio público dedicado exclusivamente a la Landing Page dentro de la organización del equipo.
* Se estructuró el control de versiones bajo GitFlow para facilitar la publicación desde la rama `main`.
* Enlace del repositorio: `[https://github.com/AGROFLET/Agroflet-landing-page]`

**2. Habilitación y configuración de GitHub Pages**

* Se activó el servicio de alojamiento estático desde `Settings > Pages` del repositorio.
* Se definió la rama `main` y el directorio raíz (`/root`) como origen de los archivos publicados.
* Se incorporó el archivo `.nojekyll` en la raíz del proyecto para evitar el procesamiento por Jekyll y asegurar la carga del directorio `assets/`.

<p align="center">
  <img src="assets/images/Cap5_Deploy_Settings_Pages.png" alt="Configuración de GitHub Pages en el repositorio" title="Settings > Pages" width="700">
</p>

**3. Publicación automatizada**

* Cada integración aprobada hacia `main` dispara automáticamente el workflow de publicación de GitHub Pages, actualizando el contenido en producción sin intervención manual del equipo.

<p align="center">
  <img src="assets/images/Cap5_Deploy_Actions.png" alt="Ejecución del workflow de despliegue" title="pages build and deployment" width="700">
</p>

**4. Verificación y validación en producción**

* Se validó la correcta carga de estilos, scripts e imágenes desde la URL pública.
* Se verificó el funcionamiento del cambio de idioma, del carrusel de testimonios y de los modales en el entorno desplegado.
* Se comprobó el acceso al documento `docs/Terms-and-conditions.html` desde el footer.

* **Versión desplegada:** `v1.0.0`
* **URL de producción:** `[https://agroflet.github.io/Agroflet-landing-page/]`

<p align="center">
  <img src="assets/images/Cap5_Deploy_Produccion.png" alt="Landing Page de AgroFlet desplegada en producción" title="AgroFlet - Producción" width="700">
</p>

#### 5.2.1.8. Team Collaboration Insights during Sprint

Durante el Sprint 1 el equipo distribuyó el desarrollo de la Landing Page en aspectos claramente delimitados: estructura HTML semántica, diseño responsive, componentes visuales, interacciones JavaScript, internacionalización, documentación y despliegue.

**Actividades de implementación desarrolladas:**

* **Planificación visual:** se tomaron como referencia los wireframes y mockups elaborados en Figma durante el Capítulo IV para definir la jerarquía de la información, las secciones y la aplicación de la paleta de marca de AgroFlet.
* **Desarrollo modular:** la maquetación se dividió en componentes independientes (Header, Hero, Plans, Testimonials, Solve, Team, Videos, Footer y Modales), permitiendo que cada integrante trabajara en una rama `feature/*` propia.
* **Integración de funcionalidades:** se aplicaron estilos responsivos mediante CSS Grid, Flexbox y Custom Properties, y se incorporó la lógica de interactividad en JavaScript, incluyendo el sistema de internacionalización español/inglés.
* **Gestión de versiones y despliegue:** se utilizó GitHub como plataforma central, aplicando Pull Requests y revisiones cruzadas antes de integrar los cambios a `develop` y, posteriormente, a `main` para su publicación en GitHub Pages.

La estrategia de ramas permitió reducir los conflictos de integración sobre archivos compartidos como `index.html` y `styles.css`, y mantener trazabilidad sobre las contribuciones individuales. Como principal aprendizaje, el equipo identificó la importancia de mantener coherencia entre las funcionalidades descritas en el Project Report y aquellas efectivamente implementadas en el producto, criterio que motivó la reprogramación de la User Story UH28 al Sprint 2.

**Analíticas de colaboración en GitHub:**

**1. Evidencia de ramas del repositorio**

<p align="center">
  <img src="assets/images/Cap5_Collab_Branches.png" alt="Ramas del repositorio de la Landing Page" title="Git Branches" width="700">
</p>

**2. Historial de commits por integrante**

*Alca Morán, César Alejandro (`CesarAlcaM`)*
<p align="center">
  <img src="assets/images/Cap5_Collab_Commits_Cesar.png" alt="Commits de César Alca" title="Commits - César" width="700">
</p>

*Centeno León, Adriano Samir (`AdrianoCenteno`)*
<p align="center">
  <img src="assets/images/Cap5_Collab_Commits_Adriano.png" alt="Commits de Adriano Centeno" title="Commits - Adriano" width="700">
</p>

*Rivas Méndez, Bernie Aarón (`BernieRivasM`)*
<p align="center">
  <img src="assets/images/Cap5_Collab_Commits_Bernie.png" alt="Commits de Bernie Rivas" title="Commits - Bernie" width="700">
</p>

*Rivas Castillo, Christoper Steven (`ChristoperRivasC`)*
<p align="center">
  <img src="assets/images/Cap5_Collab_Commits_Christoper.png" alt="Commits de Christoper Rivas" title="Commits - Christoper" width="700">
</p>

*Tello Lima, Jose Alejandro (`JoseTelloL`)*
<p align="center">
  <img src="assets/images/Cap5_Collab_Commits_Jose.png" alt="Commits de Jose Tello" title="Commits - Jose" width="700">
</p>

**3. Colaboradores activos en el repositorio**

*Gráfica de la actividad conjunta del equipo y de la distribución de aportes (adiciones y eliminaciones de código) durante el Sprint.*

<p align="center">
  <img src="assets/images/Cap5_Collab_Contributors.png" alt="Contributors del repositorio" title="Insights > Contributors" width="700">
</p>

**4. Histograma de contribuciones en el tiempo**

*Frecuencia de commits realizados durante el Sprint, evidenciando un esfuerzo sostenido y coordinado hacia la integración final.*

<p align="center">
  <img src="assets/images/Cap5_Collab_Histograma.png" alt="Histograma de contribuciones" title="Insights > Commits" width="700">
</p>

---

### 5.2.2. Sprint 2

Durante el Sprint 2 se implementó la primera versión de la **Frontend Web Application de AgroFlet (v1.0.0)** para despachadores y compradores mayoristas. La aplicación, desarrollada con **Vue 3, Vite, PrimeVue, Pinia y Vue Router**, consume una **Fake API con json-server** y se publicó en Vercel y GitHub Pages. El alcance se basa en las historias del Capítulo III que no se desarrollaron en el Sprint 1.

#### 5.2.2.1. Sprint Planning 2

| Sprint # | Sprint 2 |
| :--- | :--- |
| **Sprint Planning Background** | |
| Date | 24/09/2026  |
| Time | 8:00 PM |
| Location | Google Meet |
| Prepared By | Alca Morán, César Alejandro |
| Attendees (to planning meeting) | Alca Morán, César Alejandro<br>Centeno León, Adriano Samir<br>Rivas Méndez, Bernie Aarón<br>Rivas Castillo, Christoper Steven<br>Tello Lima, Jose Alejandro |
| **Sprint 1 Review Summary** | Se desplegó la Landing Page v1.0.0, con información del producto, planes, testimonios, navegación responsive e idiomas ES/EN. La historia de contacto **US28** quedó pendiente. |
| **Sprint 1 Retrospective Summary** | Se mantuvo el trabajo paralelo con GitFlow y se priorizó la integración temprana entre vistas, servicios y componentes compartidos. |
| **Sprint Goal & User Stories** | |
| **Sprint 2 Goal** | *Our focus is on* publicar una aplicación que permita gestionar flotas y envíos, reportar posiciones e incidencias y consultar alertas por rol.<br>*We believe it delivers* mayor visibilidad y coordinación a despachadores y compradores.<br>*This will be confirmed when* se pueda registrar, iniciar y cerrar una operación de demostración, y el comprador asociado consulte su seguimiento desde la aplicación publicada. |
| **Sprint 2 Velocity** | Por confirmar con el cierre formal del Sprint. |
| **Sum of Story Points** | **84 SP planificados**: 81 SP de las 27 historias de la aplicación y 3 SP de US28, arrastrada del Sprint 1. **US28 sigue pendiente de verificación.** |

**Nota:** El Product Backlog del Capítulo III usa los identificadores **US**. El Sprint 1 utiliza **UH** para algunas historias del Landing Page; aquí se conservan los **US** originales a fin de asegurar la trazabilidad.

#### 5.2.2.2. Aspect Leaders and Collaborators

A continuación, se presenta la distribución de responsabilidades para el desarrollo del Sprint 2 de AgroFlet. En este cuadro se detallan los módulos técnicos o aspectos liderados por cada integrante, así como sus áreas de colaboración cruzada, garantizando el cumplimiento de todos los objetivos planificados bajo un enfoque de trabajo colaborativo.

| Team Member | GitHub Username* | Aspecto liderado | Colaboración |
| :--- | :--- | :--- | :--- |
| Tello Lima, Jose Alejandro | `j4ndrow` | Fake API y gestión de flotas | Integración de servicios |
| Centeno León, Adriano Samir | `Adri11-dk` | Internacionalización, perfil y documentación | Revisión funcional |
| Rivas Castillo, Christoper Steven | `CODERT0PH` | Configuración, IAM, incidencias y despliegue | Integración de la aplicación |
| Rivas Méndez, Bernie Aarón | `ARivas3008` | Interfaz compartida y seguimiento cartográfico | Diseño responsive |
| Alca Morán, César Alejandro | `almocesar-cell` | Operaciones y gestión de envíos | Integración de vistas |

*Los nombres de usuario se toman de la documentación del repositorio y deben contrastarse con **Insights > Contributors** antes de la entrega.*

**L:** líder del aspecto. **C:** colaborador. **—:** sin participación específica documentada en ese aspecto. La validación documental está asignada a Adriano; la gestión de flotas a Jose; las operaciones y envíos a César. Los accesos, incidencias y la preparación del despliegue registran commits de Christoper, y el seguimiento cartográfico registra commits de Bernie.

**Distribución por ramas:**

| Feature Branch | Responsable | Desarrollo |
| :--- | :--- | :--- |
| `feature/project-setup` | Christoper Rivas | Configuración de Vue, Vite y estructura por capas |
| `feature/fake-api-and-fleet` | Jose Tello | Fake API, vehículos y conductores |
| `feature/i18n-profile-and-docs` | Adriano Centeno | Idiomas, perfil y documentación |
| `feature/iam-incidents-and-deployment` | Christoper Rivas | Autenticación, incidencias y despliegue |
| `feature/shared-ui-and-tracking` | Bernie Rivas | Componentes compartidos, mapas y posiciones |
| `feature/shipment-operations` | César Alca | Registro, consulta y ciclo de vida de operaciones |


#### 5.2.2.3. Sprint Backlog 2

El Backlog incorpora las **27 User Stories de la aplicación web no trabajadas en el Sprint 1** (US01–US23, US31–US34). La historia **US28**, pendiente del Landing Page, se registra por separado. Los títulos provienen del Capítulo III; las tareas se sintetizan a partir de la implementación documentada en GitHub. Se usa una tarea resumida por historia para facilitar la lectura.

| User Story Id | User Story Title | Work Item / Task Id | Work Item / Task Title | Description | Estimation (h) | Assigned To | Status |
| :--- | :--- | :--- | :--- | :--- | ---: | :--- | :---: |
| US01 | Registro de cuenta | T01 | Registro de usuarios | Crear formulario por rol y validar campos y correo único. | 5 | Christoper Rivas | Finalizada |
| US02 | Inicio de sesión | T02 | Autenticación | Implementar acceso, sesión y control de credenciales. | 4 | Christoper Rivas | Finalizada |
| US03 | Cierre de sesión | T03 | Logout y rutas protegidas | Cerrar sesión y restringir vistas según rol. | 5 | Christoper Rivas | Finalizada |
| US04 | Recuperación de contraseña | T04 | Recuperación y cambio | Solicitud genérica y restablecimiento mediante token de demostración. | 6 | Christoper Rivas | Finalizada |
| US05 | Registro de vehículo | T05 | Alta de vehículos | Crear formulario con placa, capacidad y validaciones. | 4 | Jose Tello | Finalizada |
| US06 | Consulta y edición de vehículos | T06 | Gestión de vehículos | Listar y editar flota; proteger vehículos reservados. | 5 | Jose Tello | Finalizada |
| US07 | Registro de conductor | T07 | Alta de conductores | Registrar conductores, licencia y DNI no duplicado. | 4 | Jose Tello | Finalizada |
| US08 | Selección de recursos para el despacho | T08 | Asignación de recursos | Seleccionar vehículo y conductor disponibles. | 2 | Jose Tello | Finalizada |
| US09 | Registro de operación programada | T09 | Nueva operación | Crear envío y reservar sus recursos, validando capacidad. | 6 | César Alca | Finalizada |
| US10 | Consulta de operaciones activas | T10 | Dashboard | Mostrar envíos autorizados, estados e indicadores. | 4 | César Alca | Finalizada |
| US11 | Detalle de operación | T11 | Detalle del envío | Mostrar datos, ruta e historial con acceso por rol. | 4 | César Alca | Finalizada |
| US12 | Cierre de operación | T12 | Entrega y cancelación | Cambiar estado y liberar recursos; exigir motivo al cancelar. | 4 | César Alca | Finalizada |
| US13 | Registro de incidencia | T13 | Nueva incidencia | Registrar incidente y recalcular ETA sin duplicaciones. | 5 | Christoper Rivas | Finalizada |
| US14 | Historial de incidencias | T14 | Lista de incidencias | Consultar eventos e impacto en el traslado. | 2 | Christoper Rivas | Finalizada |
| US15 | Historial con filtros | T15 | Filtros de operaciones | Filtrar por fecha, estado, carga y destino. | 4 | César Alca | Finalizada |
| US16 | Búsqueda por código o placa | T16 | Búsqueda de envíos | Localizar operaciones por código o placa. | 2 | César Alca | Finalizada |
| US17 | Posiciones en mapa | T17 | Seguimiento cartográfico | Mostrar posiciones reportadas y fecha de actualización en Leaflet. | 5 | Bernie Rivas | Finalizada |
| US18 | Ruta planificada | T18 | Visualización de ruta | Diferenciar la ruta prevista de las posiciones reportadas. | 3 | Bernie Rivas | Finalizada |
| US19 | Alertas por incidencia | T19 | Notificaciones de incidencia | Avisar a participantes sin duplicar alertas. | 3 | Christoper Rivas | Finalizada |
| US20 | Alertas por cambio de estado | T20 | Notificaciones de estado | Notificar transiciones y permitir marcar avisos como leídos. | 3 | Christoper Rivas | Finalizada |
| US21 | Edición de perfil | T21 | Configuración de perfil | Modificar datos permitidos del usuario. | 2 | Adriano Centeno | Finalizada |
| US22 | Cambio de contraseña | T22 | Seguridad de la cuenta | Validar contraseña actual y cerrar sesión al actualizarla. | 2 | Adriano Centeno | Finalizada |
| US23 | Idioma de la aplicación | T23 | Internacionalización | Incorporar inglés y español con preferencia persistente. | 2 | Adriano Centeno | Finalizada |
| US31 | Inicio del traslado | T24 | Inicio de operación | Cambiar `planned` a `in_transit` y registrar salida. | 2 | César Alca | Finalizada |
| US32 | Registro de posición reportada | T25 | Reporte de ubicación | Registrar coordenadas, fecha y fuente de la posición. | 3 | Bernie Rivas | Finalizada |
| US33 | Términos del servicio | T26 | Términos y condiciones | Publicar las condiciones del servicio dentro de la aplicación. | 2 | Adriano Centeno | Finalizada |
| US34 | Acceso por segmento desde landing | T27 | Acceso por rol | Recibir `?segment=dispatcher` o `?segment=buyer` en acceso/registro. | 1 | Christoper Rivas | Finalizada |
| US28 | Contacto | T28 | Formulario de contacto del landing | Implementar y comprobar envío efectivo desde la Landing Page. | 3 | Bernie Rivas | Finalizada |

**Tareas técnicas complementarias (sin Story Points adicionales):**

| Task Id | Task Title | Assigned To | Status |
| :--- | :--- | :--- | :---: |
| TT01 | Configuración inicial y cliente HTTP compartido | Christoper Rivas | Finalizada |
| TT02 | Fake API con `server/db.json` y rutas `/api/v1` | Jose Tello | Finalizada |
| TT03 | Layout, diseño responsive y componentes reutilizables | Bernie Rivas | Finalizada |
| TT04 | Diccionarios y documentación técnica | Adriano Centeno | Finalizada |
| TT05 | Integración, Vercel y GitHub Actions para Pages | Christoper Rivas | Finalizada |

Las 28 historias de usuario y sus respectivas tareas principales figuran Finalizadas. La tarea T28 / US28 (Contacto) fue trasladada desde el Sprint 1 del Landing Page y logró completarse en este ciclo. Adicionalmente, el equipo proporcionó el enlace y la captura del video de navegación de la aplicación web correspondiente al Sprint 2, incorporados en la sección 5.2.2.5; cabe destacar que esta evidencia valida el incremento actual y es distinta de la confirmación de los videos About-the-Product y About-the-Team incrustados en la landing page.

#### 5.2.2.4. Development Evidence for Sprint Review

La implementación se organizó mediante `main`, `develop`, ramas `feature/*` y `release/v1.0.0`. En `src/` se separaron los bounded contexts `iam`, `fleet`, `shipments`, `tracking` e `incidents`, con capas de dominio, aplicación, infraestructura y presentación.

| Evidencia de desarrollo | Rama / referencia |
| :--- | :--- |
| Base Vue, Vite y cliente HTTP | `feature/project-setup` |
| Fake API y gestión de flota | `feature/fake-api-and-fleet` |
| Componentes, vista móvil y mapa | `feature/shared-ui-and-tracking` |
| Registro, detalle e historial de envíos | `feature/shipment-operations` |
| Perfil, traducciones y documentación | `feature/i18n-profile-and-docs` |
| IAM, incidencias y despliegue | `feature/iam-incidents-and-deployment` |

**Repositorio:** [AGROFLET/Agroflet-frontend-application](https://github.com/AGROFLET/Agroflet-frontend-application). 

Vista del proyecto en github:
<p align="center">
  <img src="assets/images/Cap5_Dev_View_Sprint 2.PNG" alt="Structurizr" title="View" width="700">
</p>

Vista de las ramas trabajadas:
<p align="center">
  <img src="assets/images/Cap5_Dev_View_Sprint 2_branches.PNG" alt="Structurizr" title="Branches" width="700">
</p>

Ejemplo html de Sprint 2:
<p align="center">
  <img src="assets/images/Cap5_Dev_Sprint_2_html_example.PNG" alt="Structurizr" title="Example" width="700">
</p>

Ejemplo vue de Sprint 2:
<p align="center">
  <img src="assets/images/Cap5_Dev_Sprint_2_vue_example.PNG" alt="Structurizr" title="Example" width="700">
</p>

Ejemplo de .js de Sprint 2:
<p align="center">
  <img src="assets/images/Cap5_Dev_Sprint_2_js_example.PNG" alt="Structurizr" title="Example" width="700">
</p>

Ejemplo de .env de Sprint 2:
<p align="center">
  <img src="assets/images/Cap5_Dev_Sprint_2_env_example.PNG" alt="Structurizr" title="Example" width="700">
</p>

Pull Request sprint 2:
<p align="center">
  <img src="assets/images/Cap5_Dev_PullRequest_Sprint_2_1.PNG" alt="Structurizr" title="PullRequest" width="700">
</p>
<p align="center">
  <img src="assets/images/Cap5_Dev_PullRequest_Sprint_2_2.PNG" alt="Structurizr" title="PullRequest" width="700">
</p>


#### 5.2.2.5. Execution Evidence for Sprint Review

La versión de demostración permite recorrer las funcionalidades según el rol. Las siguientes vistas sirven como evidencia de ejecución y deben acompañarse con capturas propias de la versión desplegada.

| Vista / acción | Ruta o evidencia | User Stories |
| :--- | :--- | :--- |
| Registro, acceso y recuperación | `/iam/sign-up`, `/iam/sign-in`, `/iam/password-recovery` | US01–US04, US34 |
| Panel principal y gestión de envíos | `/dashboard`, `/shipments/new`, `/shipments/:id` | US08–US12, US31 |
| Vehículos y conductores | `/fleet/vehicles`, `/fleet/drivers` | US05–US07 |
| Historial y búsqueda | `/shipments` | US15–US16 |
| Mapa, ruta e incidencias | Detalle de envío, mapa y diálogos | US13–US14, US17–US18, US32 |
| Alertas de operaciones | `/notifications` | US19–US20 |
| Cuenta, idioma y condiciones | `/iam/profile`, `/terms` | US21–US23, US33 |


Vista de Web:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_page1.PNG" alt="Structurizr" title="View" width="700">
</p>

**Sección comprador:**
Envíos entrantes:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_buyer_view_1.PNG" alt="Structurizr" title="Buyer" width="700">
</p>

Historial:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_buyer_view_2.PNG" alt="Structurizr" title="Buyer" width="700">
</p>

Notificaciones:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_buyer_view_3.PNG" alt="Structurizr" title="Buyer" width="700">
</p>

Configuración: 
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_buyer_view_4.PNG" alt="Structurizr" title="Buyer" width="700">
</p>

---
**Sección despachador:**
Panel:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_dispatcher_view_1.PNG" alt="Structurizr" title="Dispatcher" width="700">
</p>

Envíos:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_dispatcher_view_2.PNG" alt="Structurizr" title="Dispatcher" width="700">
</p>

Registrar envío:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_dispatcher_view_3.PNG" alt="Structurizr" title="Dispatcher" width="700">
</p>

Vehículos:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_dispatcher_view_4.PNG" alt="Structurizr" title="Dispatcher" width="700">
</p>

Registrar vehículo:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_dispatcher_view_4_1.PNG" alt="Structurizr" title="Dispatcher" width="700">
</p>

Conductores:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_dispatcher_view_5.PNG" alt="Structurizr" title="Dispatcher" width="700">
</p>

Registrar conductor:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_dispatcher_view_5_1.PNG" alt="Structurizr" title="Dispatcher" width="700">
</p>

Notificaciones:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_dispatcher_view_6.PNG" alt="Structurizr" title="Dispatcher" width="700">
</p>

Configuración:
<p align="center">
  <img src="assets/images/Cap5_Deploy_Sprint 2_dispatcher_view_7.PNG" alt="Structurizr" title="Dispatcher" width="700">
</p>

#### 5.2.2.6. Services Documentation Evidence for Sprint Review

Durante el Sprint 2 (TB1), la Web Application de AgroFlet consume una **Fake API** basada en `json-server` 0.17. Este servicio permite desarrollar y demostrar los flujos de los segmentos Despachador y Comprador antes de integrar el RESTful API definitivo. A diferencia de un backend productivo, las reglas de negocio y las restricciones de acceso de esta versión se aplican principalmente desde el frontend.

La documentación del servicio simulado se encuentra en el archivo [`docs/fake-api.openapi.yaml`](https://github.com/AGROFLET/Agroflet-frontend-application/blob/main/docs/fake-api.openapi.yaml), con **OpenAPI 3.0.3** y versión de contrato **1.0.0**. El documento describe rutas, métodos HTTP, parámetros, cuerpos de solicitud, esquemas, respuestas y ejemplos. Sus operaciones identifican las Technical Stories que emulan; esto documenta el mock utilizado en TB1, no acredita la implementación del futuro backend ASP.NET Core.

**Ubicación y configuración del servicio**

| Entorno | URL base | Configuración verificable |
| :--- | :--- | :--- |
| Desarrollo integrado con Vite | `/api/v1` en el servidor de `npm run dev` o `npm run preview` | Fake API servida desde Vite. |
| JSON Server independiente | `http://localhost:3000/api/v1` | `npm run server`; datos de `server/db.json`. |
| Demostración publicada | [https://agroflet-frontend-application.vercel.app/api/v1](https://agroflet-frontend-application.vercel.app/api/v1) | Vercel Function en `api/index.js`. |

El archivo [`server/routes.json`](https://github.com/AGROFLET/Agroflet-frontend-application/blob/main/server/routes.json) transforma `/api/v1/*` en los recursos de JSON Server. El [README técnico](https://github.com/AGROFLET/Agroflet-frontend-application#fake-api-json-server) explica las diferencias de persistencia entre los modos locales y el despliegue. La función publicada admite almacenamiento compartido mediante Upstash Redis cuando la integración está configurada; sin ella utiliza datos por instancia. El código y la documentación de esa configuración no sustituyen una evidencia del estado de la base de datos en el panel de Vercel.

**Recursos documentados por contexto**

Las rutas de la tabla son relativas a la URL base `/api/v1`. Los métodos corresponden al contrato OpenAPI existente.

| Contexto | Recurso | Métodos documentados | Uso en la Web Application |
| :--- | :--- | :--- | :--- |
| IAM | `/users`, `/users/{id}` | GET y POST en colección; GET y PATCH por ID | Registro, consulta de cuentas, sesión demostrativa y actualización de perfil. |
| IAM | `/password-reset-requests`, `/password-reset-requests/{id}` | GET y POST en colección; PATCH por ID | Solicitudes de recuperación y actualización de su estado. |
| Fleet | `/vehicles`, `/vehicles/{id}` | GET y POST en colección; GET y PATCH por ID | Registro, consulta y actualización de vehículos y disponibilidad. |
| Fleet | `/drivers`, `/drivers/{id}` | GET y POST en colección; GET y PATCH por ID | Registro, consulta y actualización de conductores. |
| Shipments | `/locations` | GET | Catálogo de origen y destino. |
| Shipments | `/shipments`, `/shipments/{id}` | GET y POST en colección; GET, PATCH y DELETE por ID | Envíos, filtros y actualización de operaciones. El DELETE documentado no equivale al flujo de cancelación del frontend. |
| Shipments | `/status-changes` | GET y POST | Historial de cambios de estado. |
| Tracking | `/positions` | GET y POST | Consulta y registro de posiciones reportadas. |
| Incidents | `/incidents` | GET y POST | Registro y consulta de incidencias. |
| Incidents | `/notifications`, `/notifications/{id}` | GET y POST en colección; PATCH por ID | Alertas y marcado de notificaciones como leídas. |

El contrato también incluye `POST /contact-messages`. Sin embargo, el formulario UH28 de la Landing Page V2 guarda la demostración en `localStorage`, bajo `agroflet_contacts`; **no consume ese endpoint**. La existencia del recurso en OpenAPI no demuestra una integración de la landing con el servicio.

**Procedimiento reproducible de consulta de la documentación**

1. Abrir el repositorio del frontend y ejecutar `npm install`.
2. Iniciar la Fake API independiente mediante `npm run server`.
3. Abrir `docs/fake-api.openapi.yaml` en Swagger Editor o en el editor compatible de WebStorm.
4. Seleccionar el servidor `http://localhost:3000/api/v1` y consultar un recurso, por ejemplo `GET /locations` o `GET /shipments?dispatcherId=1`.
5. Contrastar el resultado con los esquemas y respuestas del contrato. Las solicitudes de escritura deben realizarse únicamente con datos de prueba.

Ejemplos de consulta de solo lectura contra el servicio local:

```http
GET http://localhost:3000/api/v1/locations
GET http://localhost:3000/api/v1/shipments?dispatcherId=1
GET http://localhost:3000/api/v1/positions?shipmentId=1
```

Estos ejemplos indican cómo reproducir la revisión; no se presentan como resultados de pruebas HTTP ejecutadas en esta actualización del informe. La evidencia documental comprobada es el contrato OpenAPI almacenado en GitHub y su correspondencia con la configuración del mock.

**Alcance y limitaciones de TB1**

- La autenticación es emulada sobre la colección `users`. Aunque el cliente envía un encabezado Bearer, JSON Server no valida el token ni aplica autorización productiva.
- La recuperación de contraseña no cuenta todavía con un servicio de correo. El enlace demostrativo de restablecimiento solo se muestra en desarrollo.
- Las ubicaciones representan posiciones reportadas o datos marcados como demostrativos; no acreditan telemetría GPS automática.
- La documentación OpenAPI del mock no se presenta como Swagger de un RESTful API ASP.NET Core ya desplegado.

---

#### 5.2.2.7. Software Deployment Evidence for Sprint Review

Durante el Sprint 2 (TB1) se publicó la primera versión de la Web Application de AgroFlet y se actualizó la Landing Page V2. La Web Application se encuentra disponible en Vercel y GitHub Pages; la Fake API utilizada por ambas publicaciones del frontend se aloja en Vercel. La landing constituye un producto separado, desarrollado con HTML, CSS y JavaScript.

**Productos y direcciones de publicación**

| Producto | Repositorio | URL pública | Evidencia disponible |
| :--- | :--- | :--- | :--- |
| Landing Page V2 | [Agroflet-landing-page](https://github.com/AGROFLET/Agroflet-landing-page) | [Landing Page](https://agroflet.github.io/Agroflet-landing-page/) | Workflow `pages.yml`, ejecución exitosa de GitHub Actions y commits del formulario UH28. |
| Web Application en Vercel | [Agroflet-frontend-application](https://github.com/AGROFLET/Agroflet-frontend-application) | [Web Application](https://agroflet-frontend-application.vercel.app/) | `vercel.json` y captura de Production Deployment con estado Ready. |
| Web Application en GitHub Pages | [Agroflet-frontend-application](https://github.com/AGROFLET/Agroflet-frontend-application) | [Web Application en Pages](https://agroflet.github.io/Agroflet-frontend-application/) | Workflow `deploy-github-pages.yml` y ejecución exitosa de GitHub Actions. |
| Fake API | Incluida en el repositorio del frontend | [Base del servicio simulado](https://agroflet-frontend-application.vercel.app/api/v1) | `api/index.js`, `server/routes.json` y contrato OpenAPI. |
| RESTful API definitivo | Implementación posterior al alcance acreditado de TB1 | Sin despliegue acreditado en esta sección | Se mantiene separado de la Fake API. |

La dirección `https://agroflet.github.io/Agroflet-frontend-application/` corresponde a la **Web Application**, no a la Landing Page. Esta distinción permite identificar y revisar cada producto de la entrega.

**1. Configuración y evidencia de Vercel**

El archivo [`vercel.json`](https://github.com/AGROFLET/Agroflet-frontend-application/blob/main/vercel.json) establece la configuración reproducible del frontend:

```text
Framework: Vite / Vue
Build command: npm run build
Output directory: dist
API rewrite: /api/v1/:path* -> /api
SPA rewrite: /(.*) -> /index.html
Production API base: /api/v1
```

La primera reescritura dirige las solicitudes del mock a la Vercel Function. La segunda permite que las rutas internas de Vue Router sean atendidas por la SPA. El despliegue incluye los archivos JSON del directorio `server/` necesarios para inicializar los datos demostrativos.

<p align="center">
  <img src="assets/images/Cap5_Deployment_Evidence.png" alt="Production Deployment de AgroFlet en Vercel con estado Ready y origen vercel deploy" width="700">
</p>

*Figura. El panel muestra el dominio agroflet-frontend-application.vercel.app, el estado Ready y la fuente «vercel deploy». También aparece la opción «Connect Git». La captura acredita una publicación por CLI; no acredita que el proyecto estuviera conectado a GitHub ni que cada push a main generara un despliegue automático de Vercel.*

El procedimiento reproducible documentado en el repositorio es:

```bash
npm install
npm run build
vercel login
vercel link
vercel --prod
```

La conexión Git de Vercel puede configurarse posteriormente para automatizar publicaciones. En esta sección se diferencia esa posibilidad del método acreditado por la captura. La evidencia Ready no se utiliza para afirmar que todos los endpoints fueron probados.

**2. Publicación de la Web Application en GitHub Pages**

El workflow [`deploy-github-pages.yml`](https://github.com/AGROFLET/Agroflet-frontend-application/blob/main/.github/workflows/deploy-github-pages.yml) se ejecuta ante un push a `main` o mediante `workflow_dispatch`. Sus pasos son:

1. Obtener el código y configurar Node.js 22.
2. Instalar dependencias con `npm ci`.
3. Compilar con `npm run build -- --base "/Agroflet-frontend-application/"`.
4. Configurar `VITE_AGROFLET_PLATFORM_API_URL` hacia la Fake API pública de Vercel, salvo que una variable del repositorio la reemplace.
5. Copiar `dist/index.html` a `dist/404.html` para permitir que las rutas internas abran la SPA.
6. Publicar `dist/` mediante las acciones oficiales de GitHub Pages.

GitHub Pages solo sirve contenido estático: la aplicación publicada allí consume el servicio simulado en Vercel. Las rutas internas atendidas mediante `404.html` pueden devolver un estado HTTP 404 aunque Vue Router muestre la pantalla; es una limitación de ese mecanismo de publicación.

**Evidencia de ejecución:** [Deploy to GitHub Pages — run 37274392426](https://github.com/AGROFLET/Agroflet-frontend-application/actions/runs/37274392426), asociado al commit [9576c15](https://github.com/AGROFLET/Agroflet-frontend-application/commit/9576c150b6098f9e41741793138f363d0be44473). La consulta del historial de GitHub Actions realizada para esta corrección confirmó estado `completed` y conclusión `success`.

**3. Actualización y despliegue de la Landing Page V2**

La landing conserva sus secciones de presentación, planes, testimonios, solución, equipo y videos. En TB1 se incorporó el formulario UH28 después de Videos, con validaciones, textos ES/EN y guardado demostrativo en el navegador. El formulario utiliza el azul de las secciones alternadas del sitio.

El workflow [`pages.yml`](https://github.com/AGROFLET/Agroflet-landing-page/blob/main/.github/workflows/pages.yml) revisa los archivos estáticos y la sintaxis JavaScript, prepara `index.html`, `assets/`, `docs/` y `.nojekyll`, y publica el artefacto en GitHub Pages. No requiere compilar la landing con Vite.

| Cambio de la Landing V2 | Evidencia trazable |
| :--- | :--- |
| Incorporación de UH28 después de Videos | [Pull Request #3, integrado](https://github.com/AGROFLET/Agroflet-landing-page/pull/3) |
| Adaptación al fondo azul existente | [Commit 57ce8f6](https://github.com/AGROFLET/Agroflet-landing-page/commit/57ce8f64dc7b85182205a85d157b8cb0ccab3ef6) |
| Actualización del enlace de estilos para renovar la caché | [Commit a98634a](https://github.com/AGROFLET/Agroflet-landing-page/commit/a98634ad38250b15129f87bd6af06076bbdc6f7b) |
| Publicación de la actualización | [Deploy AgroFlet to GitHub Pages — run 37855277906](https://github.com/AGROFLET/Agroflet-landing-page/actions/runs/37855277906), estado `completed`, conclusión `success` |

Las evidencias anteriores permiten revisar por separado la configuración, el resultado del despliegue y los cambios del producto. Los flujos de la aplicación se documentan en 5.2.2.5; el alcance del servicio simulado y sus limitaciones se describen en 5.2.2.6. La publicación de una interfaz o de un mock no se atribuye al backend definitivo.

---

#### 5.2.2.8. Team Collaboration Insights during Sprint

Durante el Sprint 2 el equipo distribuyó el desarrollo de la aplicación web frontend (Single-Page Application) en aspectos técnicos y funcionales claramente delimitados: configuración de la arquitectura modular en Vue, diseño de componentes de UI con PrimeVue, gestión de estado reactivo con Pinia, integración con el Fake API Server, renderizado de mapas interactivos con Leaflet, internacionalización y despliegue continuo en la nube.

**Actividades de implementación desarrolladas:**

* **Estructuración arquitectónica y de dominio:** se establecieron los Bounded Contexts del proyecto (`iam`, `fleet`, `shipments`, `tracking` e `incidents`) dentro de la estructura de carpetas de Vue, aplicando el patrón Assembler/Entity para desacoplar el modelo de dominio de los contratos de transferencia de datos de la API.
* **Desarrollo modular y UI:** la interfaz se construyó mediante componentes reutilizables y vistas adaptadas a cada rol (Despachador para gestión operativa y Comprador Mayorista para consulta y monitoreo), implementando librerías como PrimeVue y vistas clave para la gestión de flota, registro de viajes y dashboards.
* **Simulación e integración asíncrona (Fake API):** se implementó un servidor simulado mediante `json-server` (`server/db.json` y `routes.json`) para exponer los endpoints RESTful (`/api/v1/*`), permitiendo el consumo HTTP asíncrono vía Axios con interceptores de autenticación JWT y manejo centralizado de errores antes de conectar el backend definitivo.
* **Trazabilidad geográfica e incidencias:** se integró la biblioteca Leaflet para renderizar capas cartográficas y rutas terrestres, complementada con el recálculo dinámico de la Hora Estimada de Llegada (ETA) al registrar incidencias o desvíos viales.
* **Gestión de versiones y despliegue continuo:** se mantuvo la metodología GitFlow trabajando sobre ramas de características (`feature/*`) con revisiones mediante Pull Requests hacia `develop`, desplegando la Single-Page Application Vercel.

La separación del código por Bounded Contexts y la utilización de Assemblers permitió que nosotros desarrollaramos funcionalidades en paralelo sin generar conflictos sobre los stores o las rutas del sistema. Como principal aprendizaje del sprint, el equipo reconoció el valor del uso de un Fake API robusto, lo cual evitó cuellos de botella en la integración frontend-backend.

**Analíticas de colaboración en GitHub:**

**1. Evidencia de ramas del repositorio**

<p align="center">
  <img src="assets/images/Cap5_Collab_Branches2.png" alt="Ramas del repositorio de la Landing Page" title="Git Branches" width="700">
</p>

**2. Historial de commits por integrante**

*Alca Morán, César Alejandro (`CesarAlcaM`)*
<p align="center">
  <img src="assets/images/Cap5_Collab_Commits_Cesar2.png" alt="Commits de César Alca" title="Commits - César" width="700">
</p>

*Centeno León, Adriano Samir (`AdrianoCenteno`)*
<p align="center">
  <img src="assets/images/Cap5_Collab_Commits_Adriano2.png" alt="Commits de Adriano Centeno" title="Commits - Adriano" width="700">
</p>

*Rivas Méndez, Bernie Aarón (`BernieRivasM`)*
<p align="center">
  <img src="assets/images/Cap5_Collab_Commits_Bernie2.png" alt="Commits de Bernie Rivas" title="Commits - Bernie" width="700">
</p>

*Rivas Castillo, Christoper Steven (`ChristoperRivasC`)*
<p align="center">
  <img src="assets/images/Cap5_Collab_Commits_Christoper2.png" alt="Commits de Christoper Rivas" title="Commits - Christoper" width="700">
</p>

*Tello Lima, Jose Alejandro (`JoseTelloL`)*
<p align="center">
  <img src="assets/images/Cap5_Collab_Commits_Jose2.png" alt="Commits de Jose Tello" title="Commits - Jose" width="700">
</p>

**3. Colaboradores activos en el repositorio**

*Gráfica de la actividad conjunta del equipo y de la distribución de aportes (adiciones y eliminaciones de código) durante el Sprint 2.*

<p align="center">
  <img src="assets/images/Cap5_Collab_Contributors2.png" alt="Contributors del repositorio" title="Insights > Contributors" width="700">
</p>

**4. Histograma de contribuciones en el tiempo**

*Frecuencia de commits realizados durante el Sprint 2, evidenciando un esfuerzo sostenido y coordinado hacia la integración final.*

<p align="center">
  <img src="assets/images/Cap5_Collab_Histograma2.png" alt="Histograma de contribuciones" title="Insights > Commits" width="700">
</p>
