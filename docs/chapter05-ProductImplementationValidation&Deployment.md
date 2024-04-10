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

A continuación, detallaremos nuestra estrategia para ejecutar la implementación, pruebas y lanzamiento de nuestro landing page, así como de los servicios web y la interfaz de usuario de la aplicación web en cada iteración de desarrollo. En relación al Sprint 1, nos concentraremos exclusivamente en explicar el procedimiento de implementación del landing page.

### 5.2.1 Sprint n
### 5.2.1.1 Sprint Planning n

El objetivo primordial de esta reunión es crear un plan claro y alcanzable para el sprint, identificando las tareas necesarias y comprometiéndose con un conjunto definido de resultados concretos que impulsen el progreso del proyecto. A continuación, se presenta un resumen del Encuentro de Planificación del Sprint, que ofrecerá una visión general de los temas discutidos y las decisiones tomadas durante la reunión.

| Sprint #                             | Sprint 1           |
|--------------------------------------|--------------------|
| Sprint Planning Background                                |
| Date                                 |  2024-03-23        |
| Time                                 |  01:30 PM          |
| Location                             |  Discord           |
| Prepared By                          |  Piero Tarazona    |
| Attendees (to planning meeting)      |  Piero Tarazona, Mauricio Chacon, Elias, Moises Donayre, Miguel |
| Sprint 1 – 1 Review Summary          |  El primer sprint resultó exitoso en cuanto al progreso del producto de software y la colaboración eficiente del equipo. Los hitos alcanzados y la retroalimentación recopilada durante esta evaluación establecen una base sólida para el próximo sprint y demuestran el compromiso del equipo.  |
| Sprint 1 – 1 Retrospective Summary   |  La retrospectiva del primer sprint nos permitió analizar el rendimiento del equipo y detectar áreas que requieren mejoras. Este análisis nos servirá como punto de partida para promover la mejora continua y optimizar la colaboración del equipo en los siguientes sprints.  |
| Sprint Goal & User Stories                                |
| Sprint 1 Goal                        | Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado los objetivos del sprint 1.        |
| Sprint 1 Velocity                    | Con el equipo para este sprint 1 decidimos aceptar 4 Story Points      |
| Sum of Story Points                  | La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 1 es 28 |

### 5.2.1.2 Sprint Backlog n

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
            <td>US13</td>
            <td>Landing - Navegacion</td>
            <td>T01</td>
            <td>Implementar menú de navegación en la página de inicio</td>
            <td>Desarrollar un menú de navegación para la página de inicio, permitiendo a los visitantes acceder fácilmente a secciones relevantes. Esto incluye diseño, identificación de secciones clave y garantía de funcionalidad en diferentes dispositivos, mejorando así la experiencia del usuario.</td>
            <td>40 minutos</td>
            <td>Mauricio</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US14</td>
            <td>Landing - Dirigir a aplicacion web</td>
            <td>T02</td>
            <td> Integración del Enlace Directo a la Aplicación Web Principal</td>
            <td>Integrar un enlace directo en la página de inicio para permitir a los visitantes acceder fácilmente a la aplicación web principal, agilizando así su experiencia de navegación.</td>
            <td>1 hora</td>
            <td>Moises</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US15</td>
            <td>Landing - Encabezado</td>
            <td>T03</td>
            <td>Diseño del Encabezado Informativo</td>
            <td>Crear un encabezado en la página de inicio para ofrecer información breve sobre los servicios, precios y contacto, facilitando la comprensión de los visitantes sobre lo que ofrece el sitio.</td>
            <td>1 hora</td>
            <td>Miguel</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US16</td>
            <td>Landing - contactoFooter</td>
            <td>T04</td>
            <td>Diseño del Footer de Contacto</td>
            <td>Integrar un footer en la página de inicio con enlaces a redes sociales, barra de navegación adicional y detalles de contacto de la empresa para una experiencia de usuario completa.</td>
            <td>1 hora</td>
            <td>Piero</td>
            <td>Done</td>
        </tr>
    </table>

### 5.2.1.3 Development Evidence for Sprint Review.

| Repository                        | Branch              | Commit Id                          | Commit Message                   | Commit Message Body           |Commited on (Date) |
|-----------------------------------|---------------------|------------------------------------|----------------------------------|-------------------------------|-------------------|
| REPOSITORIO DEL LANDING(NOMBRE)   | feature/loremipsum  | 14ca4e3                            | feat: ...                        | MENSAJE DEL COMMIT            | FECHA DEL COMMIT  |

### 5.2.1.4 Testing Suite Evidence for Sprint Review. 

| Repository                        | Branch              | Commit Id                          | Commit Message                   | Commit Message Body           |Commited on (Date) |
|-----------------------------------|---------------------|------------------------------------|----------------------------------|-------------------------------|-------------------|
| REPOSITORIO DEL LANDING(NOMBRE)   | feature/loremipsum  | 14ca4e3                            | feat: ...                        | MENSAJE DEL COMMIT            | FECHA DEL COMMIT  |

### 5.2.1.5 Execution Evidence for Sprint Review. 

En esta sección, detallaremos los hitos alcanzados durante el Sprint 1:

- Establecimiento de repositorios en GitHub para el reporte y el landing page.
- Creación de wireframes y mock-ups para el landing page.
- Elaboración de wireframes y mock-ups para la aplicación web.
- Implementación exitosa del landing page.
- Diseño del prototipo de la aplicación web.
- Publicación del landing page en GitHub Pages.

### 5.2.1.6 Services Documentation Evidence for Sprint Review. 

Durante este Sprint 1, nos enfocamos en desarrollar el landing page, sin implementación de cualquier servicio. Por lo tanto, este punto quedará sin actividad en este aspecto.

### 5.2.1.7 Software Deployment Evidence for Sprint Review.

Describiremos las acciones llevadas a cabo durante el sprint 1, incluyendo la preparación y despliegue de nuestro landing page:

- En primer lugar, creamos un repositorio en GitHub dedicado al landing page.
- Posteriormente, creamos las ramas necesarias siguiendo el flujo de trabajo de GitFlow.
- Luego, accedimos a la sección "Pages" en la configuración del repositorio.
- Ajustamos la configuración para especificar la fuente del landing page.
- Después de guardar los cambios en la configuración, se generó un enlace para acceder al landing page.
- Este enlace nos permite visualizar las actualizaciones realizadas en la rama "develop".

### 5.2.1.8 Team Collaboration Insights during Sprint.

Para este primer Sprint, hemos completado el desarrollo del landing page y colaborado estrechamente en su implementación. La colaboración entre los miembros del equipo se refleja en los diversos commits realizados en el repositorio, los cuales han sido debidamente documentados en las capturas de pantalla adjuntas.

En cuanto a la colaboración del equipo, hemos llevado a cabo reuniones tanto presenciales como virtuales para asignar tareas y discutir la estrategia de desarrollo del proyecto. Esta práctica nos ha permitido comprender claramente nuestras responsabilidades individuales y mejorar nuestro rendimiento. Para la elaboración del código, hemos adoptado la decisión de asignar a cada miembro del equipo una sección específica del landing page, con el objetivo de avanzar de manera más eficiente y completar el trabajo antes de la fecha de entrega.

Por último, hemos realizado reuniones adicionales para intercambiar ideas y resolver cualquier duda o problema que pudiera surgir durante el desarrollo del landing page. Estas sesiones han contribuido de manera positiva al éxito del proyecto.
