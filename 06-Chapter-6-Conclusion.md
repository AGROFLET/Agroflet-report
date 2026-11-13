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

### AV2

1. **Transición efectiva hacia una arquitectura Full-Stack desplegada.** Durante el Sprint 3, el equipo concretó el desarrollo, integración y despliegue de la primera versión productiva de los Web Services RESTful en ASP.NET Core 8 (C#) con persistencia relacional en MySQL, superando la dependencia exclusiva de entornos simulados. La conexión efectiva entre la nueva versión de la Single-Page Application (Vue.js) y el servidor propio valida la coherencia del diseño modular basado en Domain-Driven Design (DDD), asegurando la aplicación real de reglas de negocio, autenticación JWT y control de acceso por roles en el servidor.

2. **Trazabilidad documental de servicios y despliegue continuo.** La elaboración de la especificación técnica de los Web Services (OpenAPI/Swagger), sumada a las evidencias de ejecución y despliegue continuo de las nuevas versiones de la Landing Page, la Web Application y el Backend API, establece un ecosistema accesible y reproducible. Este hito cierra la brecha entre los contratos arquitectónicos proyectados en etapas previas y el código ejecutándose en entornos en la nube.

3. **Retroalimentación empírica mediante validación con usuarios y heurísticas.** La ejecución de las entrevistas de validación sobre el producto desplegado con representantes de ambos segmentos objetivo (despachadores y compradores mayoristas), complementada con las evaluaciones de usabilidad basadas en principios heurísticos, aportó evidencia directa sobre la claridad de la navegación y la utilidad percibida del seguimiento de envíos e incidencias. Asimismo, estos ejercicios revelaron oportunidades de ajuste en la visualización de información móvil y formularios operativos, las cuales retroalimentan el backlog sin asumir aún métricas concluyentes de reducción de mermas a escala comercial.

4. **Comunicación integral del producto y cohesión del equipo.** La producción y publicación de las primeras versiones del *Video About-the-Product* y del *Video About-the-Team*, junto con el seguimiento del Sprint Backlog 3 y las métricas de colaboración en GitHub, consolidaron tanto la propuesta de valor comercial como la trazabilidad del desempeño individual y grupal. Esto garantiza un producto comprensible para evaluadores y potenciales usuarios, respaldado por un proceso de ingeniería ordenado.

---

## Recomendaciones

1. **Consolidar el endurecimiento de seguridad y pruebas automatizadas en el Backend.** Con la primera versión de los Web Services desplegada, se recomienda ampliar la cobertura de pruebas unitarias y de integración en ASP.NET Core 8. Es prioritario validar exhaustivamente las políticas de autorización entre distintos usuarios (asegurando el aislamiento de datos entre despachadores y compradores) y manejar de forma controlada las excepciones de concurrencia y disponibilidad de flota en la base de datos MySQL.

2. **Incorporar los hallazgos de las entrevistas y evaluaciones heurísticas en el próximo Sprint.** Priorizar la resolución de las observaciones detectadas durante las sesiones de validación (como la optimización del consumo de datos en vistas móviles para ruta, la persistencia de filtros en el historial y la inclusión de campos complementarios como referencias de guías de remisión o contacto de copiloto). Mantener el criterio de priorización basado en el impacto operativo real sobre el usuario final.

3. **Evolucionar la telemetría y el manejo de conectividad intermitente.** Dado que el transporte agrícola interprovincial atraviesa zonas sin cobertura celular estable, se sugiere implementar mecanismos de almacenamiento en caché local y sincronización diferida en la aplicación web progresiva (PWA) para el registro de incidencias y reportes de posición. Asimismo, mantener explícita en la interfaz la diferencia entre la ruta planificada y el último reporte recibido hasta integrar proveedores GPS en tiempo real.

4. **Automatizar el flujo completo del formulario de contacto y notificaciones transaccionales.** Con el backend operativo, se recomienda vincular definitivamente el formulario de contacto de la Landing Page y las alertas críticas de incidencias con servicios externos de mensajería (como SendGrid o Firebase Cloud Messaging), asegurando que las notificaciones lleguen de manera efectiva fuera del navegador del usuario y con validaciones robustas en el servidor.

5. **Refinar los artefactos audiovisuales y preparar un piloto en campo.** Utilizar la retroalimentación recibida sobre las primeras versiones del *Video About-the-Product* y *Video About-the-Team* para pulir la narrativa, claridad técnica y demostración de flujos de cara al cierre del proyecto. Paralelamente, planificar una prueba piloto acotada con un despacho real entre centro de acopio y mercado mayorista para recopilar métricas reales de tiempos de espera y cumplimiento de ETA.

6. **Mantener la disciplina de integración continua y sincronización documental.** Conservar el flujo de trabajo basado en GitFlow con revisiones cruzadas en cada Pull Request antes de actualizar las ramas productivas (`main`). Asegurar que cada despliegue de frontend, landing page o web services quede registrado con su respectiva versión, commit y documentación OpenAPI actualizada para evitar desviaciones entre el informe final y el software publicado.
