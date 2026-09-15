# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

La Gestión de Configuración de Software (SCM) establece las herramientas, convenciones y mecanismos de versionamiento utilizados por el equipo de AgroFlet para mantener la trazabilidad y consistencia de los artefactos desarrollados a lo largo del ciclo de vida del proyecto.

Durante el Sprint 1 se priorizó la implementación y despliegue de la primera versión de la Landing Page de AgroFlet, desarrollada mediante HTML5, CSS3 y JavaScript.

### 5.1.1. Software Development Environment Configuration

A continuación se listan los productos de software utilizados por el equipo, organizados por tipo de actividad, incluyendo las herramientas de arquitectura y gestión solicitadas.

| Actividad | Herramienta | Uso en AgroFlet |
| :--- | :--- | :--- |
| **Project Management** | Jira | Organización del Sprint Backlog, asignación de responsables y seguimiento de tareas ágiles. |
| **Communication** | Google Meet | Coordinación asincrónica, reuniones diarias (Daily Scrum) y revisiones de Sprint. |
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
`https://github.com/AgroFlet-Team/agroflet-landing-page` *(Reemplazar con URL real)*

Posteriormente, el ecosistema de AgroFlet contará con repositorios independientes para los demás productos que conforman la solución distribuida:
- Landing Page
- Frontend Web Application
- RESTful API
- Project Report

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
