# Capítulo 5: Product Implementation, Validation & Deployment

## 5.1 Software Configuration Management.

Para administrar la configuración de software de nuestra app, nos centraremos en tres aspectos principales: el control del código fuente, que implica gestionar las versiones y establecer una estructura organizada para el código; la configuración del entorno de desarrollo, donde nos aseguramos de que todos los miembros del equipo cuenten con herramientas consistentes; y la configuración de implementación, que se ocupa del despliegue en entornos de producción. Estas decisiones garantizan la coherencia y eficacia a lo largo de todo el ciclo de vida de la aplicación.

### 5.1.1 Software Development Environment Configuration

En esta sección, detallaremos y explicaremos los productos utilizados en el proyecto digital, así como su propósito y cómo se accede a cada uno de ellos y siguiendo las restricciones establecidas.

1. Project Management:
Para gestionar el proyecto, se utilizaron herramientas de comunicación y control de versiones. Se estableció una organización en GitHub para gestionar el código y las versiones del proyecto. Además, para las reuniones de equipo y la comunicación interna, se utilizaron plataformas como Google Meet y Discord.
- Github: https://github.com/
- Google Meet: https://meet.google.com/
- Discord: https://discord.com/download

2. Requirements Management:
Para la gestión de requisitos se llevó a cabo mediante el uso de herramientas personalizadas que permitieron recopilar, organizar y priorizar los requisitos del proyecto de manera eficiente. Se utilizó Trello, una herramienta visual para la gestión de requisitos, permitiendo la creación tableros personalizados para organizar y priorizar las tareas del proyecto que permitió realizar los Task board y Pivotal Tracker, utilizado para gestionar y realizar un seguimiento del Product Backlog del proyecto.
- Trello: https://trello.com/es
- Pivotal Tracker: https://www.pivotaltracker.com/

3. Product UX/UI Design:
Para el diseño de la experiencia de usuario (UX) y diseño de interfaz de usuario (UI) del producto se utilizo la herramienta Figma, esta herrmienta permitio al equipo crear wireframes, mockups y prototipos interactivos para visualizar y validad el diseño del producto antes de la implementación.
Por otro lado, para la creación de User Personas, Empathy Maps, Journey Maps e Impact Maps se utilizó UXPressia y para la creación de As-Is y To-Be Scenario Maps se utilizó Miro.
- Figma: https://www.figma.com/downloads/
- UXPressia: https://uxpressia.com/
- Miro: https://miro.com/es/

4. Software Development:
Para el desarrollo de software se utilizó HTML5, CSS3 y JavaScript para el desarrollo de la Landing Page de la startup, por otro lado, para la creación del Web Application de la startup se utilizarán el framework de Vue por el lado del Frontend y en el Backend se utilizará ASP.NET Core Framework y C#.
Para trabajar con estas tecnologías, se emplearon los siguientes IDEs:
Visual Studio Code: Herramienta principal para el desarrollo Frontend y Backend, que ofrece una amplia gama de extensiones para mejorar la productividad del equipo. (En nuestro caso solo fue utilizado para la Landing Page).
JetBrains Toolbox: Proporciona un entorno integrado para el desarrollo web, con características avanzadas de edición y depuración que faciitan la creación de aplicaciones web robustas.
- Visual Studio Code: https://code.visualstudio.com/
- JetBrains Toolbox: https://www.jetbrains.com/toolbox-app/

5. Software Documentation:
La documentación del software se realizó utilizando GitHub, además de ser utilizado como plataforma de control de versiones, GitHub también se empleó para alojar la documentación técnica del proyecto. Se crearon repositorios específicos para almacenar toda la información. La documentación se gestionó mediante archivos Markdown para facilitar la creación y edición colaborativa.
- GitHub: https://github.com/

### 5.1.2 Source Code Management.

En este proyecto, utilizaremos GitHub como plataforma y sistema de control de versiones para gestionar el código fuente de nuestras diferentes partes del proyecto dentro de una organización.

**Repositorios en GitHub**
- Organización: https://github.com/upc-AppWeb-BicasTeam
- Landing Page: https://github.com/upc-AppWeb-BicasTeam/upc-AppWeb-BicasTeam-LandingPage
- Report : https://github.com/upc-AppWeb-BicasTeam/upc-AppWeb-BicasTeam-Report

**GitFlow Workflow**
Implementaremos el modelo GitFlow como Workflow de control de versiones, siguiendo las convenciones y prácticas establecidas para una gestión eficiente del desarrollo de software.
1. **Branches Principales:
- `main`: Rama principal del repositorio, contiene el código estable y liberado.
- `develop`: Rama de desarrollo deonde se integran las nuevas características y mejoras.

2. Branches de Funcionalidades (Feature Branches):
- Para cada nueva funcionalidad, se creará una rama de funcionalidad con el prefijo `feature/`, seguido del nombre descriptivo de la función o característica. En nuestro caso, creamos 5 branches de características correspondientes a los 5 capítulos de nuestro informe, donde se realizan los commits respectivos antes de fusionarlos con la rama develop cuando estén listos.

3. Branches de Lanzamiento (Release Branches) y Branches de Corrección (Hotfix Branches):
En nuestro caso, no hicimos uso de estas branches ya que no lo vimos necesario al ser solo documentacion del reporte.

**Versionado Semántico**
Seguimos la especificación Semantic Versioning 2.0.0 para nombrar nuestras versiones, siguiendo el formato: `MAJOR.MINOR.PATCH`.

**Conventional Commits**
Aplicamos el estándar de Conventional Commits para los mensajes de commit, siguiendo un formato estructurado que describe claramente los cambios realizados. Esto nos ayudó a automatizar la generación de notas de versión y facilitar la comprensión del historial de cambos del proyecto.

Con estas prácticas y convenciones adaptadas a una organización en GitHub, buscamos mantener un flujo de desarrollo ordenado, colaborativo y bien documentado.

### 5.1.3 Source Code Style Guide & Conventions.

En esta sección, se establece las convenciones y prácticas que seguiremos para nombrar elementos y programar en los lenguajes utilizados en la solución, que incluyen HTML, CSS, JavaScript, Vue.js, C#, y Gherkin para los archivos `.feature`. Todas las convenciones seguirán la nomenclatura en inglés y adoptarán convenciones estándares de codificación.

1. **HTML y CSS**:
- Basado en las recomendaciones de W3C y otras fuentes de la comunidad, se establecerán convenciones para el nombramiento de elemntos hTML y estilo de la codificación CSS.
- Se seguirán las convenciones recomendadas por Google para HTML y CSS, que incluyen el uso de identaciones de 2 espacios, el uso de comillas dobles para atributos y el uso de comentarios descriptivos.
- Se utilizará la metodologìa BEM para organizar las clases CSS en bloques, elementos y modificadores, lo que facilitará la modularidad y la reutilización del código. 
- Se debe utilizar los elementos HTML de manera semántica para una correcta descripción del contenido del sitio web, incluyendo el uso adecuado de etiquetas.
- Para el desarrollo con Vue.js, se adoptarán las convenciones recomendadas por la comunidad de Vue, que incluyen el uso de PascalCase para los nombres y componentes y el uso de camelCase para las propiedades y métodos de los componentes.

2. **JavaScript**:
- Se tomarán en cuenta las directrices proporcionadas por MDN para la escritura de JavaScript, que incluyen el uso de nombres descriptivos para variables y funciones en camelCase, el uso de declaración de variavles con `let` o `const` en lugar de `var`, y el uso de punto y coma al final de cada declaración.
- Se seguirán las convenciones de codificación recomendadas por Google para JavaScript, que incluyen el uso de comillas simples para literales de cadena, el uso de comentarios descriptivos y el uso de funciones de flecha para expresiones de función.

3. **Vue.js**:
- Se adoptarán las convenciones de codificación recomendadas por la comunidad de aplicaciones Vue.js, que incluyen el uso de directivas v-bind y v-on abreviadas, el uso de ciclo de vida y la organización de componentes en carpetas y subcarpetas según su función.

4. **C# (ASP.NET Core)**:
- Se seguirán las convenciones de codificación establecidas por Microsoft para el lenguaje C#, que incluyen el uso de PascalCase para nombres de clases y métodos, el uso de camelCase para nombres de variables locales y parámetros, y el uso de comentarios XML para documentar el código.
- Para el desarrollo en ASP.NET Core, se adoptarán las directrices proporcionadas por Microsoft en sus guías de codificación, que incluyen el uso de inyección de dependencias, la separación clara entre capas de la aplicación y el uso de modelos de vista para la comunicación entre el controlador y la vista.

5. **Gherkin**:
- Se aplicarán las convenciones recomendadas para escribir especificaciones legibles en Gherkin, que incluyen el uso de palabras clave como Given, When y Then para describir el comportamiento del sistema, el uso de un lenguaje sencillo y claro, y la organización de los escenarios en contextos, acciones y resultados.
- Se seguirán las mejores prácticas recomendadas por Cucumber para escribir escenarios de prueba en Gherkin, que incluyen la reutilización de pasos de prueba, la modularización de escenarios y la escritura de pruebas autoexplicativas.

Además de estas referencias, se promoverá el uso de buenas prácticas y metodologías estándar en el desarrollo de software, como la modularidad, la reutilización de código, la legibilidad del código, la optimización del rendimiento y la seguridad. 
Con estas guías de estilo y convenciones de codificación, buscamos asegurar la coherencia, la calidad y la mantenibilidad del código a lo largo de todo el proyecto.

### 5.1.4 Software Deployment Configuration.

En esta sección, describiremos la configuración necesaria para desplegar satisfactoriamente cada uno de los productos digitales de nuestra solución, incluyendo Landing Page, los Web Services y las Frontend Web Applications.

**Pasos para el despliegue**
1. Landing Page:
- Clonar o descargar el repositorio desde GitHub.
- Configurar el servidore web para alojar la Landing Page.
- Copiar los archivos HTMLS, CSS y JavaScript en el directorio correspondiente del servidor.
- Configurar cualquier dependencia adicional, como bibliotecas de JavaScript o imágenes.
- Verificar quue la Landing Page se cargue correctamente en el navegador.

2. Web Services (API):
- Preparar el código fuente del servicio web, asegurando que esté correctamente estructurado y documentado.
- Configurar un entorno de desarrolo o pruebas para realizar pruebas exhaustivas del servicio antes del desplieguee.
- Desplegar el código en un servidor adecuado para el entorno de producción.
- Configurar la seguridad y la autenticación según los requisitos del sistema.
- Documentar la API utilizando OpenAPI Specification para facilitar su integración y uso por parte de otros sistemas.

3. Frontend Web Applications:
- Clonar repositorio desde GitHub.
- Compilar y empaquetar las aplicaciones frontend. En nuestro caso, utilizamos el framework Vue.js, por lo que se debe ejecutar los comandos de construcción (`npm run build`) para generar los archivos estáticos.
- Una vez empaquetadas, las Frontend Web Applications se pueden servir utilizando un servidor de aplicaciones compatible con archivos estáticos, como Nginx o incluso GitHub Pages para proyectos estáticos más simples.
- Si es necesario, se deben configurar las rutas en el servidor de aplicaciones para que conincidan con las rutas esperadas por las aplicaciones frontend.

## 5.2 Landing Page, Services & Applications Implementation.

En esta sección, describiremos el proceso de implementación, pruebas, documentación y despliegue de la Landing Page, los Web Services y las Frontend Web Applications. Abordaremos cada componente de manera individual a lo largo de los diferentes sprints, comenzando en este Sprint 1 con la implementación específica de la Landing Page. Una vez establecido nuestro Product Backlog, cada sprint se dividirá en secciones internas para abordar cada aspecto de la implementación y la colaboración del equipo.

### 5.2.1 Sprint 1

En esta sección, documentaremos y explicaremos el progreso tanto en el desarrollo del producto como en la colaboración del equipo durante el Sprint 1. Seguimos un proceso definido que abarca desde la planificación hasta la revisión y documentación del trabajo realizado. A lo largo de las siguientes secciones, detallaremos cómo se llevó a cabo la planificación del sprint, qué tareas se incluyeron en el Sprint Backlog, las pruebas y evidencia de desarrollo para la revisión del sprint, así como la documentación de los servicios y las percepciones clave sobre la colaboración del equipo durante este periodo

### 5.2.1.1 Sprint Planning 1

En esta sección, se detallan los aspectos principales del Sprint Planning Meeting para el Sprint n. Este encuentro es crucial para establecer los objetivos del sprint, determinar las user stories que se abordarán y asignar tareas al equipo. A continuación, se presenta un resumen del Sprint Planning Meeting para este período.

| Sprint #                             | Sprint 1           |
|--------------------------------------|--------------------|
| Sprint Planning Background                                |
| Date                                 |  2024-03-23        |
| Time                                 |  01:30 PM          |
| Location                             |  Virtual (Discord) |
| Prepared By                          |  Piero Tarazona    |
| Attendees (to planning meeting)      |  Piero Tarazona, Mauricio Chacon, Elias, Moises Donayre, Miguel |
| Sprint 1 – 1 Review Summary          |  Durante el primer sprint, avanzamos significativamente en el desarrollo del producto y logramos una colaboración eficiente dentro del equipo. Alcanzamos hitos importantes y recopilamos retroalimentación valiosa que nos servirá como base para el próximo sprint.  |
| Sprint 1 – 1 Retrospective Summary   |  En la retrospectiva del primer sprint identificamos áreas para mejorar, como la comunicación y la estimación de tareas. Estamos comprometidos a implementar acciones correctivas y mejorar continuamente nuestro proceso de trabajo.  |
| Sprint Goal & User Stories                                |
| Sprint 1 Goal                        | Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado los objetivos del sprint 1.        |
| Sprint 1 Velocity                    | Acordamos aceptar 4 Story Points como nuestra capacidad de entrega para este sprint.     |
| Sum of Story Points                  | La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 1 es 6 |

### 5.2.1.2 Sprint Backlog 1

El Sprint 1 está centrado en la implementación de las funcionalidades clave de la landing page del sitio web, priorizando las historias de usuario identificadas. Nuestro objetivo principal es proporcionar a los visitantes una experiencia inicial sólida al presentar de manera clara y concisa las características y beneficios del sitio, junto con una navegación intuitiva y acceso rápido a la información relevante. Al completar las tareas asociadas a las historias de usuario definidas, sentaremos las bases para futuras iteraciones, asegurando que la página de inicio cumpla con las expectativas de los usuarios y contribuya al éxito del proyecto.

URL del Board en Trello: https://trello.com/b/9fFNzPVl/appweb
![Board Trello](/assets/boardTrello.png)
<table>
    <tr>
        <td colspan="2">Sprint #</td>
        <td colspan="6">Sprint 1</td>
    </tr>
    <tr>
        <td colspan="2">User Story</td>
        <td colspan="6">Work-Item / Task</td>
    </tr>
    <tr>
        <td>Id</td>
        <td>Title</td>
        <td>Id</td>
        <td>Title</td>
        <td>Descripcion</td>
        <td>Estimation (Hours)</td>
        <td>Assigned To</td>
        <td>Status (To-do / In / Process / ToReview / Done)</td>
    </tr>
    <tr>
        <td>US17</td>
        <td>Landing - Resumen del sitio web</td>
        <td>T05</td>
        <td>Desarrollar resumen claro y conciso sobre las características y beneficios del sitio web en la página de inicio.</td>
        <td>Crear una sección de resumen en la página de inicio que presente de manera clara y concisa las principales características y beneficios del sitio web, destacando los puntos más relevantes de manera atractiva y fácil de entender.</td>
        <td>2 hora</td>
        <td>Piero Tarazona</td>
        <td>Done</td>
    </tr>
    <tr>
        <td>US18</td>
        <td>Landing - Resumen de precios</td>
        <td>T06</td>
        <td>Implementar acceso claro y visible a la información detallada de los planes ofrecidos en la página de inicio.</td>
        <td>Integrar un acceso claro y visible en la página de inicio que permita a los visitantes buscar información detallada sobre los planes ofrecidos, incluyendo características, beneficios, limitaciones, términos y condiciones, precio y cualquier otra información relevante.</td>
        <td>3 hora</td>
        <td>Mauricio Chacon</td>
        <td>Done</td>
    </tr>
    <tr>
        <td>US19</td>
        <td>Landing - Información a pie de página</td>
        <td>T07</td>
        <td>Desarrollar un resumen claro y conciso del sitio web al final de la página de inicio.</td>
        <td>Crear un resumen al final de la página de inicio que destaque los aspectos más relevantes del sitio web, como las características principales, los servicios ofrecidos, la información de contacto y cualquier otra información importante para los visitantes.</td>
        <td>1 hora</td>
        <td>Miguel Huarcaya</td>
        <td>Done</td>
    </tr>
    <tr>
        <td>US20</td>
        <td>Landing - Ir a aplicación web directamente</td>
        <td>T08</td>
        <td>Integrar un llamado a la acción claro y visible para dirigir a los visitantes a la aplicación web principal.</td>
        <td>Presentar un llamado a la acción claro y visible en la página de inicio que guíe a los visitantes a explorar más a fondo el sitio web o tomar la acción deseada, como registrarse, suscribirse o contactar al equipo.</td>
        <td>1 hora</td>
        <td>Elias Torres</td>
        <td>Done</td>
    </tr>
    <tr>
        <td>US21</td>
        <td>Landing - Navegación de información</td>
        <td>T09</td>
        <td>Presentar contenido claro, detallado y preciso sobre lo que ofrece el sitio web en la página de inicio.</td>
        <td>Proporcionar contenido claro, detallado y preciso en la página de inicio que describa las características, funcionalidades y beneficios del sitio web de manera comprensible y convincente.</td>
        <td>1 hora</td>
        <td>Moises Donayre</td>
        <td>Done</td>
    </tr>
    <tr>
        <td>US22</td>
        <td>Landing - Navegación de contacto</td>
        <td>T10</td>
        <td>Mostrar información de contacto visible y accesible en la página de inicio.</td>
        <td>Mostrar claramente la información de contacto, como dirección de correo electrónico, número de teléfono y/o dirección física, en una sección destacada de la página de inicio para que los visitantes puedan comunicarse con el sitio web de manera efectiva.</td>
        <td>3 hora</td>
        <td>Elias Torres</td>
        <td>Done</td>
    </tr>
</table>

### 5.2.1.3 Development Evidence for Sprint Review.
Esta sección documenta y presenta la serie de commits realizados en el repositorio del Landing Page. Estos commits, que son una parte integral del proceso de desarrollo, se han gestionado utilizando la metodología GitFlow y siguiendo estrictamente las convenciones establecidas para los commits. Esta evidencia sirve como un registro transparente y trazable de nuestro progreso y esfuerzos de desarrollo a lo largo del sprint.

![Lista de commits](/assets/commits.png)

| Repository                        | Branch              | Commit Id                          | Commit Message                   | Commit Message Body           |Commited on (Date) |
|-----------------------------------|---------------------|------------------------------------|----------------------------------|-------------------------------|-------------------|
| upc-AppWeb-BicasTeam-LandingPage.github.io   | main     | d3b094b | chore: ...                      | initial commit         | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | main     | 499f6c3 | feat: ...                        | create structure for landing            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-header  | a6fd61f                        | feat: ...                        | create header section            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-us  | f46c9f4                        | feat: ...                        | create about us             | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team  | 559b871                        | feat: ...                        | create about team           | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team   | 320162e                        | feat: ...                        | create about team            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team   | 74db128                        | feat: ...                        | create about team           | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team   | 6db4844                        | feat: ...                        | delete file style            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team   | f80d9c2                        | feat: ...                        | create about team            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team   | 77dcfbf                        | feat: ...                        | deleted style           | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team   | 57cd331                        | feat: ...                        | create about team            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team   | 2ac60ee                        | feat: ...                        | deleted style            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team   | a89f5a6                        | feat: ...                        | add folder for organizing files            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team   | 9c04bc0                        | feat: ...                        | create about team           | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team   | e645b3b                        | feat: ...                        | delete public directory            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-about-team   | 1488c1e                        | feat: ...                        | add style and images            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-hero  | 09191fd                        | feat: ...                        | implement hero section            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-hero  | 0ba7ade                        | feat: ...                        | implement footer section            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-footer  | 77037f0                        | feat: ...                        | create footer section            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-pricing  | 84c90ea                        | chore: ...                        | created pricing and contact section                           | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | develop  | c3a6a0c                            | feat: ...                        | merge branch 'feature/section-hero'                           | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | develop  | 4f4b5b7                            | feat: ...                        | merge branch 'feature/section-about-us'                       | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | develop  | e63214c                            | feat: ...                        | merge branch 'feature/section-about-team' into develop        | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | develop  | 7d5209d                            | feat: ...                        | merge branch 'feature/section-services' into develop          | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | develop  | 432e18e                            | feat: ...                        | merge branch 'feature/section-pricing' into develop           | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | develop  | 9b278c2                            | feat: ...                        | merge branch 'feature/section-footer' into develop            | 10-04             |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | main     | fbf4690                            | fix: ...                         | fix the ubication for the code            | 10-04             |

### 5.2.1.4 Testing Suite Evidence for Sprint Review. 
En esta sección, presentamos la evidencia de las pruebas realizadas durante el sprint. Hemos utilizado Gherkin para definir los escenarios de prueba y hemos registrado cada prueba en commits específicos en nuestro repositorio. A continuación, se muestra un registro de estos commits:

| Repository                        | Branch              | Commit Id                          | Commit Message                   | Commit Message Body           |Commited on (Date) |
|-----------------------------------|---------------------|------------------------------------|----------------------------------|-------------------------------|-------------------|
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-header  | 1fbb6f6                           | feat: ...                        | add tests for header section            | 10/04  |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-footer  | ee12b07                          | feat: ...                        | add test for footer section           | 10/04  |
| upc-AppWeb-BicasTeam-LandingPage.github.io   | feature/section-services  | e36977f                            | feat: ...                        | add test for pricing section            | 10/04  |

### 5.2.1.5 Execution Evidence for Sprint Review. 

Durante el Sprint 1, se logró un progreso significativo en la implementación de las características clave de la página de inicio del sitio web. El equipo completó con éxito todas las historias de usuario asignadas para este sprint, que incluyeron el desarrollo de un resumen claro de las características y beneficios del sitio web, la integración de acceso visible a información detallada de precios, la adición de un resumen conciso al final de la página de inicio, la inclusión de un llamado a la acción prominente para dirigir a los visitantes a la aplicación web principal, la presentación de contenido informativo claro y detallado, y la integración de información de contacto visible en la página de inicio. El equipo trabajó de manera colaborativa para garantizar que las características implementadas cumplan con los requisitos y contribuyan a una experiencia de usuario positiva.

Capturas de pantalla:

- Sección de Resumen:

![Resumen](/assets/resumen.png)

- Acceso a la Información de Precios:

![Precios](/assets/precios.png)

- Resumen al Final:

![Footer](/assets/footer.png)

- Contenido Informativo:

![Board Trello](/assets/servicios.png)

- Llamado a la acción

![Board Trello](/assets/calltoAction.png)

- Sección de Información de Contacto:

![Contacto](/assets/contacto.png)

Video: https://upcedupe-my.sharepoint.com/:v:/g/personal/u202212911_upc_edu_pe/EdWszOh699pDu919Y5P6xZcBELghHGlX6WIoZ03PN5I0mA?e=5AvfFc&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

### 5.2.1.6 Services Documentation Evidence for Sprint Review. 

Durante este Sprint 1, nos enfocamos en desarrollar el landing page, sin implementación de cualquier servicio. Por lo tanto, este punto quedará sin actividad en este aspecto.

### 5.2.1.7 Software Deployment Evidence for Sprint Review.

Durante el Sprint 1, llevamos a cabo el despliegue de nuestra landing page en GitHub Pages. A continuación, detallamos los pasos realizados:

1. Creación del Repositorio en GitHub: Iniciamos creando un repositorio dedicado en GitHub para nuestro proyecto de landing page.
2. Configuración de la Rama main: Aseguramos que la rama principal del repositorio se llamara main, ya que GitHub Pages toma esta rama como base para el despliegue automático.
3. Preparación del Contenido: Desarrollamos y diseñamos nuestra landing page, asegurándonos de que todos los archivos y recursos necesarios estuvieran presentes en el repositorio.
4. Generación del Enlace de GitHub Pages: Navegamos a la sección "Pages" en la configuración del repositorio en GitHub. Configuramos la fuente del GitHub Pages para que tomara el contenido de la rama main.
5. Despliegue Automático: GitHub Pages automáticamente detectó los cambios en la rama main y desplegó la landing page en la URL proporcionada por GitHub Pages.

### 5.2.1.8 Team Collaboration Insights during Sprint.

Durante este primer Sprint, hemos completado el desarrollo del landing page y hemos colaborado estrechamente en su implementación. La colaboración entre los miembros del equipo se refleja en los diversos commits realizados en el repositorio de GitHub, los cuales han sido debidamente documentados en las capturas de pantalla adjuntas.
Para asegurar una colaboración efectiva, hemos implementado GitFlow como nuestra metodología de trabajo colaborativo en Git. Con GitFlow, hemos creado ramas para cada una de las secciones de nuestra landing page. Esto nos ha permitido trabajar de manera organizada y centrarnos en completar correctamente las historias de usuario designadas para cada sección.
En cuanto a la elaboración del código, hemos asignado a cada miembro del equipo una sección específica del landing page. Esta estrategia nos ha permitido avanzar de manera más eficiente y completar el trabajo antes de la fecha de entrega.
Además, hemos realizado reuniones adicionales para intercambiar ideas y resolver cualquier duda o problema que pudiera surgir durante el desarrollo del landing page. Estas sesiones han contribuido de manera positiva al éxito del proyecto.
A continuación, presentamos algunas capturas de pantalla que muestran los commits realizados por los miembros del equipo en GitHub:
![Ramas](/assets/branches.png)

![Miguel](/assets/miguel.png)

![Mauricio](/assets/mauricio.png)

![Piero](/assets/piero.png)

![Elias](/assets/elias.png)

![Moises](/assets/moises.png)

### 5.2.2 Sprint 2
En esta sección, comentaremos y explicaremos el progreso tanto en el desarrollo del producto como en la colaboración del equipo durante el Sprint 2. Seguimos un proceso definido que abarca desde la planificación hasta la revisión y documentación del trabajo realizado. A lo largo de las siguientes secciones, detallaremos cómo se llevó a cabo la planificación del sprint, qué tareas se incluyeron en el Sprint Backlog, las pruebas y evidencia de desarrollo para la revisión del sprint, así como la documentación de los servicios y las percepciones clave sobre la colaboración del equipo durante este periodo.

#### 5.2.2.1 Sprint Planning 2
En esta sección, se detallan los aspectos principales del Sprint Planning Meeting para el Sprint n. Este encuentro es crucial para establecer los objetivos del sprint, determinar las user stories que se abordarán y asignar tareas al equipo. A continuación, se presenta un resumen del Sprint Planning Meeting para este período.

|Sprint #|Sprint 2|
| :- | :- |
|Sprint Planning Background||
|Date|2024-04-22|
|Time|07:06 PM|
|Location|Google Meet|
|Prepared by|Piero Abel Tarazona Medina|
|Attendees (to planning meeting)|Piero Tarazona, Mauricio Chacon, Elias, Moises Donayre, Miguel|
|Sprint 2 – 1 Review Summary|Sprint 2 fue un éxito en términos de avance del frontend de la aplicación web y colaboración efectiva del equipo. Los logros alcanzados y la retroalimentación recopilada durante esta revisión proporcionan una base sólida para el siguiente sprint y refuerzan el compromiso del equipo con la calidad y la entrega oportuna del producto.|
|Sprint 2 – 1 Retrospective Summary|Para la retrospectiva del Sprint 2 nos sirvió para reflexionar sobre el desempeño del equipo e identificar áreas de mejora. Esto nos servirá como base para impulsar la mejora continua y optimizar el trabajo del equipo en los próximos sprints.|
|Sprint Goal & User Stories||
|Sprint 1 Goal|Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado los objetivos del sprint 2.|
|Sprint 1 Velocity|Con el equipo para este sprint 2 decidimos aceptar 7 Story Points|
|Sum of Story Points|La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 2 es 21|

#### 5.2.2.2 Sprint Backlog 2
El Sprint 2 está centrado en el frontend de nuestra aplicación web, priorizando las historias de usuario identificadas. Nuestro objetivo principal es proporcionar a los usuarios una experiencia inicial sólida al presentar una navegación intuitiva y acceso rápido a las funcionalidades relevantes. Al completar las tareas asociadas a las historias de usuario definidas, sentaremos una buena base para la aplicación web, asegurando que lo propuesto contribuya al éxito del proyecto.

URL del Board en Trello: 

https://trello.com/b/5B5dHJXJ/appweb-sprinbacklog-2 

![trello sprint 2](/assets/chapter05%20-%20spring%202/trello-print-backlog-2.png)

|Sprint #|Sprint 2|||||||
| :- | :- | :- | :- | :- | :- | :- | :- |
|User Story|Work-Item / Task|||||||
|Id|Title|Id|Title|Descripción|Estimation (Hours)|Assigned to|Status (To-do / In / Process / ToReview / Done)|
|US02|Visualización de reportes de un transportista.|T07|Desarrollo de la función de reportes para transportistas|Establecer una conexión entre la funcionalidad y la base de datos para obtener los reportes de cada transportista.|4|Piero Tarazona|Done|
|US13|Reporte de infracciones|T08|Implementación de reporte de infracciones vehiculares|Crear las estructuras de datos necesarias para almacenar la información de las infracciones que reporte un transportista|5|Piero Tarazona|Done|
|US10|Gestión de inventario de flotas|T09|Incorporación de una gestión de flotas vehiculares|Crear un sistema de gestión de inventario de flotas que permita al gerente visualizar y agregar nuevas flotas al negocio.|5|Mauricio Chacon|Done|
|US11|Modificar perfil de gerente|T10|Sistema de modificación de perfiles de gerentes|Permitir la modificación de los campos del perfil del gerente, incluyendo información personal y credenciales de acceso.|5|Miguel Huarcaya|Done|
|US12|Modificar perfil de transportistas|T11|Sistema de modificación de perfiles de transportistas|Permitir la modificación de los campos del perfil del transportista, incluyendo información personal y credenciales de acceso.|6|Mauricio Chacon|Done|
|US03|Visualización de envíos asignados a un transportista.|T12|Implementar envios a transportista|Desarrollar un sistema que permita obtener la información de los envíos asignados a los transportistas, facilitando el seguimiento y la gestión de las entregas en tiempo real.|6|Elias Torres|Done|
|US08|Visualización de historial de envíos|T13|Implementar historial de envíos|Implementar la funcionalidad que permita recuperar y presentar los envíos asignados a un transportista específico, proporcionando una visión clara de las tareas pendientes y completadas por cada miembro del equipo de transporte.|5|Moises Donayre|Done|

#### 5.2.2.3 Development Evidence for Sprint Review
Esta sección documenta y presenta la serie de commits realizados en el repositorio de la Aplicación Web. Estos commits, que son una parte integral del proceso de desarrollo, se han gestionado utilizando la metodología GitFlow y siguiendo estrictamente las convenciones establecidas para los commits. Esta evidencia sirve como un registro transparente y trazable de nuestro progreso y esfuerzos de desarrollo a lo largo del sprint.

![Development evidence](/assets//chapter05%20-%20spring%202/sprint2-developmentEvidenceSprint.jpg)

|Repository|Branch|Commit Id|Commit Message|Commit Message Body|Committed on (Date)|
| :-: | :-: | :-: | :-: | :-: | :-: |
|upc-pre-202401-si729-sv54-bicasteam-app-web|main|f4745dd|chore|create project with Vite + Vue.js|22-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|main|6a269f7|chore|created carpets|23-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/display-of-carrier-statistics|e221a5b|feat|added default configuration for remote services client|23-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/display-of-carrier-statistics|4858997|feat|added configuration for in-app navigation|25-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/display-of-carrier-statistics|44502a1|doc|updated documentation with summary, features and dependencies|25-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/display-of-carrier-statistics|36b609a|feat|implemented main view integrating in-app navigation|27-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/display-of-carrier-statistics|a101c7a|feat|add report view in table|27-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/display-of-carrier-statistics|17863f0|feat|add sidebar component|29-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/display-of-carrier-statistics|61fba68|feat|updated table information, now driver names are shown by another json file|29-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/display-of-carrier-statistics|240de24|fix|app.vue name|30-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/main-content-flow|4858997|feat|added configuration for in-app navigation support|22-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/main-content-flow|18a5257|feat|added login page and route|22-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/main-content-flow|9f107ab|feat|add regsiter type selection account|22-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/main-content-flow|0b1da44|feat|register validations added|25-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/main-content-flow|a40221f|fix|path of login component and redirect|25-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/main-content-flow|2bb7de8|feat|update db.json|27-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/main-content-flow|9f3f805|fix|count class|27-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/main-content-flow|051757c|fix|json and endpoints|29-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/main-content-flow|4f87ae5|fix|fix components in profiles-mangment bounded countext|29-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/personal-data-managment|3dd439b|feat|change textinputarea color|25-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/personal-data-managment|f5efa83|feat|add api connection to display data from fakeAPI|25-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/personal-data-managment|e3cf545|feat|refactor data-view component|27-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/personal-data-managment|d291656|feat|add form for profile management|27-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/personal-data-managment|83da2e8|feat|add sidebar component|29-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/shipment-managment|b199910|feat|added view shipment component|22-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/shipment-managment|3db8a08|feat|added option to view details of each shipment and add new shipment and add new shipments|25-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/shipment-managment|d48519d|feat|updated connection with my json server|28-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/shipment-managment|7fa96e9|feat|added visualization of shipments|30-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/vehicules-managment|ea6e12b|feat|add vehicles-businessman methods|22-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/vehicules-managment|2758ab3|feat|add display-vehicles-businessman page|25-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/vehicules-managment|ec567a2|feat|direction for vechiles|27-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/vehicules-managment|beb6dd7|fix|routes and information from login|27-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/vehicules-managment|3dd439b|feat|change textinputarea color|27-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/vehicules-managment|2d6d5e7|feat|ddded route for vehicle fleet view|29-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|develop|9cb2d63|feat|page vehicle carrier|30-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|develop|fef7d7b|feat|add services|30-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|develop|c8e9bfb|fix|type in sidebar|30-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|develop|2758ab3|feat|add display-vehicles-businessman page|30-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|develop|ea6e12b|feat|add vehicles-businessman methods|30-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|develop|1b028ef|fix|fix components in profiles managment bounded context|30-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|develop|28c141d|feat|routes implemented and merge|30-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|develop|6cc6e44|feat|setting funcionality|30-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|develop|b199910|feat|added view shipment component|30-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|develop|26c5b8d|feat|merge and implemented shipments|30-04|

#### 5.2.2.4 Testing Suite Edvidence for Sprint Review
En esta sección, presentamos la evidencia de las pruebas realizadas durante el sprint. Hemos utilizado Gherkin para definir los escenarios de prueba y hemos registrado cada prueba en commits específicos en nuestro repositorio. A continuación, se muestra un registro de estos commits:

|Repository|Branch|Commit Id|Commit Message|Commit Message Body|Commited on (Date)|
| :- | :- | :- | :- | :- | :- |
|upc-pre-202401-si729-sv54-bicasteam-app-web|featuredisplay-of-carrier-statistics|e221a5b|feat: ...|add test for display of carrier statistics|29-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/main-content-flow|4858997|feat: ...|add test for main content flow|29-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/personal-data-managment|3dd439b|feat: ...|add test for personal data managment|29-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/shipment-managment|b199910|feat: ...|<p>add test for shipment managment</p><p></p>|29-04|
|upc-pre-202401-si729-sv54-bicasteam-app-web|feature/vehicules-managment|ea6e12b|feat: ...|add test for vehicules managment|29-04|

#### 5.2.2.5 Execution Evidence for Sprint Review
Durante el Sprint 2, se logró un progreso significativo en la implementación de las características clave del frontend en la aplicación web. El equipo completó con éxito las historias de usuario asignadas para este sprint, que incluyeron el desarrollo del frontend en nuestra aplicación web, también con la integración de acceso visible a todas las opciones, incluso de un llamado a la acción prominente para dirigir a los visitantes a la aplicación web. El equipo trabajó de manera colaborativa para garantizar que las características implementadas cumplan con los requisitos y contribuyan a una experiencia de usuario positiva.

Capturas de pantalla:
![Execution evidence](/assets/chapter05%20-%20spring%202/ExecutionEvidenceSpirntReview1.png)

![Execution evidence 2](/assets/chapter05%20-%20spring%202/ExecutionEvidenceSpirntReview2.png)

#### 5.2.2.6 Serivces Documentation Evidence for Sprint Review
Durante este Sprint 2, nos enfocamos en desarrollar el “App web Solution”, sin implementación de ningún servicio. Por lo tanto, este punto quedará sin actividad en este aspecto.

#### 5.2.2.7 Software Deployment Evidence for Sprint Review
Durante el Sprint 2, llevamos a cabo el despliegue de nuestra aplicación web en GitHub Pages. A continuación, detallamos los pasos realizados:

- Creación del Repositorio en GitHub: Iniciamos creando un repositorio dedicado en GitHub para nuestro proyecto de aplicación web.
- Configuración de la Rama main: Aseguramos que la rama principal del repositorio se llamará main, ya que GitHub Pages toma esta rama como base para el despliegue automático.
- Preparación del Contenido: Desarrollamos y diseñamos nuestra aplicación web, asegurándonos de que todos los archivos y recursos necesarios estuvieran presentes en el repositorio.
- Generación del enlace de GitHub Pages: Navegamos a la sección "Pages" en la configuración del repositorio en GitHub. Configuramos la fuente del GitHub Pages para que tomara el contenido de la rama main.
- Despliegue Automático: GitHub Pages automáticamente detectó los cambios en la rama main y desplegó la aplicación web en la URL proporcionada por GitHub Pages.

#### 5.2.2.8 Team collaboration insights during Sprint
Durante este segundo Sprint, hemos avanzado el desarrollo de la aplicación web y hemos colaborado estrechamente en su implementación. La colaboración entre los miembros del equipo se refleja en los diversos commits realizados en el repositorio de GitHub, los cuales han sido debidamente documentados en las capturas de pantalla adjuntas. Para asegurar una colaboración efectiva, hemos implementado GitFlow como nuestra metodología de trabajo colaborativo en Git. Con GitFlow, hemos creado ramas para cada una de las secciones de nuestra aplicación web. Esto nos ha permitido trabajar de manera organizada y centrarnos en completar correctamente las historias de usuario designadas para cada sección. En cuanto a la elaboración del código, hemos asignado a cada miembro del equipo una sección específica de la aplicación web. Esta estrategia nos ha permitido avanzar de manera más eficiente y completar el trabajo antes de la fecha de entrega. Además, hemos realizado reuniones adicionales para intercambiar ideas y resolver cualquier duda o problema que pudiera surgir durante el desarrollo del landing page. Estas sesiones han contribuido de manera positiva al éxito del proyecto. A continuación, presentamos algunas capturas de pantalla que muestran los commits realizados por los miembros del equipo en GitHub:

![Team Collaboration Insights](/assets/chapter05%20-%20spring%202/TeamCollaborationInsightDuringSprint.png)

---

### 5.2.3 Sprint 3
En esta sección, comentaremos y explicaremos el progreso tanto en el desarrollo del producto como en la colaboración del equipo durante el Sprint 3. Seguimos un proceso definido que abarca desde la planificación hasta la revisión y documentación del trabajo realizado. A lo largo de las siguientes secciones, detallaremos cómo se llevó a cabo la planificación del sprint, qué tareas se incluyeron en el Sprint Backlog, las pruebas y evidencia de desarrollo para la revisión del sprint, así como la documentación de los servicios y las percepciones clave sobre la colaboración del equipo durante este periodo.

#### 5.2.3.1 Sprint Planning 3
En esta sección, se detallan los aspectos principales del Sprint Planning Meeting para el Sprint n. Este encuentro es crucial para establecer los objetivos del sprint, determinar las user stories que se abordarán y asignar tareas al equipo. A continuación, se presenta un resumen del Sprint Planning Meeting para este período.
|Sprint #|Sprint 3|
| :- | :- |
|Sprint Planning Background||
|Date|2024-05-24|
|Time|04:23 PM|
|Location|Google Meet|
|Prepared by|Piero Abel Tarazona Medina|
|Attendees (to planning meeting)|Moises Rodolfo Donayre Peña, Mauricio Sebastián Chacon Martinez, Flavio Eduardo Trigueros Chumacero, Piero Abel Tarazona Medina|
|Sprint 3 – 1 Review Summary|Después de realizar todos los procedimientos establecidos para la identificación de objetivos y áreas de retroalimentación, hemos podido concluir la reunión del sprint 3 con éxito en términos de avance en los productos de software y en la colaboración general del equipo. El proceso de mejora con la retroalimentación y la programación de varias secciones nuevas en el servicio web significó un gran proceso de mejora para la construcción y realización del sprint, además de reforzar el compromiso de nuestro equipo y la mejora exponencial de las actividades indicadas.|
|Sprint 3 – 1 Retrospective Summary|Para el proceso de la retrospectiva del Sprint 3, fue necesario que nuestro equipo revisará a detalle toda la retroalimentación recibida ante el primer sprint realizado, para luego generar un análisis a profundidad del desempeño general e individual de todos los miembros del equipo de trabajo. Después de ese proceso, pudimos identificar varias áreas de mejora en las cuales centrarnos para así poder garantizar la entrega de un mejor trabajo y un buen producto para todos nuestros clientes, promoviendo la mejora continua y optimizando los métodos de trabajo en los próximos sprints durante el ciclo de vida del proyecto.|
|Sprint Goal & User Stories||
|Sprint 3 Goal|Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado los objetivos del sprint 3.|
|Sprint 3 Velocity|Con el equipo para este sprint 3 decidimos aceptar 6 Story Points|
|Sum of Story Points|La suma de los Story Points para los User Stories que se están incluyendo en este Sprint es 32.|

#### 5.2.3.2 Sprint Backlog 3
El Sprint 3 está centrado en el servicio web, priorizando las historias de usuario identificadas. Nuestro objetivo principal es proporcionar a los usuarios una experiencia inicial sólida al presentar una navegación intuitiva y acceso rápido a las funcionalidades relevantes. Al completar las tareas asociadas a las historias de usuario definidas, sentaremos una buena base para el servicio web, asegurando que lo propuesto contribuya al éxito del proyecto.

URL del Board en Trello:

https://trello.com/b/vTLeIEal/appweb-sprintbacklog-3 

![Trello Sprint 3](/assets/chapter05%20-%20spring%203/trello-sprint-3.png)

|&emsp;&emsp;&emsp;&emsp;<a name="_heading=h.kn5t1eh5nzqr"></a>Sprint #|&emsp;&emsp;&emsp;&emsp;Sprint 3|||||||
| :- | :- | :- | :- | :- | :- | :- | :- |
|&emsp;&emsp;&emsp;&emsp;User Story|&emsp;&emsp;&emsp;&emsp;Work-Item / Task|||||||
|&emsp;&emsp;&emsp;&emsp;Id|&emsp;&emsp;&emsp;&emsp;Title|&emsp;&emsp;&emsp;&emsp;Id|&emsp;&emsp;&emsp;&emsp;Title|&emsp;&emsp;&emsp;&emsp;Descripción|&emsp;&emsp;&emsp;&emsp;Estimation (Hours)|&emsp;&emsp;&emsp;&emsp;Assigned to|&emsp;&emsp;&emsp;&emsp;Status (To-do / In / Process / ToReview / Done)|
|&emsp;&emsp;&emsp;&emsp;US09|&emsp;&emsp;&emsp;&emsp;Asignación de flotas|&emsp;&emsp;&emsp;&emsp;T14|&emsp;&emsp;&emsp;&emsp;Desarrollo de interfaz y lógica de asignación de flotas|&emsp;&emsp;&emsp;&emsp;Crear una interfaz en la aplicación web que permita al gerente seleccionar y asignar flotas a los transportistas, junto con la lógica de backend necesaria para actualizar las bases de datos con las asignaciones realizadas.|&emsp;&emsp;&emsp;&emsp;4|&emsp;&emsp;&emsp;&emsp;Piero Tarazona|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US14|&emsp;&emsp;&emsp;&emsp;Reporte de accidentes en la carretera|&emsp;&emsp;&emsp;&emsp;T15|&emsp;&emsp;&emsp;&emsp;Implementación de sistema de reporte de accidentes|&emsp;&emsp;&emsp;&emsp;Crear un formulario en la aplicación móvil o web para que los transportistas reporten accidentes, junto con un endpoint en el servidor que reciba y almacene los reportes, e implemente notificaciones automáticas a los gerentes.|&emsp;&emsp;&emsp;&emsp;5|&emsp;&emsp;&emsp;&emsp;Mauricio Chacon|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US15|&emsp;&emsp;&emsp;&emsp;Reporte de problemas con el paquete|&emsp;&emsp;&emsp;&emsp;T16|&emsp;&emsp;&emsp;&emsp;Implementación de sistema de reporte de problemas con el paquete|&emsp;&emsp;&emsp;&emsp;Crear un formulario en la aplicación móvil o web para reportar problemas con los paquetes, junto con un endpoint en el servidor que reciba y almacene los reportes, e implemente notificaciones automáticas a los gerentes y clientes.|&emsp;&emsp;&emsp;&emsp;4|&emsp;&emsp;&emsp;&emsp;Miguel Huarcaya|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US16|&emsp;&emsp;&emsp;&emsp;Reporte de problemas técnicos|&emsp;&emsp;&emsp;&emsp;T17|&emsp;&emsp;&emsp;&emsp;Implementación de sistema de reporte de problemas técnicos|&emsp;&emsp;&emsp;&emsp;Crear un formulario en la aplicación móvil o web para reportar problemas técnicos, junto con un endpoint en el servidor que reciba y almacene los reportes, e implementa notificaciones automáticas a los gerentes.|&emsp;&emsp;&emsp;&emsp;5|&emsp;&emsp;&emsp;&emsp;Elias Torres|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US23|&emsp;&emsp;&emsp;&emsp;Eliminar registro|&emsp;&emsp;&emsp;&emsp;T18|&emsp;&emsp;&emsp;&emsp;Desarrollo de endpoint para eliminar registro|&emsp;&emsp;&emsp;&emsp;Crear un endpoint en la API que permite eliminar registros específicos de la base de datos, incluyendo la lógica de backend para realizar las verificaciones necesarias antes de la eliminación.|&emsp;&emsp;&emsp;&emsp;4|&emsp;&emsp;&emsp;&emsp;Moises Donayre|&emsp;&emsp;&emsp;&emsp;Done|
|<p>&emsp;&emsp;&emsp;&emsp;US24</p><p>&emsp;&emsp;&emsp;&emsp;</p>|&emsp;&emsp;&emsp;&emsp;Agregar registro|&emsp;&emsp;&emsp;&emsp;T19|&emsp;&emsp;&emsp;&emsp;Desarrollo de endpoint para agregar registro|&emsp;&emsp;&emsp;&emsp;Crear un endpoint en la API que permita agregar nuevos registros a la base de datos, incluyendo la lógica de backend para validar los datos antes de su inserción.|&emsp;&emsp;&emsp;&emsp;5|&emsp;&emsp;&emsp;&emsp;Piero Tarazona|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US25|&emsp;&emsp;&emsp;&emsp;Actualizar registro|&emsp;&emsp;&emsp;&emsp;T20|&emsp;&emsp;&emsp;&emsp;Desarrollo de endpoint para actualizar registro|&emsp;&emsp;&emsp;&emsp;Crear un endpoint en la API que permita actualizar registros existentes en la base de datos, incluyendo la lógica de backend para validar los datos antes de su actualización.|&emsp;&emsp;&emsp;&emsp;5|&emsp;&emsp;&emsp;&emsp;Mauricio Chacon|&emsp;&emsp;&emsp;&emsp;Done|

#### 5.2.3.3 Development Evidence for Sprint Review
Esta sección documenta y presenta la serie de commits realizados en el repositorio del Servicio Web. Estos commits, que son una parte integral del proceso de desarrollo, se han gestionado utilizando la metodología GitFlow y siguiendo estrictamente las convenciones establecidas para los commits. Esta evidencia sirve como un registro transparente y trazable de nuestro progreso y esfuerzos de desarrollo a lo largo del sprint.

![Development Evidence fpr Spóinrt Review](/assets/chapter05%20-%20spring%203/DevelopmetEvidenceForSprintReview%203.png)

|Repository|Branch|Commit Id|Commit Message|Commit Message Body|Committed on (Date)|
| :-: | :-: | :-: | :-: | :-: | :-: |
|upc-AppWeb-BicasTeam-Api|main|cc1ecb8|chore|create default project|27-05|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|3c630b1|chore|implemented persistence base configuration|27-05|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|46d523d|feat|added aggregate user|27-05|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|05ef98f|feat|added user repository|27-05|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|7b06c81|feat|implemented query service and command for user aggregate|27-05|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|431353c|feat|added user controller|27-05|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|554df5b|chore|implemented persistence base configuration|27-05|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|5475552|fix|base configuration|27-05|
|upc-AppWeb-BicasTeam-Api|feature/shipments|cb61040|feat|added layers domain, infrastructure and application|28-05|
|upc-AppWeb-BicasTeam-Api|feature/shipments|b913385|feat|added resources and transform|28-05|
|upc-AppWeb-BicasTeam-Api|feature/shipments|9ee7c1c|feat|added shipment controller|28-05|
|upc-AppWeb-BicasTeam-Api|feature/shipments|8cdc129|chore|implemented interface layer base configuration, including configuration statements in main program|28-05|
|upc-AppWeb-BicasTeam-Api|feature/shipments|132998c|chore|added database context|28-05|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|49269c5|feat|added report aggregate|01-06|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|7c0c3ef|feat|added repositories and services for the model|01-06|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|328d93b|feat|added infrastructure and application for the report|01-06|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|77af4a6|feat|added resources and transform|01-06|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|a0a9813|chore|implemented interface layer base configuration, including configuration statements in main program|01-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|0977fa1|feat|added aggregate vehicle|02-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|0ce3c84|feat|added command and query services|02-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|a6fac64|feat|added resources and transform|02-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|ee78294|feat|added vehicle controller|02-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|3395c27|chore|implemented interface layer base configuration in main program|02-06|

#### 5.2.3.4 Testing Suite Evidence for Sprint Review
En esta sección, presentamos la evidencia de las pruebas realizadas durante el sprint. Hemos utilizado Gherkin para definir los escenarios de prueba y hemos registrado cada prueba en commits específicos en nuestro repositorio. A continuación, se muestra un registro de estos commits:

|Repository|Branch|Commit Id|Commit Message|Commit Message Body|Commited on (Date)|
| :- | :- | :- | :- | :- | :- |
|upc-AppWeb-BicasTeam-Api|feature/profile-management|328d93b|feat|add test for profile management|02-06|
|upc-AppWeb-BicasTeam-Api|feature/shipments|132998c|feat|add test for shipments|02-06|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|7c0c3ef|feat|add test for communication-reports|02-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|e221a5b|feat|add test for vehicles|02-06|

#### 5.2.3.5 Execution Evidence for Sprint Review
El equipo ha logrado despegar el web service de MoviGestion. Todas las historias de usuario asignadas para este sprint fueron completadas exitosamente. En primer lugar, nos enfocamos en el desarrollo y la implementación del web service que es fundamental para la aplicación MoviGestion. Este esfuerzo incluyó la creación de APIs RESTful, la integración segura y eficiente con la base de datos, y la implementación de pruebas exhaustivas para asegurar la fiabilidad y el rendimiento del servicio. 

Capturas de pantalla:

![CAPTURAS DEL WEB SERVICE DESPLEGADO](/assets/chapter05%20-%20spring%203/executionEvidenceSprint3_0.jpg)

![CAPTURAS DEL WEB SERVICE DESPLEGADO 2](/assets/chapter05%20-%20spring%203/executionEvidenceSprint3_1.jpg)


#### 5.2.3.6 Services Documentation Evidence for Sprint Review
Durante el Sprint 3, el equipo ha trabajado intensamente en la documentación de los Web Services desarrollados. Utilizando OpenAPI, hemos documentado todos los endpoints relevantes, asegurando que cada uno de ellos esté claramente definido y accesible para los desarrolladores. Esta documentación es esencial para garantizar una integración fluida y eficiente del web service con otros componentes de la aplicación y con sistemas externos.

|&emsp;&emsp;&emsp;&emsp;Endpoint|&emsp;&emsp;&emsp;&emsp;Acción Implementada|&emsp;&emsp;&emsp;&emsp;Verbo HTTP|&emsp;&emsp;&emsp;&emsp;Sintaxis de Llamada|&emsp;&emsp;&emsp;&emsp;Parámetros|&emsp;&emsp;&emsp;&emsp;Ejemplo de Response|
| :- | :- | :- | :- | :- | :- |
|&emsp;&emsp;&emsp;&emsp;/report|&emsp;&emsp;&emsp;&emsp;Crear reporte|&emsp;&emsp;&emsp;&emsp;POST|&emsp;&emsp;&emsp;&emsp;/api/v1/report|&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/report/{id}|&emsp;&emsp;&emsp;&emsp;Obtener reporte por Id|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/report/{id}|&emsp;&emsp;&emsp;&emsp;id|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/report/user/{userId}|&emsp;&emsp;&emsp;&emsp;Obtener reportes por id de usuario|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/report/users/{userId}|&emsp;&emsp;&emsp;&emsp;userId|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/report|&emsp;&emsp;&emsp;&emsp;Obtener todo los reportes|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/report|&emsp;&emsp;&emsp;&emsp;none|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/vehicle|&emsp;&emsp;&emsp;&emsp;Crear vehiculo|&emsp;&emsp;&emsp;&emsp;POST|&emsp;&emsp;&emsp;&emsp;/api/v1/vehicle|&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/vehicle/{id}|&emsp;&emsp;&emsp;&emsp;Obtener vehículo por Id|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/vehicle/{id}|&emsp;&emsp;&emsp;&emsp;id|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/vehicle|&emsp;&emsp;&emsp;&emsp;Obtener todo los vehículos|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/vehicle|&emsp;&emsp;&emsp;&emsp;none|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/shipment|&emsp;&emsp;&emsp;&emsp;Crear envío|&emsp;&emsp;&emsp;&emsp;POST|&emsp;&emsp;&emsp;&emsp;/api/v1/shipment|&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/shipment/{id}|&emsp;&emsp;&emsp;&emsp;Obtener envío por Id|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/shipment/{id}|&emsp;&emsp;&emsp;&emsp;id|&emsp;&emsp;&emsp;&emsp;|
|<p>&emsp;&emsp;&emsp;&emsp;/shipment/user/{userId}</p><p>&emsp;&emsp;&emsp;&emsp;</p>|&emsp;&emsp;&emsp;&emsp;Obtener envíos por id de usuario|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/shipment/users/{userId}|&emsp;&emsp;&emsp;&emsp;userId|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/shipment|&emsp;&emsp;&emsp;&emsp;Obtener todo los envíos|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/shipment|&emsp;&emsp;&emsp;&emsp;none|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/user|&emsp;&emsp;&emsp;&emsp;Crear perfil|&emsp;&emsp;&emsp;&emsp;POST|&emsp;&emsp;&emsp;&emsp;/api/v1/user|&emsp;&emsp;&emsp;&emsp;|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/user/{id}|&emsp;&emsp;&emsp;&emsp;Obtener perfil por Id|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/user/{id}|&emsp;&emsp;&emsp;&emsp;id|&emsp;&emsp;&emsp;&emsp;|
|&emsp;&emsp;&emsp;&emsp;/user|&emsp;&emsp;&emsp;&emsp;Obtener todo los perfil|&emsp;&emsp;&emsp;&emsp;GET|&emsp;&emsp;&emsp;&emsp;/api/v1/user|&emsp;&emsp;&emsp;&emsp;none|&emsp;&emsp;&emsp;&emsp;|

CAPTURAS DE INTERACCION CON LA DOCUMENTACION:

A continuación, se incluyen capturas de pantalla que muestran la interacción con la documentación de los web services, utilizando datos de muestra.

1. Endopoint de crear Reporte (/report) - POST

![1](/assets/chapter05%20-%20spring%203/post.png)

Descripción: La captura muestra la documentación del endpoint para crear un nuevo reporte, incluyendo los parámetros requeridos y un ejemplo del response.

2. Endpoint de Obtener Reporte por ID (/report/{id}) - GET:

![2](/assets/chapter05%20-%20spring%203/get.png)

Descripción: La captura presenta la documentación del endpoint para obtener un reporte por ID, con la sintaxis de llamada y un ejemplo de response.

3. Endpoint de Crear Vehículo (/vehicle) - POST:

![3](/assets/chapter05%20-%20spring%203/post-veh.png)

Descripción: La imagen muestra cómo documentamos la creación de un nuevo vehículo, especificando los parámetros y un ejemplo del response.

4. Endpoint de Obtener Envío por ID (/shipment/{id}) - GET:

![4](/assets/chapter05%20-%20spring%203/get-id.png)

 Descripción: La captura ilustra la documentación del endpoint para obtener un envío por ID, incluyendo un ejemplo del request y response.

 #### <a name="_heading=h.ikcf394glpjk"></a>**URL del Repositorio:**
   El código fuente del Web Services se encuentran en el siguiente repositorio:

- **Repositorio de Web Service:** [upc-AppWeb-BicasTeam/upc-AppWeb-BicasTeam-Api: Bicas Team - Movigestion - API (github.com)](https://github.com/upc-AppWeb-BicasTeam/upc-AppWeb-BicasTeam-Api)

#### 5.2.3.7 Software Deployment Evidence for Sprint Review
Durante el Sprint 3, llevamos a cabo el despliegue de nuestra web service en GitHub Pages. A continuación, detallamos los pasos realizados:

- Creación del Repositorio en GitHub: Iniciamos creando un repositorio dedicado en GitHub para nuestro proyecto de web service.
- Configuración de la Rama main: Aseguramos que la rama principal del repositorio se llamará main, ya que esta rama sirve como base para el despliegue automático.
- Preparación del Contenido: Desarrollamos y diseñamos nuestra web service, asegurándonos de que todos los archivos y recursos necesarios estuvieran presentes en el repositorio.
- Generación del enlace del hosting: Creamos nuestra cuenta en el hosting, le asignamos un nombre y desplegamos el web service en la URL proporcionada por el hosting.

#### 5.2.3.8 Team Collaboration Insights During Sprint
Durante este segundo Sprint, hemos avanzado el desarrollo del web service y hemos colaborado estrechamente en su implementación. La colaboración entre los miembros del equipo se refleja en los diversos commits realizados en el repositorio de GitHub, los cuales han sido debidamente documentados en las capturas de pantalla adjuntas. Para asegurar una colaboración efectiva, hemos implementado GitFlow como nuestra metodología de trabajo colaborativo en Git. Con GitFlow, hemos creado ramas para cada una de las secciones de nuestro web service. Esto nos ha permitido trabajar de manera organizada y centrarnos en completar correctamente las historias de usuario designadas para cada sección. En cuanto a la elaboración del código, hemos asignado a cada miembro del equipo una sección específica del web service. Esta estrategia nos ha permitido avanzar de manera más eficiente y completar el trabajo antes de la fecha de entrega. Además, hemos realizado reuniones adicionales para intercambiar ideas y resolver cualquier duda o problema que pudiera surgir durante el desarrollo del web service. Estas sesiones han contribuido de manera positiva al éxito del proyecto. A continuación, presentamos algunas capturas de pantalla que muestran los commits realizados por los miembros del equipo en GitHub:

![Team Collaobraiton](/assets/chapter05%20-%20spring%203/TeamCollaborationInsightsDuringSprint%203.png)

---

### 5.2.4 Sprint 4

En esta sección, comentaremos y explicaremos el progreso tanto en el desarrollo del producto como en la colaboración del equipo durante el Sprint 4. Seguimos un proceso definido que abarca desde la planificación hasta la revisión y documentación del trabajo realizado. A lo largo de las siguientes secciones, detallaremos cómo se llevó a cabo la planificación del sprint, qué tareas se incluyeron en el Sprint Backlog, las pruebas y evidencia de desarrollo para la revisión del sprint, así como la documentación de los servicios y las percepciones clave sobre la colaboración del equipo durante este periodo.

#### 5.2.4.1 Sprint Planning 4

En esta sección, se detallan los aspectos principales del Sprint Planning Meeting para el Sprint 4. Este encuentro es crucial para establecer los objetivos del sprint, determinar las user stories que se abordarán y asignar tareas al equipo. A continuación, se presenta un resumen del Sprint Planning Meeting para este período.

|Sprint #|Sprint 4|
| :- | :- |
|Sprint Planning Background||
|Date|2024-06-15|
|Time|09:40 PM|
|Location|Google Meet|
|Prepared by|Piero Abel Tarazona Medina|
|Attendees (to planning meeting)|Piero Tarazona, Mauricio Chacon, Elias Torres, Moises Donayre, Miguel Huarcaya|
|Sprint 4 – 1 Review Summary|Después de realizar todos los procedimientos establecidos para la identificación de objetivos y áreas de retroalimentación, hemos podido concluir la reunión del sprint 4 con éxito en términos de avance en los productos de software y en la colaboración general del equipo. El proceso de mejora con la retroalimentación y la programación de varias secciones en el servicio web y aplicación web significó un gran proceso de mejora para la construcción y realización del sprint, además de reforzar el compromiso de nuestro equipo y la mejora exponencial de las actividades indicadas.|
|Sprint 4 – 1 Retrospective Summary|Para el proceso de la retrospectiva del Sprint 4, fue necesario que nuestro equipo revisará a detalle toda la retroalimentación recibida ante el primer sprint realizado, para luego generar un análisis a profundidad del desempeño general e individual de todos los miembros del equipo de trabajo. Después de ese proceso, pudimos identificar varias áreas de mejora en las cuales centrarnos para así poder garantizar la entrega de un mejor trabajo y un buen producto para todos nuestros clientes, promoviendo la mejora continua y optimizando los métodos de trabajo en los próximos sprints durante el ciclo de vida del proyecto.|
|Sprint Goal & User Stories||
|Sprint 4 Goal|Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado los objetivos del sprint 4.|
|Sprint 1 Velocity|Con el equipo para este sprint 4 decidimos aceptar 4 Story Points|
|Sum of Story Points|La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 4 es 9|

#### 5.2.4.2 Sprint Backlog 4

El Sprint 4 está centrado en la versión final de nuestro servicio web y aplicación web, priorizando las historias de usuario identificadas. Nuestro objetivo principal es proporcionar a los usuarios una experiencia inicial sólida al presentar una navegación intuitiva y acceso rápido a las funcionalidades relevantes. Al completar las tareas asociadas a las historias de usuario definidas, sentaremos una buena base para el servicio web, asegurando que lo propuesto contribuya al éxito del proyecto.

URL del Board en Trello:

https://trello.com/b/38iyNoXX/appweb-sprintbacklog-4

![trello sprint 4](/assets/chapter05%20-%20sprint%204/trello-sprint-4.png)

|&emsp;&emsp;&emsp;&emsp;<a name="_heading=h.kn5t1eh5nzqr"></a>Sprint #|&emsp;&emsp;&emsp;&emsp;Sprint 4|||||||
| :- | :- | :- | :- | :- | :- | :- | :- |
|&emsp;&emsp;&emsp;&emsp;User Story|&emsp;&emsp;&emsp;&emsp;Work-Item / Task|||||||
|&emsp;&emsp;&emsp;&emsp;Id|&emsp;&emsp;&emsp;&emsp;Title|&emsp;&emsp;&emsp;&emsp;Id|&emsp;&emsp;&emsp;&emsp;Title|&emsp;&emsp;&emsp;&emsp;Descripción|&emsp;&emsp;&emsp;&emsp;Estimation (Hours)|&emsp;&emsp;&emsp;&emsp;Assigned to|&emsp;&emsp;&emsp;&emsp;Status (To-do / In / Process / ToReview / Done)|
|&emsp;&emsp;&emsp;&emsp;US01|&emsp;&emsp;&emsp;&emsp;Visualización de paquetes entregados por un transportista|&emsp;&emsp;&emsp;&emsp;T21|&emsp;&emsp;&emsp;&emsp;Desarrollo de interfaz y lógica para visualización de paquetes entregados|&emsp;&emsp;&emsp;&emsp;Crear una interfaz en la aplicación web que permita al gerente seleccionar un transportista y visualizar el registro de paquetes que ha entregado.|&emsp;&emsp;&emsp;&emsp;4|&emsp;&emsp;&emsp;&emsp;Piero Tarazona|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US04|&emsp;&emsp;&emsp;&emsp;Visualización de envíos asignados|&emsp;&emsp;&emsp;&emsp;T22|&emsp;&emsp;&emsp;&emsp;Implementación de sistema de visualización de envíos asignados|&emsp;&emsp;&emsp;&emsp;Crear una interfaz en la aplicación web donde los transportistas puedan ver los envíos que les han sido asignados, junto con todos los detalles relevantes (destinos, horarios, etc.).|&emsp;&emsp;&emsp;&emsp;5|&emsp;&emsp;&emsp;&emsp;Mauricio Chacon|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US06|&emsp;&emsp;&emsp;&emsp;Visualización de reportes realizados|&emsp;&emsp;&emsp;&emsp;T23|&emsp;&emsp;&emsp;&emsp;Desarrollo de interfaz y lógica para visualización de reportes realizados|&emsp;&emsp;&emsp;&emsp;Crear una sección en la aplicación web donde los transportistas puedan ver un historial de todos los reportes de incidencias que se han realizado.|&emsp;&emsp;&emsp;&emsp;4|&emsp;&emsp;&emsp;&emsp;Miguel Huarcaya|&emsp;&emsp;&emsp;&emsp;Done|
|&emsp;&emsp;&emsp;&emsp;US07|&emsp;&emsp;&emsp;&emsp;Asignación de envíos|&emsp;&emsp;&emsp;&emsp;T24|&emsp;&emsp;&emsp;&emsp;Desarrollo de interfaz y lógica para asignación de envíos|&emsp;&emsp;&emsp;&emsp;Crear una sección en la aplicación web que permita al gerente seleccionar y asignar envíos a los transportistas.|&emsp;&emsp;&emsp;&emsp;5|&emsp;&emsp;&emsp;&emsp;Elias Torres|&emsp;&emsp;&emsp;&emsp;Done|

#### 5.2.4.3 Development Evidence for Sprint Review

Esta sección documenta y presenta la serie de commits realizados en el repositorio de App Web Bicas Team. Estos commits, que son una parte integral del proceso de desarrollo, se han gestionado utilizando la metodología GitFlow y siguiendo estrictamente las convenciones establecidas para los commits. Esta evidencia sirve como un registro transparente y trazable de nuestro progreso y esfuerzos de desarrollo a lo largo del sprint.

![Development Evidence fpr Spóinrt Review](/assets/chapter05%20-%20sprint%204/DevelopmentEvidenceForSprintReview4.png)

|Repository|Branch|Commit Id|Commit Message|Commit Message Body|Committed on (Date)|
| :-: | :-: | :-: | :-: | :-: | :-: |
|upc-AppWeb-BicasTeam-Api|main|cc1ecb8|chore|create default project|18-06|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|3c630b1|chore|implemented persistence base configuration|18-06|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|46d523d|feat|added aggregate user|18-06|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|05ef98f|feat|added user repository|18-06|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|7b06c81|feat|implemented query service and command for user aggregate|18-06|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|431353c|feat|added user controller|18-06|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|554df5b|chore|implemented persistence base configuration|18-06|
|upc-AppWeb-BicasTeam-Api|feature/profile-management|5475552|fix|base configuration|18-06|
|upc-AppWeb-BicasTeam-Api|feature/shipments|cb61040|feat|added layers domain, infrastructure and application|19-06|
|upc-AppWeb-BicasTeam-Api|feature/shipments|b913385|feat|added resources and transform|19-06|
|upc-AppWeb-BicasTeam-Api|feature/shipments|9ee7c1c|feat|added shipment controller|19-06|
|upc-AppWeb-BicasTeam-Api|feature/shipments|8cdc129|chore|implemented interface layer base configuration, including configuration statements in main program|19-08|
|upc-AppWeb-BicasTeam-Api|feature/shipments|132998c|chore|added database context|19-06|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|49269c5|feat|added report aggregate|19-06|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|7c0c3ef|feat|added repositories and services for the model|19-06|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|328d93b|feat|added infrastructure and application for the report|19-06|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|77af4a6|feat|added resources and transform|19-06|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|a0a9813|chore|implemented interface layer base configuration, including configuration statements in main program|19-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|0977fa1|feat|added aggregate vehicle|20-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|0ce3c84|feat|added command and query services|20-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|a6fac64|feat|added resources and transform|20-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|ee78294|feat|added vehicle controller|20-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|3395c27|chore|implemented interface layer base configuration in main program|20-06|

#### 5.2.4.4. Testing Suite Evidence for Sprint Review

En esta sección, presentamos la evidencia de las pruebas realizadas durante el sprint. Hemos utilizado Gherkin para definir los escenarios de prueba y hemos registrado cada prueba en commits específicos en nuestro repositorio. A continuación, se muestra un registro de estos commits:

|Repository|Branch|Commit Id|Commit Message|Commit Message Body|Commited on (Date)|
| :- | :- | :- | :- | :- | :- |
|upc-AppWeb-BicasTeam-Api|feature/profile-management|328d93b|feat|add test for profile management|22-06|
|upc-AppWeb-BicasTeam-Api|feature/shipments|132998c|feat|add test for shipments|22-06|
|upc-AppWeb-BicasTeam-Api|feature/communication-reports|7c0c3ef|feat|add test for communication-reports|22-06|
|upc-AppWeb-BicasTeam-Api|feature/vehicles|e221a5b|feat|add test for vehicles|22-06|

#### 5.2.4.5. Execution Evidence for Sprint Review

El equipo ha logrado desplegar la última versión de la aplicación web y web service de MoviGestion. Todas las historias de usuario asignadas para este sprint fueron completadas exitosamente. En primer lugar, nos enfocamos en el desarrollo y la implementación del web service que es fundamental para la aplicación MoviGestion. Este esfuerzo incluyó la creación de APIs RESTful, la integración segura y eficiente con la base de datos, y la implementación de pruebas exhaustivas para asegurar la fiabilidad y el rendimiento del servicio. 

Capturas de pantalla:

![CAPTURAS DEL WEB SERVICE DESPLEGADO](/assets/chapter05%20-%20sprint%204/executionEvidenceSprint4_0.png)

![CAPTURAS DEL WEB SERVICE DESPLEGADO 2](/assets/chapter05%20-%20sprint%204/executionEvidenceSprint4_1.png)

#### 5.2.4.6. Services Documentation Evidence for Sprint Review

Durante el Sprint 4, el equipo ha trabajado intensamente en la documentación de los Web Services desarrollados. Utilizando OpenAPI, hemos documentado todos los endpoints relevantes, asegurando que cada uno de ellos esté claramente definido y accesible para los desarrolladores. Esta documentación es esencial para garantizar una integración fluida y eficiente del web service con otros componentes de la aplicación y con sistemas externos.

| Endpoint                         | Acción Implementada              | Verbo HTTP | Sintaxis de Llamada              | Parámetros                           | Ejemplo de Response                                                                                       |
|----------------------------------|----------------------------------|------------|----------------------------------|--------------------------------------|------------------------------------------------------------------------------------------------------------|
| /report                          | Crear reporte                    | POST       | /api/v1/report                   | type, description, userId            | {"id": 1, "id-user": "2", "type": "infringement", "description": "Speeding violation, I was going 156km/h", "dateTime": "2024-03-10"} |
| /report/{id}                     | Obtener reporte por Id           | GET        | /api/v1/report/{id}              | id                                   | {"id": 1, "id-user": "2", "type": "infringement", "description": "Speeding violation, I was going 156km/h", "dateTime": "2024-03-10"} |
| /report/user/{userId}            | Obtener reportes por id de usuario | GET        | /api/v1/report/users/{userId}    | userId                               | [{"id": 1, "id-user": "2", "type": "infringement", "description": "Speeding violation, I was going 156km/h", "dateTime": "2024-03-10"}] |
| /report                          | Obtener todos los reportes       | GET        | /api/v1/report                   | none                                 | [{"id": 1, "id-user": "2", "type": "infringement", "description": "Speeding violation, I was going 156km/h", "dateTime": "2024-03-10"}] |
| /vehicle                         | Crear vehículo                   | POST       | /api/v1/vehicle                  | licensePlate, model, serialNumber    | {"id": 1, "licensePlate": "AAA-321", "model": "Chevrolet Corvette", "serialNumber": "IO547SMX"}              |
| /vehicle/{id}                    | Obtener vehículo por Id          | GET        | /api/v1/vehicle/{id}             | id                                   | {"id": 1, "licensePlate": "AAA-321", "model": "Chevrolet Corvette", "serialNumber": "IO547SMX"}              |
| /vehicle                         | Obtener todos los vehículos      | GET        | /api/v1/vehicle                  | none                                 | [{"id": 1, "licensePlate": "AAA-321", "model": "Chevrolet Corvette", "serialNumber": "IO547SMX"}]            |
| /shipment                        | Crear envío                      | POST       | /api/v1/shipment                 | destiny, status, userId, description | {"id": 1, "id-user": "2", "destiny": "Callao, Av Pedro espadaro 2568", "description": "The package to be delivered is a 40-inch smart TV.", "dateTime": "2024-04-25", "status": "Programmed"} |
| /shipment/{id}                   | Obtener envío por Id             | GET        | /api/v1/shipment/{id}            | id                                   | {"id": 1, "id-user": "2", "destiny": "Callao, Av Pedro espadaro 2568", "description": "The package to be delivered is a 40-inch smart TV.", "dateTime": "2024-04-25", "status": "Programmed"} |
| /shipment/user/{userId}          | Obtener envíos por id de usuario | GET        | /api/v1/shipment/users/{userId}  | userId                               | [{"id": 1, "id-user": "2", "destiny": "Callao, Av Pedro espadaro 2568", "description": "The package to be delivered is a 40-inch smart TV.", "dateTime": "2024-04-25", "status": "Programmed"}] |
| /shipment                        | Obtener todos los envíos         | GET        | /api/v1/shipment                 | none                                 | [{"id": 1, "id-user": "2", "destiny": "Callao, Av Pedro espadaro 2568", "description": "The package to be delivered is a 40-inch smart TV.", "dateTime": "2024-04-25", "status": "Programmed"}] |
| /user                            | Crear perfil                     | POST       | /api/v1/user                     | name, lastName, email, type          | {"id": "1", "name": "Peter", "lastName": "Castle", "email": "admin", "password": "admin", "type": "businessman"} |
| /user/{id}                       | Obtener perfil por Id            | GET        | /api/v1/user/{id}                | id                                   | {"id": "1", "name": "Peter", "lastName": "Castle", "email": "admin", "password": "admin", "type": "businessman"} |
| /user                            | Obtener todos los perfiles       | GET        | /api/v1/user                     | none                                 | [{"id": "1", "name": "Peter", "lastName": "Castle", "email": "admin", "password": "admin", "type": "businessman"}] |

Capturas de Interaccion con la Documentacion

A continuación, se incluyen capturas de pantalla que muestran la interacción con la documentación de los web services, utilizando datos de muestra.

1. Endpoint de Crear Reporte (/report) - POST:

![1](/assets/chapter05%20-%20sprint%204/post-rep1.png)

![1](/assets/chapter05%20-%20sprint%204/post-rep2.png)

Descripción: La captura muestra la documentación del endpoint para crear un nuevo reporte, incluyendo los parámetros requeridos y un ejemplo del response.

2. Endpoint de Obtener Reporte por ID (/report/{id}) - GET

![2](/assets/chapter05%20-%20sprint%204/get-rep1.png)

![2](/assets/chapter05%20-%20sprint%204/get-rep2.png)

Descripción: La captura presenta la documentación del endpoint para obtener un reporte por ID, con la sintaxis de llamada y un ejemplo de response.

3. Endpoint de Crear Vehículo (/vehicle) - POST:

![3](/assets/chapter05%20-%20sprint%204/post-ve1.png)

![3](/assets/chapter05%20-%20sprint%204/post-ve2.png)

Descripción: La imagen muestra cómo documentamos la creación de un nuevo vehículo, especificando los parámetros y un ejemplo del response.

4. Endpoint de Obtener Envío por ID (/shipment/{id}) - GET:

![4](/assets/chapter05%20-%20sprint%204/get-ship1.png)

![4](/assets/chapter05%20-%20sprint%204/get-ship2.png)

Descripción: La captura ilustra la documentación del endpoint para obtener un envío por ID, incluyendo un ejemplo del request y response.

#### <a name="_heading=h.ikcf394glpjk"></a>**URL del Repositorio:**
   El código fuente del Web Services se encuentran en el siguiente repositorio:

- **Repositorio de Web Service:** [upc-AppWeb-BicasTeam/upc-AppWeb-BicasTeam-Api: Bicas Team - Movigestion - API (github.com)](https://github.com/upc-AppWeb-BicasTeam/upc-AppWeb-BicasTeam-Api) 

#### 5.2.4.7. Software Deployment Evidence for Sprint Review

Durante el Sprint 4, llevamos a cabo el despliegue de nuestra web service en SmarterASP.NET. A continuación, detallamos los pasos realizados:

- Ingesamos la cuenta de SmarterASP.NET

![1](/assets/chapter05%20-%20sprint%204/softwareDeployment1.png)

- Creamos nuestra cuenta de hosting con el plan gratuito de 60 dias

![2](/assets/chapter05%20-%20sprint%204/softwareDeployment2.png)

- Entramos al panel de control de nuestro hosting creado

![3](/assets/chapter05%20-%20sprint%204/softwareDeployment3.png)

- En la sección Databases elegimos MySQL

![4](/assets/chapter05%20-%20sprint%204/softwareDeployment4.png)

- Creamos nuestra base de datos para nuestro web service

![5](/assets/chapter05%20-%20sprint%204/softwareDeployment5.png)

- En Files subiremos el publish de nuestro web service

![6](/assets/chapter05%20-%20sprint%204/softwareDeployment6.png)

- Volvemos a WebSite y le damos click en site1

![7](/assets/chapter05%20-%20sprint%204/softwareDeployment7.png)

- Finalmente, comprobamos de que se realizó el deploy correstamente

![8](/assets/chapter05%20-%20sprint%204/softwareDeployment8.png)

#### 5.2.4.8. Team Collaboration Insights during Sprint

Durante este cuarto Sprint, hemos avanzado el desarrollo del web service y hemos colaborado estrechamente en su implementación. La colaboración entre los miembros del equipo se refleja en los diversos commits realizados en el repositorio de GitHub, los cuales han sido debidamente documentados en las capturas de pantalla adjuntas. Para asegurar una colaboración efectiva, hemos implementado GitFlow como nuestra metodología de trabajo colaborativo en Git. Con GitFlow, hemos creado ramas para cada una de las secciones de nuestro web service. Esto nos ha permitido trabajar de manera organizada y centrarnos en completar correctamente las historias de usuario designadas para cada sección. En cuanto a la elaboración del código, hemos asignado a cada miembro del equipo una sección específica del web service. Esta estrategia nos ha permitido avanzar de manera más eficiente y completar el trabajo antes de la fecha de entrega. Además, hemos realizado reuniones adicionales para intercambiar ideas y resolver cualquier duda o problema que pudiera surgir durante el desarrollo del web service. Estas sesiones han contribuido de manera positiva al éxito del proyecto. A continuación, presentamos algunas capturas de pantalla que muestran los commits realizados por los miembros del equipo en GitHub:

![Team Collaboration Insights during Sprint](/assets/chapter05%20-%20sprint%204/teamCollaboration.png)

## 5.3 Validation Interviews
Con el fin de obtener y separar correctamente toda la información obtenida durante las entrevistas, se optó por definir un banco de preguntas según nuestro segmento de mercado identificado anteriormente. Este grupo de preguntas está especializado para la obtención de información específica según la persona entrevistada y según la problemática investigada para el proyecto y la posible solución en la forma de nuestro producto. 

### 5.3.1 Diseño de Entrevsitas
**Para los Empresarios:**

- ¿Cuál es su opinión general sobre la plataforma MoviGestion tras la demostración?
- ¿Qué características de MoviGestion le resultaron más útiles para la gestión de su flota?
- ¿Hay alguna función que no encontró en MoviGestion y que consideraría esencial para su operación?
- ¿Cómo evalúa la interfaz de usuario en términos de facilidad de uso y navegación?
- ¿Cuánto tiempo cree que le tomaría a su equipo adaptarse al uso de MoviGestion?
- ¿Cuáles son los principales desafíos que enfrenta actualmente en la gestión de su flota?
- ¿Cómo cree que MoviGestion podría ayudarle a superar esos desafíos?
- ¿Qué tan útil considera la funcionalidad de registro de incidencias en la plataforma?
- ¿Qué aspectos de la gestión de envíos exitosos le parecen más críticos para su operación?
- ¿Está dispuesto a recomendar MoviGestion a otros empresarios del sector? ¿Por qué?
- ¿Cómo valora la seguridad de la información y los datos en la plataforma MoviGestion?

**Para los Transportistas:**

- ¿Cuál fue su impresión general de la plataforma MoviGestion después de la demostración?
- ¿Qué tan fácil le resultó navegar y utilizar las funciones de MoviGestion?
- ¿Qué características de MoviGestion le parecieron más útiles para su trabajo diario?
- ¿Hay alguna función que no encontró en MoviGestion y que consideraría útil para su labor?
- ¿Cómo cree que MoviGestion podría ayudarle a realizar su trabajo de manera más eficiente?
- ¿Qué tan útil considera la funcionalidad de registro de incidencias para reportar problemas en tiempo real?
- ¿Qué tan fácil le resultó el proceso de seguimiento de envíos en MoviGestion?
- ¿Cómo valora la capacidad de monitorear los sitios de entrega a través de la plataforma?
- ¿Le parece intuitiva la interfaz de usuario de MoviGestion? ¿Hay algo que cambiaría?
- ¿Cómo le gustaría que MoviGestion le notificara sobre nuevas tareas o cambios en las entregas?
- ¿Qué mejoras le gustaría ver en futuras actualizaciones de la plataforma?
- ¿Cómo valora la seguridad de la información y los datos en la plataforma MoviGestion?
- ¿Cree que MoviGestion le ayudaría a reducir el tiempo de inactividad y aumentar la productividad?
- ¿Estaría dispuesto a recomendar MoviGestion a otros transportistas? ¿Por qué?

### 5.3.2 Registro de Entrevistas
1. ### <a name="_heading=h.mqpm42spx03x"></a>***Segmento objetivo: Empresarios***
   **Entrevista N°1:**

   
![Entrevsita 1](/assets/chapter05%20-%20review/entrevista3.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Abraham Quenta
- **Edad:** 28 años
- **Distrito:** Tacna
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de la entrevista:** 0:00
- **Duración:** 10:45
- **Resumen:** Abraham se presenta como un profesional del transporte con 5 años de experiencia en el sector transporte provincial, cuya ruta principal es de Tacna a Puno. Comenta sobre la página de destino de su servicio, que incluye información sobre los servicios ofrecidos y permite la personalización del idioma. Abraham explora las características y funcionalidades del sitio web, como la gestión de la flota, los informes de los conductores y la gestión de vehículos, y aprecia el aspecto organizativo de la plataforma, señalando que es fácil encontrar las funciones deseadas. Abraham menciona algunos problemas menores con la visibilidad del texto y la navegación, pero en general considera que la interfaz de usuario es clara y sencilla. información del vehículo, así como las estrategias de marketing y el diseño de la página de destino, pero en general. considera que la aplicación es valiosa, especialmente para monitorear las actividades de los conductores.

**Entrevista N°2:**

![Entrevista 2](/assets/chapter05%20-%20review/entrevista1.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Gustavo Manrique
- **Edad:** 40 años
- **Distrito: Chorrillos**
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de la entrevista:** 10:46
- **Duración:** 6:40
- **Resumen:** El empresario Gustavo Manrique expresó una opinión muy bien sobre MoviGestion, destacando la utilidad de las estadísticas de rendimiento y el seguimiento de envíos exitosos. Considera que la plataforma es fácil de usar y que su equipo podría adaptarse rápidamente. También, identificó como desafíos principales el seguimiento de envíos, gestión de incidencias y optimización de rutas, áreas donde cree que MoviGestion puede ayudar significativamente. Mencionó la necesidad de una herramienta para la optimización de rutas en tiempo real. Valora altamente la seguridad de la información y está dispuesto a recomendar la plataforma a otros empresarios del sector.


**Entrevista N°3:**

![Entrevsita3](/assets/chapter05%20-%20review/entrevista2.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Marco Tarazona
- **Edad:** 57 años
- **Distrito:** Puente Piedra
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de la entrevista:** 17:34
- **Duración:** 2:17
- **Resumen:** El empresario Marco Tarazona expresó una opinión positiva sobre MoviGestion, resaltando su utilidad para la gestión de flotas, especialmente en el seguimiento de envíos y la gestión de incidencias. Mencionó la facilidad de uso de la plataforma y consideró que su equipo podría adaptarse rápidamente. Identificó como posible desafio la optimización de rutas y la necesidad de integración con otros sistemas. Además, valora la seguridad de la información y está dispuesto a recomendar MoviGestion a otros empresarios del sector.



**Segmento objetivo: Transportistas**

**Entrevista N°1:**

![Entrevsita 4](/assets/chapter05%20-%20review/Entrevista1reviw.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Renzo Cesar Silva Morales
- **Edad:** 24 años
- **Distrito:** Santiago de Surco
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de entrevista:** 19:43
- **Duración:** 7:50
- **Resumen:** Renzo es un transportista que recién está comenzando en el negocio, tuvo una experiencia inicial positiva con la plataforma. En donde destaca las secciones que tenemos implementadas por su funcionalidad. La interfaz le pareció amigable y fácil de usar, pero encontró algunas dificultades técnicas. Considera que sería beneficioso añadir seguimiento en tiempo real para envíos, notificaciones automáticas y soporte por chat en vivo. Aunque las opciones actuales son útiles, a él le gustaría tener más información detallada en cada apartado. Por último, sugiere la inclusión de tutoriales interactivos para que los nuevos usuarios puedan familiarizarse.

**Entrevista N°2:**

![Entrevsita 5](/assets/chapter05%20-%20review/entrevista5.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Ricardo Chate Flores
- **Edad:** 45 años
- **Distrito:** Cercado de Lima
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de entrevista:** 28:01
- **Duración:** 8:00
- **Resumen:** El transportista Ricardo Chate Flores expresó una opinión positiva sobre MoviGestion, destacando su facilidad de uso y navegación intuitiva. Consideró útiles las funciones de registro de incidencias y seguimiento de envíos para su trabajo diario. Valora la capacidad de monitorear los sitios de entrega y mencionó que la plataforma podría ayudarle a trabajar de manera más eficiente. Aunque satisfecho con las funcionalidades actuales, sugirió la necesidad de notificaciones más personalizables. José destacó la seguridad de la información y está dispuesto a recomendar MoviGestion a otros transportistas, ya que cree que puede reducir el tiempo de inactividad y aumentar la productividad.

**Entrevista N°3:**

![Entrevsita 6](/assets/chapter05%20-%20review/entrevista6.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Víctor Cuba Bautista
- **Edad:** 42 años
- **Distrito:** Villa El Salvador
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de entrevista:** 35:37
- **Duración:** 4:50
- **Resumen:** El transportista Víctor Cuba Bautista tras probar la plataforma, reconoció que el uso de las funciones eran más sencillos de lo que esperaba. Encontró especialmente útil el registro de incidencias en tiempo real. Aunque le gustaría ver mejoras en algunas funcionalidades adicionales, valora la capacidad de monitorear los sitios de entrega y la seguridad de los datos proporcionada por la plataforma. Al final, Víctor concluyó que MoviGestion es una herramienta efectiva que puede mejorar su eficiencia y reducir el tiempo de inactividad, y estaría dispuesto a recomendarla a otros transportistas.



### 5.3.3 Evaluaciones segun heuristicas
Esta sección contiene el proceso de evaluación de las sesiones de validación basado en heurísticas, considerando heurísticas de usabilidad, arquitectura de información e inclusive design de la experiencia propuesta. Para esto la sección usamos la estructura del formato para evaluaciones de heurísticas indicado.


**UX Heuristics & Principles Evaluation**

**Usability – Inclusive Design – Information Architecture**
\***


**CARRERA                	: Ingeniería de Software**

**CURSO                    	: Aplicaciones Web**

**SECCIÓN                   	: SV51**

**PROFESORES         	: Angel Augusto Velasquez Nuñez**

**AUDITOR                 	: Bicas Team**

**CLIENTE                  	: MoviGestion**
1. ## <a name="_heading=h.3ibjgvegxoc5"></a>** 
   **SITE o APP A EVALUAR:**

   **MoviGestion**

   **TAREAS A EVALUAR:**

   *El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:*

*1.* 	*Gestión y edición de perfil de usuario.*

*2.     Visualización de asignación de envíos que pertenecen a cada transportista*

*3. 	Agregar un nuevo vehículo a la flota de vehículos.*

*4. 	Eliminar un vehículo de la flota de vehículos.*

*5. 	Visualización de alertas de cada transportista.*

**ESCALA DE SEVERIDAD:**

*Los errores serán puntuados tomando en cuenta la siguiente escala de severidad*

|***Nivel***|***Descripción***|
| :- | :- |
|*1*|*Problema superficial: puede ser fácilmente superado o hasta ignorado por el usuario ó ocurre con muy poca frecuencia. El error no necesita ser arreglado de forma inmediata en la mayoría de las casos, a no ser que exista disponibilidad de tiempo.*|
|*2*|*Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de superar para el usuario. Se le debería asignar una prioridad baja para resolverlo de cara antes de la siguiente entrega o actualización.*|
|*3*|*Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlos. Es importante que sean corregidos y se les debe asignar una prioridad alta.*|
|*4*|*Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento.*|


**TABLA RESUMEN:**

|*#*|*Problema*|*Escala de severidad*|*Heurística/Principio violada(o)*|
| :-: | :-: | :-: | :-: |
|*1*|*Incluye un botón “See More” pero no tiene funcionalidad*|*3*|*Information Architecture: Is it usable?*|
|*2*|*No parece haber consistencia en la forma en que se presentan las opciones para actualizar la información*|*2*|*Usability: Consistencia y estándares*|
|*3*|*Información de pagos no está claramente presentada*|*3*|*Usability: Visibilidad del estado del sistema*|
|*4*|*No funciona cancelar el agregado de un vehículo.*|*2*|*Usability: Libertad y control del usuario*|





**DESCRIPCIÓN DE PROBLEMAS:**

*PROBLEMA #1:* 

*Severidad: 3*

*Heurística violada: Information Architecture: Is it usable?*

*Problema:*

*La aplicación incluye un botón “See More” pero no tiene funcionalidad, lo que confunde a los usuarios y les impide acceder a contenido adicional esperado.*

![H1](/assets/chapter05%20-%20heuristc%20and%20final/h1.png)

*Recomendación:*

*Eliminar el botón “See More” si no hay contenido adicional disponible, o implementar la funcionalidad esperada para que los usuarios puedan acceder a más información.*

*PROBLEMA #2:* 

*Severidad: 2*

*Heurística violada: Usability - Consistencia y estándares*

*Problema:*

*La interfaz de Settings incluye campos para Nickname, Bio, Email y Avatar, pero no parece haber consistencia en la forma en que se presentan las opciones para actualizar la información. Por ejemplo, el botón ‘Choose’ para actualizar el avatar está separado del campo ‘Avatar’, lo que podría confundir a los usuarios.*

![H2](/assets/chapter05%20-%20heuristc%20and%20final/h2.png)

*Recomendación:*

*Asegurar que todos los campos de entrada y botones relacionados estén agrupados de manera coherente y clara para mejorar la comprensión y la facilidad de uso.*

*PROBLEMA #3:* 

*Severidad: 3*

*Heurística violada: Usability: Visibilidad del estado del sistema*

*Problema:*

*La información relacionada con Organization no está claramente presentada, lo que puede causar confusión a la hora de querer tener información y dificulta la asignación de envíos.*

![H3](/assets/chapter05%20-%20heuristc%20and%20final/h3.png)

*Recomendación:*

*Mejorar la presentación y accesibilidad de la información relacionada con "Organization" puede mejorar significativamente la experiencia del usuario y facilitar la asignación de envíos en la aplicación.* 

*PROBLEMA #4:* 

*Severidad: 2*

*Heurística violada: Usability: Libertad y control del usuario*

*Problema:*

*Al momento de ingresar los datos del nuevo vehículo, no se puede cerrar hasta darle darle al botón “Close” y luego se tiene que eliminar en el botón “Delete Vehicle”, esto obliga a agregar nuevos carros no deseados, también incrementando así la cantidad de esfuerzo del usuario.*

![H4](/assets/chapter05%20-%20heuristc%20and%20final/h4.png)

*Recomendación:*

*Hacer que el botón "Close" tenga la funcionalidad para cerrar la ventana emergente sin guardar los datos del vehículo ingresados.*

---

## 5.4 Video About The Product

En esta sección elaboramos un resumen de los aspectos más relevantes del video About-The-Product.

**Título**: About the Product Movigestion

**Duración**: 2:08

**Objetivo**: Presentar el producto Movigestion y sus funcionalidades

**Pautas de secuencias de contenidos**


|Sección|Inicio(hh:mm)|Resumen|
|-------|-------------|-------|
|Introducción del presentador|00:01|Se presenta y menciona que va a hablar sobre el producto desarrollado, Movigestión.|
|Descripción general del producto|00:06|Movigestión está diseñado para ayudar a empresarios con flotas de vehículos a administrar eficientemente.|
|Funcionalidades de la aplicación|00:11|La aplicación permite a administradores y transportistas gestionar envíos y reportes de sus vehículos.|
|Pantalla de inicio y login|00:21|Descripción de la pantalla de login y las opciones para registrarse como administrador o transportista.|
|Funcionalidades para administradores|00:59|Los administradores pueden ver envíos programados, reportes generados por empleados y gestionar vehículos.|
|Funcionalidades para transportistas|01:30|Los transportistas pueden ver envíos asignados, reportes, agregar reportes y ver los vehículos asignados.|
|Conclusión|01:55|Resumen final de las capacidades de Movigestión, enfatizando en la gestión y organización de vehículos y reportes.|

![About The Product](/assets/chapter05%20-%20review/about%20the%20product.PNG)


Microsoft Stream URL: <https://upcedupe-my.sharepoint.com/:v:/g/personal/u202116207_upc_edu_pe/EVzNfjl7ZRtAvgrVtGxeeSEB24lFo7SCNzRMpCjNjY7bRg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=sBmRa5>

Youtube URL: https://www.youtube.com/About The Product MoviGestion 
