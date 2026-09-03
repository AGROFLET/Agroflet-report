# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup
AgroFlet es una startup tecnológica peruana que está orientada a transformar la visibilidad, el control y la trazabilidad del transporte terrestre de alimentos a nivel nacional. Su propuesta de valor se centra en el monitoreo digital de productos agrícolas y alimentos perecibles como tubérculos, frutas, hortalizas, granos y otros productos que requieren seguimiento continuo durante su traslado desde las zonas de producción hasta los centros de distribución y comercialización.

Nuestro país, Perú, cuenta con una gran diversidad agroproductiva de la región. Según el Instituto Nacional de Estadística e Informática (INEI, 2023), la actividad agropecuaria representa aproximadamente el 6 % del Producto Bruto Interno (PBI) nacional y ocupa a más del 28 % de la Población Económicamente Activa (PEA) en zonas rurales. Sin embargo, la cadena logística que conecta la producción con el consumo sigue siendo altamente informal, fragmentada y opaca. El Ministerio de Transportes y Comunicaciones (MTC, 2022) estima que más del 70 % del transporte de carga agrícola se realiza sin sistemas de seguimiento ni trazabilidad digital, lo que genera pérdidas económicas significativas, retrasos no reportados y baja capacidad de respuesta ante incidencias en ruta.

Ante este escenario, AgroFlet propone una plataforma web de monitoreo y gestión logística que centraliza en tiempo casi real la información de cada operación de transporte: el tipo de alimento trasladado, el origen y destino del envío, la hora de salida, la fecha estimada de llegada, la ubicación actual de la unidad y las incidencias que puedan afectar el recorrido. De esta manera, los actores de la cadena —productores, empresas transportistas, compradores mayoristas y gestores logísticos— pueden tomar decisiones informadas, reducir pérdidas y mejorar la eficiencia operativa.

La propuesta de AgroFlet tiene coherencia con las tendencias globales en *agri-tech* y *logistics-tech*. Según el informe de la Organización de las Naciones Unidas para la Alimentación y la Agricultura (FAO, 2022), la digitalización de las cadenas de valor agrícolas puede reducir hasta en un 15 % las pérdidas postcosecha asociadas a problemas logísticos, lo que en el contexto peruano representaría un ahorro económico de cientos de millones de soles anuales. Por su parte, Deloitte (2023) señala que las plataformas de trazabilidad logística en países en desarrollo están creciendo a una tasa anual compuesta (CAGR) superior al 18 %, impulsadas por la demanda de transparencia en la cadena de suministro.

AgroFlet se posiciona inicialmente en el mercado peruano con foco en las principales rutas agrícolas del país —Sierra-Costa y Costa-Lima Metropolitana—, con potencial de escalamiento a nivel regional en el mediano plazo. La plataforma está diseñada para ser accesible desde dispositivos de escritorio y móvil, con una interfaz adaptable que prioriza la simplicidad operativa para usuarios con distintos niveles de alfabetización digital.

**Misión:** Digitalizar y transparentar la cadena logística del transporte de alimentos en el Perú, reduciendo pérdidas, mejorando la eficiencia operativa y contribuyendo a la seguridad alimentaria nacional.

**Visión:** Ser la plataforma de referencia en trazabilidad logística agroalimentaria en América Latina para el año 2030.
### 1.1.2. Perfiles de integrantes del equipo

| Foto | Descripción |
|:---:|:---|
| <img src="../assets/Alca Morán, César Alejandro - U20241F027 - Profile.jpg" alt="Foto" width="120"> | **Alca Morán, César Alejandro - U20241F027**<br>Soy estudiante de Ingeniería de Software. Aporto conocimientos en desarrollo web, programación y trabajo en equipo. Me caracterizo por ser responsable, proactivo y comprometido con el aprendizaje y el desarrollo de nuevas habilidades.|
| <img src="../assets/Centeno León, Adriano Samir - U20241D920 - Profile.jpg" alt="Foto" width="120"> | **Centeno León, Adriano Samir - U20241D920**<br>Estudiante de la carrera de Ingeniería de Software con conocimientos en programación, bases de datos y gestión de proyectos mediante Github. Referente a la gestión de trabajos en equipo, me gusta mantenerme organizado y cumplir con los plazos establecidos. |
| <img src="../assets/Rivas Méndez, Bernie Aarón - U20241F109 - Profile.PNG" alt="Foto" width="120"> | **Rivas Méndez, Bernie Aarón - U20241F109**<br>Soy un estudiante de la carrera de Ingeniería de Software y curso el 5to ciclo de la carrera. En cuanto a los trabajos me gusta revisar y que estén completos a la hora de entregarlos. En cuanto a la programación me gusta ser ordenado y que tenga lógica, por lo cual prefiero programar el BackEnd, pero también hago el FrontEnd.|
| <img src="ruta/a/tu/imagen.jpg" alt="Foto" width="120"> | **Rivas Castillo, Christoper Steven - U202323551**<br>descripción |
| <img src="../assets/Tello Lima, Jose Alejandro - U202421618 - Profile.png" alt="Foto" width="120"> | **Tello Lima, Jose Alejandro - U202421618**<br>Soy estudiante de Ingeniería de Software. Aporto conocimientos en diseño de experiencias de usuario, interfaces web responsivas y mapeo de trayectorias utilizando herramientas como Figma y UXPressia, asegurando que la plataforma sea altamente intuitiva para el cliente. |

## 1.2. Solution Profile

En esta sección se describen las características principales de la solución propuesta, así como su propuesta de valor y modelo de monetización.

**Product Description**

AgroFlet es una plataforma web de monitoreo y gestión logística orientada a transformar la visibilidad, el control y la trazabilidad del transporte terrestre de alimentos y productos agrícolas perecibles en el Perú. La herramienta permite centralizar y registrar en tiempo casi real la información clave de cada viaje, incluyendo la ubicación de la unidad de carga, el tipo de alimento trasladado, los puntos de origen y destino, las horas de salida, las fechas estimadas de llegada y las incidencias que afecten la ruta.

### 1.2.1. Antecedentes y problemática

El transporte de alimentos en el Perú constituye un eslabón crítico y frecuentemente subestimado dentro de la cadena de valor agroalimentaria. A diferencia de sectores como el minero o el manufacturero, donde la logística ha experimentado una digitalización progresiva, el transporte de productos agrícolas continúa operando bajo esquemas tradicionales basados en acuerdos verbales, registros en papel y comunicación telefónica informal (Ministerio de Agricultura y Riego [MIDAGRI], 2022).

La problemática tiene raíces estructurales. Según el Banco Mundial (2021), el Perú presenta un índice de desempeño logístico (*Logistics Performance Index* o LPI) de 2.95 sobre 5.0, ubicándose por debajo del promedio regional latinoamericano de 3.14. Esta brecha logística impacta directamente en la competitividad del sector agrícola, pues el agricultor no puede garantizar tiempos de entrega confiables ni el comprador puede anticiparse a posibles retrasos o mermas en el producto.

Los datos del Instituto Nacional de Estadística e Informática (INEI, 2022) revelan que aproximadamente el 35 % de la producción agrícola peruana se pierde entre la cosecha y el punto de venta, y que una parte significativa de esas pérdidas ocurre durante el transporte, ya sea por demoras, condiciones inadecuadas de la unidad o falta de comunicación entre los actores de la cadena. En términos económicos, esto equivale a pérdidas anuales superiores a los S/ 2,000 millones, según estimaciones del Centro Nacional de Planeamiento Estratégico (CEPLAN, 2023).

A nivel internacional, experiencias como las de plataformas de trazabilidad logística en Brasil (Agrofy), Colombia (TigoUne Agro) o India (Arya.ag) demuestran que la digitalización del monitoreo del transporte agrícola puede reducir las pérdidas postcosecha en un rango del 10 % al 20 % y mejorar los ingresos de los pequeños agricultores hasta en un 25 %, según la Organización de las Naciones Unidas para la Alimentación y la Agricultura (FAO, 2022). Sin embargo, estas soluciones no se han adaptado al contexto peruano, el cual presenta características particulares: una geografía accidentada con tramos de sierra que dificultan la conectividad, una alta informalidad en el sector transporte y un ecosistema de pequeños y medianos transportistas que operan de manera independiente.


Para estructurar de manera rigurosa la descripción de la problemática, el equipo aplicó la técnica de análisis 5W's + 2H's:

*   **Who (¿Quiénes son los afectados?)**
    Los principales actores afectados por la problemática son:
    *   **Productores agrícolas y cooperativas:** Agricultores individuales o asociados que despachan sus productos desde zonas de producción (Ayacucho, Junín, La Libertad, Puno, entre otras) hacia mercados mayoristas y minoristas, principalmente en Lima Metropolitana. Según el Ministerio de Agricultura y Riego (MIDAGRI, 2022), el 78 % de las unidades agropecuarias en el Perú tienen menos de 5 hectáreas, lo que evidencia el perfil predominantemente pequeño y mediano del productor peruano.
    *   **Empresas y operadores de transporte terrestre:** Transportistas formales e informales que prestan el servicio de flete agrícola. Según el Ministerio de Transportes y Comunicaciones (MTC, 2022), existen más de 80,000 unidades de carga habilitadas para el transporte terrestre de mercancías en el Perú, de las cuales una proporción significativa opera sin herramientas digitales de gestión.
    *   **Compradores mayoristas y empresas distribuidoras:** Intermediarios que adquieren la producción agrícola para su distribución en mercados de abastos, supermercados y cadenas de restaurantes. La incertidumbre sobre los tiempos de llegada les impide planificar adecuadamente sus operaciones.
    *   **Gestores logísticos y coordinadores de flota:** Responsables de la coordinación de múltiples unidades de transporte que carecen de herramientas unificadas para el monitoreo simultáneo de operaciones.

*   **What (¿Cuál es el problema?)**
    El problema central es la **ausencia de visibilidad en tiempo casi real** sobre el estado y la ubicación de las unidades de transporte de alimentos durante su recorrido. Esta opacidad informacional genera:
    *   Incapacidad de anticipar retrasos o incidencias en ruta.
    *   Dificultad para coordinar la recepción del producto en destino.
    *   Pérdida de control sobre las condiciones del transporte, lo que puede derivar en deterioro de la carga.
    *   Incapacidad de generar registros históricos confiables sobre las operaciones, impidiendo la mejora continua del proceso logístico.

*   **Where (¿Dónde ocurre el problema?)**
    El problema ocurre en las rutas de transporte terrestre de alcance nacional, con especial incidencia en los corredores viales que conectan las principales regiones productoras de alimentos con los centros de distribución y consumo. Los corredores más críticos incluyen:
    *   Ayacucho → Lima (papa, quinua, maíz)
    *   Junín → Lima (café, cítricos, papa)
    *   La Libertad → Lima (espárragos, palta, arándanos)
    *   Puno → Arequipa y Lima (quinua, cañihua, papa nativa)
    *   Cusco → Lima y Arequipa (maíz, papa, kiwicha)
    
    Estas rutas concentran un alto volumen de carga agrícola y presentan tramos de difícil acceso geográfico que incrementan el riesgo de incidencias durante el trayecto (MTC, 2022).

*   **When (¿Cuándo ocurre el problema?)**
    El problema es **continuo y estructural**, presente durante las 24 horas del día y los 7 días de la semana en cada operación de transporte. Se agudiza en periodos de alta demanda logística, como las campañas agrícolas de cosecha (enero-marzo y julio-septiembre), en los que el volumen de transporte se incrementa significativamente y la coordinación se vuelve más crítica (MIDAGRI, 2022).

*   **Why (¿Por qué ocurre el problema?)**
    Las causas raíz del problema pueden clasificarse en tres niveles:
    1.  **Causas tecnológicas:** La mayoría de los operadores de transporte agrícola no cuenta con sistemas de rastreo GPS integrados ni con plataformas digitales de gestión de flotas. La penetración de soluciones *fleet management* en el sector es inferior al 15 % (MTC, 2022).
    2.  **Causas organizacionales:** La alta informalidad del sector (se estima que más del 40 % de los transportistas de carga agrícola opera sin habilitación formal vigente) dificulta la adopción de estándares tecnológicos (Ministerio de Trabajo y Promoción del Empleo [MTPE], 2023).
    3.  **Causas económicas:** El costo percibido de las soluciones tecnológicas existentes es elevado para el perfil de pequeño y mediano transportista, que opera con márgenes ajustados. Las soluciones disponibles en el mercado (como los sistemas ERP logísticos de gran escala) no están diseñadas para este segmento.

*   **How (¿Cómo ocurre el problema?)**
    En la práctica, el proceso logístico de transporte de alimentos funciona de la siguiente manera: el productor o acopiador contrata verbalmente a un transportista, acuerdan el precio del flete y la fecha de salida, y el seguimiento del envío se realiza exclusivamente mediante llamadas telefónicas al conductor. Si ocurre una incidencia —avería mecánica, bloqueo de vía, accidente— la comunicación depende de que el conductor tenga señal telefónica y decida informar a la contraparte. No existe registro formal de la operación, ni trazabilidad del recorrido, ni mecanismo de alerta temprana. El comprador en destino tampoco tiene visibilidad sobre el estado del envío y solo puede estimar tiempos de llegada con base en experiencias previas o comunicaciones informales.

*   **How Much (¿Cuánto impacta el problema?)**
    El impacto económico de la problemática es considerable:
    *   Las pérdidas postcosecha asociadas a deficiencias logísticas en el Perú ascienden a más de S/ 2,000 millones anuales (CEPLAN, 2023).
    *   El tiempo promedio de retraso no gestionado en rutas de sierra-costa es de entre 4 y 8 horas por viaje, lo que equivale a una pérdida de frescura y calidad del producto (MIDAGRI, 2022).
    *   La incertidumbre en los tiempos de entrega obliga a los compradores a mantener inventarios de seguridad más elevados, incrementando sus costos operativos (Banco Mundial, 2021).
    *   Las empresas transportistas que no cuentan con registros de sus operaciones pierden oportunidades de negocio con clientes que exigen trazabilidad como condición de contratación (FAO, 2022).
Para delimitar con precisión el alcance y el impacto del desarrollo del producto de software, el equipo ha establecido los siguientes objetivos orientados al negocio, al proceso de ingeniería y a la experiencia del usuario:

#### 1.2.1.1. Objetivos del Proyecto
Para delimitar con precisión el alcance y el impacto del desarrollo del producto de software, el equipo ha establecido los siguientes objetivos orientados al negocio, al proceso de ingeniería y a la experiencia del usuario:

*   **Objetivo General:**
    *   Diseñar, desarrollar e implementar un sistema web distribuido (compuesto por una aplicación de interfaz cliente responsive y un RESTful API de desarrollo interno) para la startup AgroFlet, que permita centralizar, monitorear y gestionar de forma transparente el transporte terrestre de alimentos en el Perú, contribuyendo de manera directa a la reducción de mermas postcosecha y a la eficiencia logística.
*   **Objetivos Específicos:**
    *   Desarrollar una aplicación frontend responsive que proporcione una experiencia de usuario altamente intuitiva e inclusiva, optimizada para los segmentos de medianos productores/acopiadores y compradores mayoristas.
    *   Construir un RESTful API del lado del servidor robusto y de alto rendimiento que garantice la persistencia segura, la lógica de negocio y la consistencia en el procesamiento de operaciones y alertas logísticas.
    *   Garantizar la cobertura del diseño inclusivo implementando atributos de accesibilidad ARIA e internacionalización (i18n) para soportar fluidamente los idiomas inglés y español latinoamericano.
    *   Integrar de manera fluida un servicio geográfico de terceros que brinde soporte visual e interactivo al trayecto físico de las unidades de transporte sobre mapas digitales.
    *   Alcanzar los criterios de éxito planteados en la visión de negocio: registrar al menos 200 usuarios activos en la plataforma en los primeros 8 meses, reducir en un 20 % los tiempos de gestión de incidencias en ruta, asegurar una tasa de retención superior al 70 % a partir del tercer mes de operación, y registrar un nivel de satisfacción (NPS) superior a los 40 puntos a los 3 meses de uso de la aplicación.

#### 1.2.1.2. Restricciones del Proyecto
El ciclo de vida de desarrollo de AgroFlet está sujeto a un conjunto de limitaciones tecnológicas, metodológicas y operativas impuestas para asegurar la calidad y los estándares de la ingeniería de software:

*   **Restricciones Tecnológicas del Servidor:** El RESTful API del lado del servidor debe ser construido estrictamente con tecnologías open-source basadas en el lenguaje de programación C#, utilizando el framework ASP.NET Core y Entity Framework Core como mapeador objeto-relacional (ORM), persistiendo los datos obligatoriamente en un sistema de gestión de bases de datos relacionales (RDBMS) MySQL Server o PostgreSQL.
*   **Restricciones Tecnológicas del Cliente:** La aplicación web frontend debe implementarse con el framework progresivo Vue, empleando JavaScript como lenguaje de programación. El diseño visual debe ceñirse al lenguaje de diseño Material Design utilizando PrimeVue como biblioteca de componentes de interfaz de usuario.
*   **Restricciones de Integración y Documentación:** El sistema web distribuido debe consumir de manera obligatoria un servicio externo de mapas e integrarse mediante llamadas API RESTful documentadas técnicamente con OpenAPI Specification a través de Swagger.
*   **Restricciones de Proceso y Calidad de Código:** El proyecto debe ser gestionado bajo el marco de trabajo ágil Scrum. El código fuente debe ser almacenado y administrado en repositorios dentro de una organización pública en GitHub, aplicando estrictamente el flujo de ramas GitFlow, la nomenclatura estandarizada en inglés para el código, mensajes de commit bajo la convención de Conventional Commits, y el versionamiento formal bajo Semantic Versioning (SemVer 2.0.0).
*   **Restricciones de Idioma y Accesibilidad:** AgroFlet está diseñado y dirigido de manera prioritaria para el entorno agrícola y logístico peruano, por lo cual la plataforma se concibe de forma nativa en **español** para asegurar una usabilidad óptima y libre de fricciones para los agricultores y transportistas locales. No obstante, para alinearse con las directrices de ingeniería globales y cumplir estrictamente con los requisitos de acreditación ABET del curso, el sistema web distribuido se desarrollará utilizando un marco de **internacionalización (i18n)**. Esto permitirá que la interfaz de usuario, los mensajes del sistema y la documentación del API cuenten con soporte técnico en **inglés** y **español**, configurando el idioma de manera fluida según la preferencia del usuario. Asimismo, se implementarán **atributos ARIA** para asegurar la accesibilidad web (**a11y**).




### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements

El equipo aplicó la versión *Brand new initiative* del template de Lean UX Problem Statement:

**The current state of* agricultural food transportation logistics in Peru *has focused mainly on** informal operators who manage freight transport without digital tools, relying on verbal agreements, phone calls, and paper records, unable to provide real-time visibility on shipment location or status to producers, buyers, and logistics coordinators.

**What existing products/services fail to address is** an affordable, accessible, and sector-specific digital monitoring platform that consolidates fleet tracking, incident reporting, and shipment management in a single interface adapted to the operational reality of Peruvian agricultural transport actors.

**Our product/service will address this gap by** developing AgroFlet, a responsive web platform for near real-time monitoring and management of agricultural food transport operations, enabling users to track shipment location, consult delivery estimates, register and visualize route incidents, and access historical operation data — all from a single, intuitive dashboard.

**Our initial focus will be** logistics coordinators and fleet managers of medium-sized agricultural transport companies operating on high-volume routes between Peru's producing regions and Lima Metropolitana, as well as wholesale buyers seeking visibility over incoming shipments.

**We’ll know we are successful when we see** at least 200 active users within the first 8 months, a monthly user retention rate above 70% starting from month 3, a 20% reduction in incident management times, and a Net Promoter Score (NPS) exceeding 40 points after 3 months of platform usage.

#### 1.2.2.2. Lean UX Assumptions

En concordancia con el proceso Lean UX, el equipo identificó los siguientes supuestos (*assumptions*) agrupados por tipo:

**Business Assumptions**
1. Creemos que existe un mercado suficientemente grande de empresas de transporte agrícola y compradores mayoristas en el Perú que están dispuestos a adoptar una plataforma digital de monitoreo logístico, dado el impacto económico de la falta de visibilidad en sus operaciones.
2. Creemos que un modelo de negocio basado en suscripción mensual por rango de flota (número de unidades registradas) es viable y aceptable para el segmento de medianas empresas de transporte agrícola en el Perú.
3. Creemos que AgroFlet puede diferenciarse de las soluciones ERP logísticas existentes por su enfoque sectorial, su accesibilidad de precio y su diseño orientado a usuarios con distintos niveles de alfabetización digital.
4. Creemos que la integración con un servicio externo de geolocalización (como Google Maps Platform o HERE Maps) es técnicamente factible dentro del alcance del proyecto y agrega valor significativo a la experiencia del usuario.
5. Creemos que el equipo de desarrollo cuenta con las competencias técnicas para desarrollar, desplegar y mantener la plataforma utilizando Vue.js (frontend), ASP.NET Core (backend) y MySQL (base de datos relacional) dentro del ciclo académico.

**Business Outcome Assumptions**
1. Creemos que, al cabo de 8 meses desde el lanzamiento, AgroFlet habrá registrado al menos 200 empresas o usuarios activos en la plataforma.
2. Creemos que la tasa de retención mensual de usuarios activos superará el 70 % a partir del tercer mes de operación, como indicador de la generación de valor percibido.
3. Creemos que la plataforma contribuirá a reducir el tiempo promedio de respuesta ante incidencias en ruta en al menos un 20 % para los usuarios que la adopten.
4. Creemos que la generación de historial de operaciones dentro de la plataforma se convertirá en un activo de valor para los usuarios, incentivando la renovación de la suscripción.
5. Creemos que la publicación de reseñas y recomendaciones de usuarios tempranos (*early adopters*) contribuirá a un crecimiento orgánico de la base de usuarios a través de referencias en el sector.

**User Assumptions**
1. Creemos que nuestros usuarios principales son coordinadores logísticos y gestores de flota de empresas de transporte agrícola de mediano tamaño (entre 5 y 50 unidades de transporte), con edades entre 28 y 55 años, que operan desde oficinas en Lima o en capitales de región.
2. Creemos que un segundo segmento relevante son los compradores mayoristas (jefes de compras o encargados de abastecimiento) de empresas distribuidoras, mercados de abastos o cadenas de supermercados, que reciben envíos agrícolas de forma regular.
3. Creemos que ambos segmentos utilizan principalmente smartphones Android de gama media y computadoras de escritorio con Windows para sus actividades laborales diarias.
4. Creemos que los usuarios del segmento transportista tienen experiencia básica con aplicaciones de mensajería (WhatsApp) y navegación web, pero no con plataformas de gestión empresarial (ERP o CRM).
5. Creemos que los usuarios del segmento comprador tienen mayor familiaridad con herramientas digitales de oficina (hojas de cálculo, correo electrónico) y están acostumbrados a la consulta de información en dashboards.

**User Outcome and Benefit Assumptions**
1. Creemos que los coordinadores logísticos quieren reducir el tiempo que dedican a gestionar incidencias por teléfono y obtener visibilidad centralizada sobre el estado de sus flotas sin depender de llamadas frecuentes a los conductores.
2. Creemos que los gestores de flota quieren poder asignar y monitorear viajes de forma más ordenada, con un historial que les permita evaluar el desempeño de sus unidades y conductores.
3. Creemos que los compradores mayoristas quieren conocer con anticipación la hora estimada de llegada de sus envíos para coordinar la recepción del producto, optimizar el uso de sus espacios de almacenamiento y reducir el tiempo de espera de su personal.
4. Creemos que ambos segmentos valoran la posibilidad de registrar y consultar incidencias de ruta (bloqueos, averías, retrasos) como un mecanismo de *accountability* que les permite justificar retrasos ante sus clientes o proveedores.
5. Creemos que los usuarios del segmento transportista considerarán que la plataforma agrega valor diferencial si les permite demostrar a sus clientes un nivel de servicio más profesional y transparente, incrementando así su competitividad en el mercado.

**Feature Assumptions**
1. Creemos que un dashboard de monitoreo en tiempo casi real que muestre la ubicación actual, el estado y los datos principales de cada operación de transporte activa es la funcionalidad de mayor valor percibido para ambos segmentos.
2. Creemos que el registro y visualización de incidencias en ruta (tipo, descripción, impacto estimado en el tiempo de entrega) es una funcionalidad crítica que diferencia a AgroFlet de soluciones genéricas de rastreo GPS.
3. Creemos que la gestión del historial de operaciones (filtrado por fecha, ruta, tipo de alimento, unidad de transporte y estado) es una funcionalidad de alto valor para los usuarios con necesidad de *reporting* y planificación.
4. Creemos que la visualización geográfica de rutas activas sobre un mapa interactivo, integrado con un servicio externo de mapas, incrementará significativamente la usabilidad y adopción de la plataforma.
5. Creemos que la gestión de flotas y conductores (registro de unidades, asignación de conductores, consulta de disponibilidad) es una funcionalidad necesaria para el segmento de coordinadores logísticos de empresas de transporte.
6. Creemos que el envío de alertas y notificaciones ante incidencias registradas o retrasos detectados incrementará el valor percibido de la plataforma y la frecuencia de uso diario.
7. Creemos que un sistema de filtros y búsqueda avanzada sobre el listado de operaciones facilita la consulta de información por parte de usuarios con alto volumen de operaciones registradas.

#### 1.2.2.3. Lean UX Hypothesis Statements

En concordancia con el proceso Lean UX, el equipo formuló los siguientes hypothesis statements, uno por cada feature assumption identificada:

**Hypothesis Statement 1:**
*We believe we will achieve* **an active adoption of at least 200 users within the first 8 months** 
*If* **logistics coordinators and fleet managers** 
*Attain* **centralized, near real-time visibility over active fleet locations and shipment status without depending on constant phone calls** 
*With* **a near real-time monitoring dashboard displaying live location, status, and shipment details of active transport operations.**

**Hypothesis Statement 2:**
*We believe we will achieve* **a 20% reduction in incident management times** 
*If* **logistics coordinators and wholesale buyers** 
*Attain* **the ability to immediately report and visualize road incidents (such as delays, breakdowns, or roadblocks) and estimate delivery impact** 
*With* **an incident reporting and visual tracking system directly integrated on the route details page.**

**Hypothesis Statement 3:**
*We believe we will achieve* **a monthly user retention rate above 70% starting from month 3** 
*If* **fleet managers** 
*Attain* **a reliable historical record of past shipments to audit performance, analyze recurring routes, and optimize logistics planning** 
*With* **an operation history management module with advanced search, filtering, and exportable logs.**

**Hypothesis Statement 4:**
*We believe we will achieve* **a Net Promoter Score (NPS) exceeding 40 points after 3 months of platform usage** 
*If* **logistics coordinators and wholesale buyers** 
*Attain* **an intuitive and highly visual way to track shipment progress along national highway corridors** 
*With* **an interactive map interface integrated with an external geolocation service.**

**Hypothesis Statement 5:**
*We believe we will achieve* **a monthly user retention rate above 70% starting from month 3** 
*If* **logistics coordinators** 
*Attain* **an orderly mechanism to register trucks, assign available drivers, and organize dispatch workflows** 
*With* **a fleet and driver management module with status indicators and simplified registry forms.**

**Hypothesis Statement 6:**
*We believe we will achieve* **a 20% reduction in incident management times** 
*If* **logistics coordinators and wholesale buyers** 
*Attain* **instant awareness of critical delays, breakdowns, or road blockages to execute contingency plans immediately** 
*With* **an automated system of push alerts and in-app notifications triggered upon incident registration.**

**Hypothesis Statement 7:**
*We believe we will achieve* **a Net Promoter Score (NPS) exceeding 40 points after 3 months of platform usage** 
*If* **logistics coordinators with high daily operational volumes** 
*Attain* **the ability to find specific shipments, drivers, or routes within seconds, minimizing search fatigue** 
*With* **an advanced search bar and multi-criteria filters on the active shipments dashboard.**


#### 1.2.2.4. Lean UX Canvas

El Lean UX Canvas es una herramienta ágil que sintetiza los elementos clave del proceso Lean UX en un único artefacto visual colaborativo. A continuación, se presenta el canvas desarrollado por el equipo para el diseño y concepción de AgroFlet:

| **1. Business Problem** | **2. Business Outcomes** | **3. Users & Customers** |
| ------ | ------ | ------ |
| Los actores de la cadena de transporte de alimentos en el Perú —productores, transportistas y compradores— operan sin visibilidad digital sobre el estado y la ubicación de los envíos agrícolas durante el trayecto, lo que genera retrasos no gestionados, pérdidas económicas significativas y baja capacidad de respuesta ante incidencias en ruta. | • Registrar al menos  **200 usuarios activos**  en la plataforma en los primeros 8 meses.<br><br>• Lograr una  **reducción del 20 %**  en los tiempos de gestión de incidencias en ruta.<br><br>• Mantener una  **tasa de retención mensual superior al 70 %**  a partir del tercer mes de operación.<br><br>• Alcanzar una satisfacción del usuario ( **NPS) superior a los 40 puntos**  tras 3 meses de uso de la plataforma. | **Segmento 1: Medianos Productores Agrícolas y Acopiadores (Despachadores)** <br>• Agricultores medianos independientes, cooperativas agrícolas y acopiadores locales que consolidan la carga agrícola y contratan servicios de flete terrestre.<br><br> **Segmento 2: Compradores Mayoristas y Encargados de Abastecimiento** <br>• Jefes de compras, encargados de abastecimiento, gerentes de logística o dueños de puestos en mercados de abastos, supermercados y distribuidoras. |
| **4. User Benefits** | **5. Solutions (Features)** | **6. Hypotheses** |
| •  **Visibilidad centralizada**  y en tiempo casi real del estado y la ubicación de los fletes agrícolas.<br><br>• Capacidad de  **anticiparse a retrasos**  y gestionar incidencias viales de forma proactiva.<br><br>• Acceso a un  **historial de operaciones**  formalizado para auditoría de fletes y planificación comercial.<br><br>• Incremento del profesionalismo, la transparencia y la competitividad en el mercado de fletes terrestres. | • Dashboard de monitoreo logístico en tiempo casi real.<br><br>• Módulo de registro y visualización de incidencias en ruta.<br><br>• Gestión de historial de operaciones con exportación de reportes.<br><br>• Visualización geográfica de viajes activos sobre mapa interactivo.<br><br>• Gestión interna de flotas, unidades y conductores asignados.<br><br>• Sistema automatizado de alertas y notificaciones push en ruta.<br><br>• Barra de búsqueda avanzada y multi-filtros de operaciones. | *Debido a la extensión de los enunciados, las declaraciones detalladas de hipótesis del negocio se encuentran mapeadas y numeradas secuencialmente en la sección previa:* <br><br> **Ver Sección 1.2.2.3. Lean UX Hypothesis Statements** |
| **7. What's the most important thing we need to learn first?** | **8. What's the least amount of work we need to do to learn the next most important thing?** |  |
| Validar si los **medianos productores agrícolas/acopiadores (despachadores)** y los **compradores mayoristas** están dispuestos a adoptar y pagar por una plataforma digital de monitoreo logístico, y cuáles son las funcionalidades que consideran críticas dentro de su flujo diario de trabajo. | Construir un  **prototipo interactivo de alta fidelidad**  en Figma que simule el flujo de visualización del dashboard de monitoreo y el registro de incidencias en ruta. Con este artefacto, realizar entre  **6 y 10 entrevistas de validación**  con representantes reales de ambos segmentos para evaluar la propuesta de valor, la usabilidad percibida y la disposición de pago bajo un modelo de suscripción. |  |


## 1.3. Segmentos objetivo

La identificación de los segmentos objetivo de AgroFlet parte del análisis de la problemática de la cadena logística terrestre, la viabilidad de validación con actores reales y la revisión de fuentes estadísticas oficiales del sector [7]. Se han definido dos segmentos clave que interactúan directamente en la cadena de suministro agroalimentaria [7]:

---

### Segmento 1: Medianos Productores Agrícolas y Acopiadores (Despachadores)

**Descripción general:**  
Este segmento está constituido por agricultores medianos independientes, representantes de cooperativas agrícolas y acopiadores locales que se encargan de consolidar la carga agrícola en las zonas de producción para despacharla hacia los principales mercados de consumo. Son los cargadores (*shippers*) de la cadena logística, responsables de contratar los servicios de flete terrestre. Su principal dolor es la pérdida de visibilidad y el riesgo de deterioro de los alimentos perecibles una vez que la unidad de transporte sale del centro de acopio con rumbo a su destino nacional.

**Características demográficas y estadísticas integradas:**  
*   **Edad:** Entre 25 y 60 años.
*   **Género:** Mixto, con una participación destacada de liderazgo femenino del **30 % en las juntas de cooperativas agrarias**.
*   **Ubicación geográfica:** Ubicados en zonas de producción agrícola con alta conectividad comercial hacia Lima Metropolitana, tales como Junín, Huánuco, Ica, La Libertad, Cañete y Huaral. Estas regiones forman parte de la base productiva del país, donde la actividad agropecuaria representa aproximadamente el **6 % del Producto Bruto Interno (PBI) nacional** y ocupa a más del **28 % de la Población Económicamente Activa (PEA) rural**.
*   **Nivel educativo y perfil organizacional:** Educación secundaria completa, técnica o superior universitaria en Agronomía, Administración de Negocios o carreras afines. Se organizan habitualmente bajo esquemas de cooperativas de acopio para mejorar su poder de negociación frente a intermediarios, representando un sector clave en el Perú donde el **78 % de las unidades agropecuarias poseen menos de 5 hectáreas**.
*   **Experiencia laboral y volumen de mermas asociadas:** Más de 5 años en la gestión de cultivos, acopio y comercialización agrícola. Operan en un entorno altamente crítico donde aproximadamente el **35 % de la producción agrícola peruana se pierde** entre la cosecha y el punto de venta debido a ineficiencias de transporte [3], lo que genera un impacto económico directo acumulado para los productores que supera los **S/ 2,000 millones anuales**.

**Características psicográficas y conductuales:**  
*   **Presión por mermas:** Experimentan un alto nivel de estrés debido a la volatilidad de los precios en el mercado mayorista y el riesgo latente de que la carga sufra retrasos prolongados en carretera.
*   **Coordinación informal:** Dependen casi exclusivamente de llamadas de voz y mensajes de WhatsApp con transportistas independientes para conocer el estado de sus despachos, enfrentándose a que más del **70 % del transporte de carga agrícola opere sin trazabilidad digital**.
*   **Tecnología:** Utilizan smartphones Android de gama media con acceso a planes de datos móviles y aplicaciones de mensajería, además de computadoras portátiles para coordinar la facturación y guías de remisión.
*   **Disposición tecnológica:** Alta receptividad a adoptar herramientas de bajo costo que demuestren reducir las pérdidas de alimentos y mejoren la transparencia con sus clientes.

**Puntos de dolor (Pain Points):**  
*   Incertidumbre absoluta sobre la ubicación física del camión que traslada sus productos agrícolas perecibles.
*   Falta de mecanismos de alerta temprana para enterarse de incidencias viales (bloqueos, accidentes o fallas mecánicas) y poder desviar la carga o negociar prórrogas.
*   Dificultad para demostrar ante el comprador final que un retraso o merma en el producto fue responsabilidad de incidencias viales en carretera y no de un mal manejo en origen.
*   Pérdida de tiempo operativo llamando repetidamente a conductores que muchas veces no contestan el teléfono o transitan por zonas con cobertura intermitente.

---

### Segmento 2: Compradores Mayoristas y Encargados de Abastecimiento

**Descripción general:**  
Este segmento agrupa a los actores que reciben los envíos de alimentos agrícolas en los centros de distribución, mercados de abastos o plataformas de supermercados. Pueden ser jefes de compras, encargados de abastecimiento, gerentes de logística de entrada o propietarios de puestos en mercados mayoristas. Su principal necesidad es contar con información anticipada y de confianza sobre la hora de llegada de los envíos para coordinar la recepción del producto, optimizar el uso de su personal y sus espacios de almacenamiento, y garantizar la continuidad de su cadena de suministro.

**Características demográficas y estadísticas integradas:**  
*   **Edad:** Entre 30 y 60 años.
*   **Género:** Mixto, con representación equitativa según el contexto (mercados de abastos con predominio masculino; cadenas de supermercados con mayor participación femenina en roles de compras).
*   **Ubicación geográfica y alcance de mercado:** Principalmente Lima Metropolitana (que concentra la mayor distribución del país) y capitales de región con mercados de abastos de alta actividad. En Lima Metropolitana, operan en un entorno que alberga más de **1,200 mercados de abastos**, donde los 4 mercados mayoristas principales manejan un volumen diario masivo de más de **8,000 toneladas de alimentos**.
*   **Nivel educativo y tipología de negocio:** Variable, abarcando desde educación secundaria completa (comerciantes independientes de mercados de abastos) hasta educación superior universitaria o de posgrado (gerentes de compras de cadenas formales de supermercados).
*   **Volumen de operaciones y participación comercial:** Entre **2 y 30 envíos recibidos por semana**, dependiendo del tamaño del negocio [13]. En el canal moderno, las cadenas de supermercados (Wong, Plaza Vea, Tottus, Metro) representan una participación del **35 % del gasto en alimentos** de los hogares limeños de nivel socioeconómico medio y alto [4], lo que exige un estándar logístico de alta trazabilidad y confiabilidad.

**Características psicográficas y conductuales:**  
*   **Sensibilidad al tiempo:** Alta sensibilidad a la puntualidad de las entregas, ya que el retraso en productos perecibles impacta de manera directa en la frescura y calidad final del producto recibido.
*   **Frustración operativa:** Frustración frecuente ante la falta de información proactiva de los transportistas sobre retrasos o incidencias en carretera.
*   **Tecnología:** Mayor familiaridad con herramientas digitales de oficina (hojas de cálculo, correo electrónico) que el promedio del segmento transportista.
*   **Disposición tecnológica:** Receptividad a adoptar herramientas que reduzcan la incertidumbre en su cadena de abastecimiento. En el caso de compradores formales (supermercados y distribuidoras), existe una exigencia creciente de trazabilidad como requisito contractual obligatorio para sus proveedores logísticos.

**Puntos de dolor (Pain Points):**  
*   Incertidumbre sobre la hora de llegada de los envíos, lo que obliga a mantener personal de recepción en espera durante periodos prolongados.
*   Imposibilidad de anticipar retrasos que puedan generar desabastecimiento o pérdida de frescura del producto.
*   Falta de un canal formal para recibir información sobre incidencias en ruta de parte del transportista.
*   Dificultad para evaluar el desempeño de sus proveedores de transporte al carecer de registros históricos de cumplimiento.
*   En el caso de compradores formales, presión creciente de sus propias cadenas de auditoría interna para documentar la trazabilidad de su cadena de suministro.
