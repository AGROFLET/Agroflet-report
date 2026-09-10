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
| **Landing Page Deployment** | GitHub Pages | SaaS | Se utiliza para publicar la Landing Page directamente desde el repositorio de GitHub, sin depender de servicios externos adicionales. |
| **Acceptance Test Specification** | Gherkin .feature files | Local / GitHub | Se utilizarán para documentar los criterios de aceptación mediante escenarios escritos en lenguaje Gherkin, vinculados a las User Stories del proyecto. |
| **Acceptance Test Automation** | Cucumber | Local | Se utilizará para interpretar y ejecutar los archivos .feature, permitiendo validar escenarios funcionales definidos en lenguaje Gherkin. |
| **Runtime Environment** | Node.js / npm | Local | Se utilizará para gestionar la instalación y ejecución de dependencias del proyecto, especialmente Cucumber y scripts asociados a pruebas automatizadas. |
| **Browser Testing** | Google Chrome / DevTools | Local | Se utiliza para inspeccionar la Landing Page, validar el comportamiento responsive, revisar consola y analizar interacciones del usuario. |
| **HTML/CSS Validation Support** | W3C Markup Validator / W3C CSS Validator | Web | Se utilizarán como apoyo para verificar la correcta estructura del código HTML y CSS, alineando el desarrollo con buenas prácticas web. |

El entorno seleccionado permite mantener coherencia entre el diseño elaborado en Figma y la implementación web desarrollada por el equipo. Visual Studio Code, Live Server y DevTools facilitan la construcción y validación local del producto; Git y GitHub permiten asegurar trazabilidad de cambios; GitHub Pages permite publicar la solución final directamente desde el repositorio; y la combinación de Gherkin + Cucumber permite documentar y ejecutar pruebas de aceptación asociadas a los requerimientos funcionales del proyecto. En ese sentido, los archivos .feature constituyen la especificación funcional de los escenarios de prueba, mientras que Cucumber actúa como herramienta de interpretación y ejecución de dichos escenarios, fortaleciendo la validación del comportamiento esperado del sistema.

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

Las convenciones de código de la Landing Page se alinean con los lineamientos visuales ya definidos en el Capítulo IV (Style Guidelines), en particular la identidad de marca, la paleta de colores oficial y la tipografía corporativa de AgroFlet.

**Identidad de marca**

<p align="center">
  <img src="assets/images/LogoOfi.png" alt="Isotipo AgroFlet" title="Isotipo AgroFlet" width="400">
</p>

**Tipografía:** familia **Inter**, con jerarquías estrictas (Headings en SemiBold, Body en Regular).

<p align="center">
  <img src="assets/images/Inter sans serif.jpeg" alt="Tipografía Inter" title="Tipografía Inter" width="500">
</p>

**Paleta de colores** utilizada como variables CSS en toda la Landing Page:

<p align="center">
  <img src="assets/images/Agroflet coolors.png" alt="Paleta de colores AgroFlet" title="Paleta de colores AgroFlet" width="500">
</p>

```css
:root {
  --color-primary: #27AE60;   /* Verde AgroFlet */
  --color-secondary: #0B3B60; /* Azul Marino Corporativo */
  --color-accent: #F39C12;    /* Naranja Ruta */
  --color-error: #D32F2F;     /* Error/Crítico */
  --color-bg: #F8F9FA;        /* Neutral fondo */
  --color-text: #212529;      /* Neutral texto base */
  --font-family-base: 'Inter', sans-serif;
}
```

> `[Insertar las convenciones específicas que el equipo acuerde para nomenclatura de archivos, clases CSS y funciones JavaScript]`

### 5.1.4. Software Deployment Configuration

La Landing Page de Agroflet se despliega mediante **GitHub Pages**, publicando directamente el contenido estático (HTML5, CSS3 y JavaScript) desde el repositorio del proyecto, sin necesidad de servicios de hosting externos.

> `[Insertar rama utilizada para el despliegue (main o gh-pages), la URL pública generada por GitHub Pages y una captura del panel de Settings > Pages del repositorio]`

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1

El Sprint 1 toma como base la estructura definida en los wireframes de la Landing Page (Capítulo IV), priorizando la implementación de la sección Hero, beneficios, planes de suscripción y formulario de contacto.

**Wireframes Desktop (estructura base a implementar)**

![Landing Wireframe Desktop 1](assets/images/Landing_Desktop1.png)
![Landing Wireframe Desktop 2](assets/images/Landing_Desktop2.png)
![Landing Wireframe Desktop 3](assets/images/Landing_Desktop3.png)
![Landing Wireframe Desktop 4](assets/images/Landing_Desktop4.png)
![Landing Wireframe Desktop 5](assets/images/Landing_Desktop5.png)
![Landing Wireframe Desktop 6](assets/images/Landing_Desktop6.png)
![Landing Wireframe Desktop 7](assets/images/Landing_Desktop7.png)

**Wireframes Mobile (estructura base a implementar)**

![Landing Wireframe Mobile 1](assets/images/Landing_MobileW1.png)
![Landing Wireframe Mobile 2](assets/images/Landing_MobileW2.png)
![Landing Wireframe Mobile 3](assets/images/Landing_MobileW3.png)
![Landing Wireframe Mobile 4](assets/images/Landing_MobileW4.png)
![Landing Wireframe Mobile 5](assets/images/Landing_MobileW5.png)
![Landing Wireframe Mobile 6](assets/images/Landing_MobileW6.png)
![Landing Wireframe Mobile 7](assets/images/Landing_MobileW7.png)

> `[Insertar Sprint Goal, fecha de inicio/fin y captura del tablero de Trello con el Sprint Backlog]`

#### 5.2.1.2. Aspect Leaders and Collaborators

| Aspecto | Líder | Colaboradores |
| :--- | :--- | :--- |
| `[Insertar aspecto]` | `[Insertar nombre]` | `[Insertar nombres]` |
| `[Insertar aspecto]` | `[Insertar nombre]` | `[Insertar nombres]` |
| `[Insertar aspecto]` | `[Insertar nombre]` | `[Insertar nombres]` |

#### 5.2.1.3. Sprint Backlog 1

| User Story / Tarea | Story Points | Responsable | Estado |
| :--- | :--- | :--- | :--- |
| `[Insertar tarea]` | `[Insertar]` | `[Insertar]` | `[Insertar]` |
| `[Insertar tarea]` | `[Insertar]` | `[Insertar]` | `[Insertar]` |
| `[Insertar tarea]` | `[Insertar]` | `[Insertar]` | `[Insertar]` |

#### 5.2.1.4. Development Evidence for Sprint Review

El desarrollo de esta sección del Sprint traduce a código HTML5, CSS3 y JavaScript los siguientes mockups de alta fidelidad, elaborados en el Capítulo IV:

**Mockups Desktop (diseño de referencia implementado)**

![Landing Mockup Desktop 1](assets/images/Landing_DesktopM1.png)
![Landing Mockup Desktop 2](assets/images/Landing_DesktopM2.png)
![Landing Mockup Desktop 3](assets/images/Landing_DesktopM3.png)
![Landing Mockup Desktop 4](assets/images/Landing_DesktopM4.png)
![Landing Mockup Desktop 5](assets/images/Landing_DesktopM5.png)
![Landing Mockup Desktop 6](assets/images/Landing_DesktopM6.png)
![Landing Mockup Desktop 7](assets/images/Landing_DesktopM7.png)

> `[Insertar captura del código fuente en VS Code y de los commits en GitHub asociados a la implementación de estas secciones]`

#### 5.2.1.5. Execution Evidence for Sprint Review

La validación de la Landing Page en dispositivos móviles se realiza contrastando la ejecución real con los siguientes mockups mobile del Capítulo IV:

**Mockups Mobile (diseño de referencia para validación responsive)**

![Landing Mockup Mobile 1](assets/images/Landing_MobileM1.png)
![Landing Mockup Mobile 2](assets/images/Landing_MobileM2.png)
![Landing Mockup Mobile 3](assets/images/Landing_MobileM3.png)
![Landing Mockup Mobile 4](assets/images/Landing_MobileM4.png)
![Landing Mockup Mobile 5](assets/images/Landing_MobileM5.png)
![Landing Mockup Mobile 6](assets/images/Landing_MobileM6.png)
![Landing Mockup Mobile 7](assets/images/Landing_MobileM7.png)

> `[Insertar captura de la Landing Page ejecutándose en Live Server / navegador y de DevTools validando los breakpoints]`

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

> `[Insertar documentación del servicio consumido por la Landing Page en este Sprint (ej. envío del formulario de contacto), o indicar explícitamente si el Sprint 1 no consumió ningún servicio externo]`

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

> `[Insertar captura del despliegue generado en GitHub Pages y la URL pública resultante]`

#### 5.2.1.8. Team Collaboration Insights during Sprint

> `[Insertar una reflexión breve del equipo sobre la colaboración durante el Sprint 1: dificultades, coordinación entre responsables y aprendizajes]`
