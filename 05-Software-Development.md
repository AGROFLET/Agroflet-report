# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

La Gestión de Configuración de Software (SCM) establece las herramientas, convenciones y mecanismos de versionamiento utilizados por el equipo de AgroFlet para mantener la trazabilidad y consistencia de los artefactos desarrollados a lo largo del ciclo de vida del proyecto.

Durante el Sprint 1 se priorizó la implementación y despliegue de la primera versión de la Landing Page de AgroFlet, desarrollada mediante HTML5, CSS3 y JavaScript.

### 5.1.1. Software Development Environment Configuration

A continuación se listan los productos de software utilizados por el equipo, organizados por tipo de actividad, incluyendo las herramientas de arquitectura y gestión solicitadas.

| Actividad | Herramienta | Uso en AgroFlet |
| :--- | :--- | :--- |
| **Project Management** | Jira | Organización del Sprint Backlog, asignación de responsables y seguimiento de tareas ágiles. |
| **Communication** | Discord / Google Meet | Coordinación asincrónica, reuniones diarias (Daily Scrum) y revisiones de Sprint. |
| **Requirements & UX** | UXPressia / Miro | Elaboración de User Personas, Journey Maps y diagramas de EventStorming. |
| **UX/UI Design** | Figma | Desarrollo de wireframes, mockups y prototipos de la Landing Page y Web Application. |
| **Software Development** | Visual Studio Code | Editor principal para la implementación de HTML5, CSS3 y JavaScript. |
| **Frontend Framework** | Vue.js / PrimeVue | Desarrollo de la aplicación web del lado del cliente. |
| **Backend & DB** | ASP.NET Core / MySQL | Desarrollo de servicios RESTful API con C# y Entity Framework Core, y persistencia de datos. |
| **Software Architecture** | Structurizr | Elaboración de diagramas de arquitectura de software bajo el modelo C4. |
| **Version Control** | Git / GitHub | Gestión local de versiones y repositorio remoto para colaboración (Pull Requests, GitFlow). |
| **Deployment** | GitHub Pages | Publicación y alojamiento estático de la primera versión de la Landing Page. |
| **Documentation** | Swagger / Markdown | Documentación de API mediante OpenAPI y redacción del Project Report en GitHub. |

### 5.1.2. Source Code Management

Para la gestión del código fuente de AgroFlet se utiliza Git como sistema de control de versiones distribuido y GitHub como plataforma de colaboración.

Durante el Sprint 1, el producto implementado corresponde a la Landing Page de AgroFlet.

**Repositorio de Landing Page:**
*https://github.com/AGROFLET/Agroflet-landing-page*

Posteriormente, el ecosistema de AgroFlet contará con repositorios independientes para los demás productos que conforman la solución distribuida:
*   Landing Page
*   Frontend Web Application
*   RESTful API
*   Project Report

#### Estructura del repositorio de Landing Page

De acuerdo con el entorno local de desarrollo, la estructura del proyecto se organiza de la siguiente manera:

```text
AGROFLET/
├── assets/
│   ├── css/
│   │   └── styles.css
│   ├── i18n/
│   │   ├── en.json
│   │   └── es.json
│   ├── images/
│   │   ├── logo.jpg
│   │   └── team/
│   └── js/
│       └── app.js
├── docs/
│   └── Terms-and-conditions.html
├── .editorconfig
├── .gitignore
├── .nojekyll
├── index.html
├── LICENSE
└── README.md
```

**GitFlow Workflow**
El equipo adopta GitFlow como estrategia de administración de ramas.
*   `main`: contiene versiones estables y desplegables.
*   `develop`: integra los cambios aprobados para la siguiente versión.
*   `feature/*`: contiene el desarrollo de nuevas funcionalidades (ej. `feature/hero-section`, `feature/i18n`).
*   `release/*`: estabilización de una versión antes de producción.
*   `hotfix/*`: correcciones urgentes sobre una versión publicada.

**Semantic Versioning y Conventional Commits**
AgroFlet adopta Semantic Versioning 2.0.0 (`MAJOR.MINOR.PATCH`). La primera versión desplegada de la Landing Page se identifica como `v1.0.0`.
Los mensajes de commit siguen la convención de Conventional Commits (ej. `feat: implement responsive hero section`, `docs: update landing page documentation`).

### 5.1.3. Source Code Style Guide

**Convenciones HTML**
*   Elementos estructurales basados en HTML5 semántico (`<header>`, `<nav>`, `<main>`, `<section>`)[cite: 4].
*   Identificadores y clases redactados estrictamente en inglés[cite: 4].
*   Atributos `alt` obligatorios en imágenes informativas[cite: 4].
*   Uso de atributos de accesibilidad como `aria-label`[cite: 4].
*   Indentación consistente de dos espacios[cite: 2].

**Convenciones CSS**
Se utiliza una nomenclatura inspirada en BEM (Block, Element, Modifier)[cite: 4]:
```css
.hero {}
.hero__title {}
.hero__title-line--sub {}
.plan-card {}
.plan-card--featured {}
```

Las variables globales se centralizan utilizando Custom Properties en la raíz[cite: 4]:
```css
:root {
  --color-primary: #27AE60;
  --color-secondary: #0B3B60;
  --color-accent: #F39C12;
}
```

**Convenciones JavaScript**
*   `camelCase` para variables y funciones.
*   `const` como declaración predeterminada; `let` únicamente para variables reasignables.
*   Nombres de funciones y variables en inglés.
*   Separación de funcionalidades mediante bloques lógicos (ej. inicialización de i18n, carrusel).
*   Manejo de eventos con `addEventListener`[cite: 4].

**Convenciones C# (.NET Core) para futuros Sprints**
*   Indentación de 4 espacios (estilo Allman para llaves).
*   `PascalCase` para clases, métodos y propiedades públicas.
*   Prefijo `I` seguido de `PascalCase` para interfaces (ej. `IShipmentService`).
*   `camelCase` para parámetros y variables locales.

### 5.1.4. Software Deployment Configuration

La primera versión de la Landing Page de AgroFlet se despliega utilizando GitHub Pages. El deployment utiliza el contenido estático alojado en la rama `main` del repositorio.

#### Procedimiento de despliegue
1.  Integrar los cambios aprobados desde `develop` hacia la rama de release correspondiente.
2.  Validar localmente la versión.
3.  Integrar la release en `main`.
4.  Crear el tag correspondiente mediante Semantic Versioning (`v1.0.0`).
5.  Ingresar a `Settings > Pages` en el repositorio de GitHub.
6.  Seleccionar `Deploy from a branch`, especificando la rama `main` y la carpeta `/root`.
7.  Guardar la configuración y validar la URL pública generada.

**Evidencia de Configuración:**

<p align="center">
  <img src="assets/images/github-pages-settings.png" alt="Configuración de GitHub Pages" title="Configuración GitHub Pages" width="600">
</p>

---

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1

| Sprint # | Sprint 1 |
| :--- | :--- |
| **Date** | 02/09/2026 |
| **Time** | 10:00 AM |
| **Location** | Google Meet |
| **Prepared By** | Jose Alejandro Tello Lima |
| **Attendees** | César Alca, Adriano Centeno, Bernie Rivas, Christoper Rivas, Jose Tello |
| **Sprint Goal** | Implementar y desplegar la primera versión funcional y responsive de la Landing Page de AgroFlet, comunicando la propuesta de valor del producto, sus funcionalidades proyectadas, planes, equipo y contenido institucional, incorporando navegación responsive, internacionalización (ES/EN) y elementos interactivos demostrativos. |
| **Sprint Velocity** | 24 Story Points |

#### 5.2.1.2. Aspect Leaders and Collaborators

| Aspecto | Líder | Colaboradores |
| :--- | :--- | :--- |
| **Landing Page UX/UI** | Bernie Rivas | Christoper Rivas, Jose Tello |
| **HTML Structure** | César Alca | Adriano Centeno |
| **CSS & Responsive Design** | Jose Tello | César Alca, Bernie Rivas |
| **JavaScript Interactions** | Adriano Centeno | Christoper Rivas |
| **Internationalization (i18n)** | Christoper Rivas | Jose Tello |
| **Documentation** | César Alca | Todo el equipo |
| **Deployment & SCM** | Jose Tello | Adriano Centeno |

#### 5.2.1.3. Sprint Backlog 1

| ID | Tarea | Story Points | Responsable | Estado |
| :---: | :--- | :---: | :--- | :---: |
| **US24** | Implementar presentación de la propuesta de valor (Hero) | 3 | César Alca | Done |
| **US25** | Implementar sección informativa de funcionalidades | 3 | Bernie Rivas | Done |
| **US26** | Implementar presentación de planes de suscripción | 3 | Adriano Centeno | Done |
| **US27** | Implementar sección de testimonios en carrusel | 3 | Christoper Rivas | Done |
| **US29** | Implementar navegación responsive (Header & Footer) | 5 | Jose Tello | Done |
| **US30** | Implementar cambio de idioma dinámico ES/EN (i18n) | 5 | Christoper Rivas | Done |
| **US33** | Implementar documento HTML de términos del servicio | 2 | Bernie Rivas | Done |

#### 5.2.1.4. Development Evidence for Sprint Review

Durante el Sprint 1 se implementó la primera versión funcional de la Landing Page de AgroFlet. Las principales funcionalidades desarrolladas incluyen: navegación responsive mediante anchors, menú hamburguesa para móviles, Hero principal con efectos visuales, sección de planes (`plan-card`), carrusel interactivo de testimonios, internacionalización dinámica mediante archivos JSON (`en.json`, `es.json`), y un modal de autenticación demostrativo[cite: 4].

> *Nota: La autenticación incluida en esta versión es exclusivamente demostrativa (ejecutada en el cliente) y no se encuentra integrada con el RESTful API.*

**Evidencia de Desarrollo (Código Fuente):**

*A continuación se presentan capturas del código fuente alojado en el repositorio local.*

**1. Estructura HTML Semántica y atributos i18n (`index.html`)**
*(Tomar captura en VS Code del archivo index.html, enfocando la sección del header o hero, mostrando los `data-i18n` y guardarla como `assets/images/code-html-hero.png`)*
<p align="center">
  <img src="assets/images/code-html-hero.png" alt="HTML Development" title="HTML Code Structure" width="600">
</p>

**2. Convenciones BEM y Variables CSS (`styles.css`)**
*(Tomar captura en VS Code del archivo styles.css, mostrando el bloque `:root` con los colores de AgroFlet o la clase `.plan-card`, y guardarla como `assets/images/code-css-bem.png`)*
<p align="center">
  <img src="assets/images/code-css-bem.png" alt="CSS Development" title="CSS Variables and BEM" width="600">
</p>

**3. Lógica JavaScript para Internacionalización (`app.js`)**
*(Tomar captura en VS Code del archivo app.js, mostrando la función que cambia el idioma cargando los JSON, y guardarla como `assets/images/code-js-i18n.png`)*
<p align="center">
  <img src="assets/images/code-js-i18n.png" alt="JavaScript Development" title="JS i18n Implementation" width="600">
</p>

**4. Estructura del Entorno de Desarrollo**
*(Se evidencia la estructura de carpetas `assets/`, `css/`, `i18n/`, `js/` según lo configurado en el entorno local)*
<p align="center">
  <img src="assets/images/vscode-explorer-structure.png" alt="VS Code Explorer" title="Project Folder Structure" width="300">
</p>

#### 5.2.1.5. Execution Evidence for Sprint Review

Se verificó la correcta ejecución de la Landing Page en navegadores de escritorio y mediante Chrome DevTools para garantizar el comportamiento responsive.

**Vista Desktop - Hero Section & Navegación**
*(Tomar captura de la web renderizada en pantalla completa en PC y guardarla como `assets/images/execution-desktop.png`)*
<p align="center">
  <img src="assets/images/execution-desktop.png" alt="Desktop Execution" title="AgroFlet Desktop View" width="600">
</p>

**Vista Mobile - Responsive Menu & Planes**
*(Tomar captura de la web renderizada en modo móvil desde DevTools y guardarla como `assets/images/execution-mobile.png`)*
<p align="center">
  <img src="assets/images/execution-mobile.png" alt="Mobile Execution" title="AgroFlet Mobile View" width="300">
</p>

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

Durante el Sprint 1 la Landing Page no consume todavía el RESTful API de AgroFlet ni servicios externos. Las funcionalidades interactivas (como el modal de autenticación o el cambio de idioma) corresponden a una demostración ejecutada en el cliente mediante JavaScript.

La integración con los servicios RESTful internos y la provisión de la documentación OpenAPI (Swagger) se incorporará en los siguientes Sprints una vez se inicie el desarrollo del Backend con ASP.NET Core.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

La versión `v1.0.0` de la Landing Page fue publicada utilizando GitHub Pages.

**Repositorio:** `[ENLACE A TU REPOSITORIO GITHUB]`
**Landing Page desplegada:** `[ENLACE A LA PÁGINA PUBLICADA]`

**Evidencia del deployment en producción:**
*(Tomar captura de la web cargada desde la URL pública de GitHub Pages y guardarla como `assets/images/deployment-production.png`)*
<p align="center">
  <img src="assets/images/deployment-production.png" alt="AgroFlet Deployment" title="AgroFlet Production URL" width="600">
</p>

#### 5.2.1.8. Team Collaboration Insights during Sprint

El trabajo colaborativo se organizó mediante ramas funcionales (`feature/*`), permitiendo que el equipo de AgroFlet desarrollara componentes en paralelo sin generar conflictos directos.

Las integraciones hacia la rama `develop` y posteriormente a `main` se realizaron mediante Pull Requests. Esta estrategia permitió mantener un estricto control de calidad, asegurando que funcionalidades críticas como el sistema multilingüe (i18n) y la adaptabilidad móvil fueran revisadas antes de su pase a producción.

**Evidencia de Colaboración en GitHub (Pull Requests / Commits):**
*(Tomar captura de la pestaña 'Pull requests' o de la gráfica de 'Contributors' en GitHub y guardarla como `assets/images/github-collaboration.png`)*
<p align="center">
  <img src="assets/images/github-collaboration.png" alt="Team Collaboration" title="GitHub PRs and Commits" width="600">
</p>
