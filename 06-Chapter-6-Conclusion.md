# Conclusiones y recomendaciones

## Conclusiones

### AV1

1. **Comprensión del problema y de los usuarios.** Las entrevistas, el análisis competitivo y los artefactos de Needfinding permitieron identificar dificultades de comunicación y visibilidad entre los productores o acopiadores que despachan productos agrícolas y los compradores mayoristas que los reciben. Estos hallazgos orientaron la propuesta de AgroFlet hacia la consulta del estado de los envíos y el registro de información compartida. La investigación inicial sustenta la pertinencia del problema; la reducción de mermas y tiempos de espera deberá evaluarse mediante pruebas con usuarios y datos de operaciones reales.

2. **Relación entre requisitos y diseño.** Las User Stories, el Product Backlog, el Impact Mapping y los prototipos permitieron relacionar las necesidades identificadas con las funcionalidades previstas. El diseño de arquitectura mediante Domain-Driven Design, EventStorming y diagramas C4 estableció una separación de responsabilidades para identidad y acceso, recursos de transporte, operaciones, seguimiento e incidencias. Estos artefactos constituyen una guía para la implementación y deben actualizarse conforme evoluciona el producto.

3. **Primera implementación de la presencia web.** El Sprint 1 permitió publicar la primera Landing Page de AgroFlet y establecer el trabajo colaborativo mediante Git y GitHub. La página presentó la propuesta de valor, las funcionalidades, los planes, el equipo y los videos del producto, incorporando adaptación a distintos tamaños de pantalla e intercambio de idioma. Esta entrega proporcionó una base para comunicar el proyecto y continuar con el desarrollo de la aplicación.

### TB1

1. **Primera versión funcional de la Web Application.** Durante el Sprint 2, el equipo implementó una Single-Page Application con Vue, Vite y PrimeVue, organizada en módulos y componentes compartidos. Las evidencias de ejecución muestran recorridos de acceso, gestión de vehículos y conductores, consulta y registro de envíos, visualización de posiciones reportadas, incidencias y configuración de usuario. Esta versión permite demostrar los flujos previstos para despachadores y compradores, sin acreditar todavía su operación en condiciones reales de transporte agrícola.

2. **Integración con servicios simulados y límites del alcance.** La aplicación consume una Fake API basada en `json-server`, cuyo contrato se documentó con OpenAPI 3.0.3. Este recurso facilitó la integración y demostración del frontend antes de completar el backend definitivo. La autenticación demostrativa, las validaciones del cliente y las posiciones registradas permiten evaluar la interacción, pero no constituyen evidencia de autorización segura en el servidor, telemetría GPS continua o funcionamiento de un RESTful API productivo desarrollado con ASP.NET Core.

3. **Publicación y acceso a los entregables.** La Web Application se publicó en Vercel y GitHub Pages, mientras que la Landing Page V2 mantiene su publicación en GitHub Pages. Las evidencias de configuración, ejecución y despliegue permiten consultar los productos y reproducir sus recorridos. La actualización de la landing incorporó el formulario de contacto UH28 después de los videos. Su almacenamiento en el navegador permite demostrar el registro de datos, pero todavía requiere un servicio de recepción para atender solicitudes fuera del dispositivo del visitante.

4. **Colaboración y trazabilidad del Sprint 2.** La distribución de responsables, el Sprint Backlog 2, las ramas de trabajo y los commits permitieron relacionar los aportes de los cinco integrantes con los entregables. La documentación de desarrollo, ejecución, servicios y despliegue complementa el código y facilita la revisión del trabajo realizado. La integración de estos aportes permitió avanzar desde la landing inicial hacia una aplicación web demostrable, conservando las evidencias de AV1 y ampliando el informe para TB1.

5. **Validación pendiente del impacto del producto.** Los resultados de TB1 muestran avances de implementación y publicación, pero aún no permiten concluir que AgroFlet reduzca pérdidas económicas, mejore el ETA o disminuya los tiempos de espera en operaciones reales. La siguiente etapa debe contrastar los recorridos implementados con usuarios de ambos segmentos y medir resultados antes de atribuir beneficios operativos a la solución.

---

## Recomendaciones

1. **Completar el backend y aplicar las reglas en el servidor.** Priorizar la implementación del RESTful API definitivo conforme al backlog y a los contratos revisados. Incorporar autenticación, autorización por rol y por operación, validación de solicitudes y persistencia de datos. Las pruebas deben comprobar que un usuario no pueda consultar ni modificar envíos ajenos y que los estados de las operaciones y la disponibilidad de vehículos y conductores se mantengan coherentes.

2. **Mantener consistentes el contrato y las evidencias de servicios.** Actualizar la documentación OpenAPI cuando cambien rutas, esquemas o respuestas y diferenciar expresamente los servicios simulados de los implementados en el backend. Documentar y verificar la persistencia del entorno desplegado, incluidos sus límites y comportamiento ante reinicios. Conservar instrucciones reproducibles de configuración local y publicación para facilitar la integración del equipo.

3. **Validar los flujos con los dos segmentos objetivo.** Realizar sesiones de evaluación con despachadores y compradores mayoristas para observar tareas como registrar un envío, localizar su estado, consultar una incidencia y confirmar la información de recepción. Registrar dificultades, tasa de finalización y tiempo por tarea, y utilizar estos resultados para priorizar mejoras de usabilidad y accesibilidad. Los beneficios sobre mermas y tiempos de espera deben evaluarse posteriormente mediante un piloto con operaciones reales.

4. **Evolucionar el seguimiento con un alcance explícito.** Distinguir en la interfaz la ruta planificada, la última posición reportada y la fecha de actualización. Antes de incorporar seguimiento automático o recálculo del ETA, definir el origen de los datos, los permisos de ubicación, la frecuencia de actualización y el comportamiento ante pérdida de conectividad. Probar estas capacidades sin presentar datos simulados como mediciones de un vehículo en tiempo real.

5. **Conectar el formulario de contacto con un servicio de recepción.** Sustituir el almacenamiento exclusivamente local por un endpoint que permita recibir y gestionar las solicitudes. Incorporar validación en el servidor, consentimiento informado, controles contra envíos abusivos y mensajes de éxito o error que reflejen el resultado real. Mantener su ubicación después de los videos y comprobar su funcionamiento en ambos idiomas y en dispositivos móviles.

6. **Reforzar la calidad antes de cada integración y despliegue.** Verificar los recorridos críticos de IAM, flota, envíos e incidencias, además de la navegación directa a rutas, la internacionalización y la adaptación móvil. Mantener los cambios revisables mediante Pull Requests hacia `develop` y publicar en `main` las versiones verificadas. Registrar el commit desplegado y las evidencias correspondientes para evitar diferencias entre el código, el informe y la aplicación publicada.

7. **Actualizar el informe junto con el producto.** Revisar el Sprint Backlog, los diagramas, las evidencias y las conclusiones en cada entrega, identificando las funcionalidades completadas y las pendientes. Conservar los cortes históricos de colaboración con sus fechas y alcance, sin confundir cifras acumuladas con aportes exclusivos de un sprint. Priorizar futuras capacidades, como guías de remisión, reportes o suscripciones, a partir de las necesidades comprobadas y de la estabilidad de los flujos principales.
