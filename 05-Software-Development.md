# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration
Para la implementación de Agroflet se configuró un entorno de desarrollo orientado a la construcción, validación, versionamiento y despliegue de una Landing Page funcional. De acuerdo con los lineamientos del proyecto, la solución web se desarrolla utilizando HTML5 y CSS3 como base obligatoria, manteniendo un comportamiento 100% responsive y empleando JavaScript únicamente como apoyo para interacciones simples de la interfaz. Asimismo, el entorno considera herramientas de diseño UX/UI, gestión de tareas, control de versiones, especificación de pruebas de aceptación y despliegue web.

| Actividad | Herramienta | Tipo | Uso en el proyecto |
| :--- | :--- | :--- | :--- |
| **Project Management** | Trello | SaaS | Se utilizará para organizar el Sprint Backlog, asignar tareas, hacer seguimiento del avance del equipo y evidenciar la gestión iterativa del proyecto. |
| **Product UX/UI Design** | Figma | SaaS | Se emplea para diseñar y consultar wireframes, mockups, prototipos y lineamientos visuales que guían la implementación de la Landing Page. |
| **Software Development** | Visual Studio Code | Local | Se utiliza como editor principal para desarrollar los archivos HTML, CSS y JavaScript del proyecto. |
| **Local Web Execution** | Live Server | Extensión local de VS Code | Se utiliza para ejecutar localmente la Landing Page durante el desarrollo y validar cambios en tiempo real. |
| **Source Code Versioning** | Git | Local | Se utiliza mediante terminal para registrar cambios, administrar ramas y sincronizar el código fuente del proyecto. |
| **Source Code Repository** | GitHub | SaaS | Se utiliza como repositorio remoto para alojar el código fuente, controlar versiones y centralizar los archivos del proyecto. |
| **Acceptance Test Specification** | Gherkin .feature files | Local / GitHub | Se utilizarán para documentar los criterios de aceptación mediante escenarios escritos en lenguaje Gherkin, vinculados a las User Stories del proyecto. |
| **Acceptance Test Automation** | Cucumber | Local | Se utilizará para interpretar y ejecutar los archivos .feature, permitiendo validar escenarios funcionales definidos en lenguaje Gherkin. |
| **Runtime Environment** | Node.js / npm | Local | Se utilizará para gestionar la instalación y ejecución de dependencias del proyecto, especialmente Cucumber y scripts asociados a pruebas automatizadas. |
| **Browser Testing** | Google Chrome / DevTools | Local | Se utiliza para inspeccionar la Landing Page, validar el comportamiento responsive, revisar consola y analizar interacciones del usuario. |
| **HTML/CSS Validation Support** | W3C Markup Validator / W3C CSS Validator | Web | Se utilizarán como apoyo para verificar la correcta estructura del código HTML y CSS, alineando el desarrollo con buenas prácticas web. |

El entorno seleccionado permite mantener coherencia entre el diseño elaborado en Figma y la implementación web desarrollada por el equipo. Visual Studio Code, Live Server y DevTools facilitan la construcción y validación local del producto; Git y GitHub permiten asegurar trazabilidad de cambios; Vercel permite publicar la solución final; y la combinación de Gherkin + Cucumber permite documentar y ejecutar pruebas de aceptación asociadas a los requerimientos funcionales del proyecto. En ese sentido, los archivos .feature constituyen la especificación funcional de los escenarios de prueba, mientras que Cucumber actúa como herramienta de interpretación y ejecución de dichos escenarios, fortaleciendo la validación del comportamiento esperado del sistema.

### 5.1.2. Source Code Management
Para la gestión del código fuente de Agroflet se utiliza Git como sistema de control de versiones y GitHub como plataforma de alojamiento remoto del repositorio. Esta configuración permite mantener trazabilidad sobre los cambios realizados en la Landing Page, organizar el trabajo colaborativo del equipo y conservar un historial verificable de la evolución del producto.

El repositorio principal del proyecto es el siguiente:
* **Repositorio del Landing Page y pruebas de aceptación:** https://github.com/-------------

En este mismo repositorio se almacenará tanto el código fuente de la Landing Page como los archivos de pruebas de aceptación en formato .feature. Para ello, se utilizará una carpeta específica denominada `features/`, ubicada en la raíz del proyecto. Esta decisión permite mantener en un mismo espacio la implementación web y los escenarios de aceptación asociados a las User Stories del producto.

La estructura general esperada del repositorio será la siguiente:

```text
Agroflet/
├── index.html
├── css/
├── js/
├── recursos/
├── features/
│   ├── landing/
│   │   ├── landing-navigation.feature
│   │   ├── landing-sections.feature
│   │   ├── contact-form.feature
│   │   ├── login-access.feature
│   │   └── mobile-demo.feature
│   ├── mobile-core/
│   │   ├── epic-01-yy.feature
│   │   ├── epic-02-yy.feature
│   │   ├── epic-x3-yy.feature
│   │   ├── epic-x4-yy.feature
│   │   ├── epic-x5-yy.feature
│   │   └── epic-x6-yy.feature
│   └── step_definitions/
│       └── landing.steps.js
├── package.json
├── package-lock.json
├── .gitignore
└── README.md
```
### 5.1.3. Source Code Style Guide & Conventions

### 5.1.4. Software Deployment Configuration

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1

#### 5.2.1.2. Aspect Leaders and Collaborators

#### 5.2.1.3. Sprint Backlog 1

#### 5.2.1.4. Development Evidence for Sprint Review

#### 5.2.1.5. Execution Evidence for Sprint Review

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

#### 5.2.1.8. Team Collaboration Insights during Sprint
