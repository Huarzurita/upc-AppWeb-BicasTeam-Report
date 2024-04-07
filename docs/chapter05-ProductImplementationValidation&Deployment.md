# Capítulo 5: Product Implementation, Validation & Deployment

## 5.1 Software Configuration Management.

Para administrar la configuración de software de nuestra app, nos centraremos en tres aspectos principales: el control del código fuente, que implica gestionar las versiones y establecer una estructura organizada para el código; la configuración del entorno de desarrollo, donde nos aseguramos de que todos los miembros del equipo cuenten con herramientas consistentes; y la configuración de implementación, que se ocupa del despliegue en entornos de producción. Estas decisiones garantizan la coherencia y eficacia a lo largo de todo el ciclo de vida de la aplicación.

### 5.1.1 Software Development Environment Configuration

En esta sección, detallaremos y explicaremos los productos utilizados en el proyecto digital, así como su propósito y cómo se accede a cada uno de ellos.

* Project Management:
Para las reuniones de equipo, se emplearon herramientas como Google Meet y Discord. Asimismo, para gestionar las versiones, se estableció un repositorio colaborativo en GitHub, lo que permitió mantener y modificar el proyecto de forma eficiente mediante commits.

* Diseño UX/UI del Producto:
En la elaboración de los escenarios As-Is y To-Be, así como en el segmetno objetivo y impact mappin, se hizo uso de la plataforma Miro. Respecto a los wireframes, maquetas y prototipos de la aplicación web, se optó por Figma.

* Desarrollo de Software:
Para la creación de la página de inicio, se utilizaron las siguientes herramientas:

Visual Studio Code: Un editor de código optimizado para desarrollar y depurar aplicaciones web y en la nube de manera eficaz.

HTML: Un lenguaje utilizado para la creación de la página de inicio.

CSS: Un lenguaje empleado para dar estilo y mejorar la presentación de los contenidos.

JavaScript: Un lenguaje de programación utilizado por los desarrolladores para hacer las páginas web más interactivas.

Git: Un sistema de control de versiones distribuido que permite la colaboración del equipo en el proyecto.

* Software Testing:
Dado que empleamos Visual Studio Code como editor de código, tendremos acceso a la extensión Live Server, la cual nos permite configurar un servidor local para visualizar instantáneamente las modificaciones realizadas en un navegador web como Microsoft Edge o Chrome. Además, para llevar a cabo pruebas de aceptación, utilizaremos Gherkin y luego cargaremos los resultados en el repositorio.

* Software Deployment:
Optaremos por utilizar Github Pages para alojar nuestra página de inicio, dado que se trata de una página estática que no requiere cambios frecuentes. Esta elección es beneficiosa ya que Github Pages permite actualizar el contenido de forma gratuita.

* Software Document:
En lo que respecta a la documentación del software, emplearemos HTML para crear nuestra página de inicio. Esta página servirá como una fuente de información detallada sobre el software que estamos desarrollando.

### 5.1.2 Source Code Management.

En esta sección, detallaremos la implementación de GitFlow, un flujo de trabajo para el control de versiones que define diferentes ramas además de la rama principal (main), como la rama de desarrollo (develop). Para GitFlow, cada nueva característica requiere su propia rama, por lo que describiremos las convenciones utilizadas para nombrar estas ramas de características.

| *Main: *Esta rama contendrá la versión estable del proyecto, lista para su despliegue.  |
|-----------------------------------------------------------------------------------------|

Develop: En esta rama se agrupan todos los elementos en proceso de desarrollo. Una vez que el trabajo en una funcionalidad está completo y se considera listo para avanzar, se fusionará con la rama de lanzamiento (release).

Feature: Cada miembro del equipo trabajará en su propia rama individual, donde subirá el código asignado para una función específica. Estas ramas de características se integrarán con la rama "develop".

En cuanto a la convención para nombrar las ramas de características, seguiremos el formato siguiente:

| feature_<nombre -integrante>/<breve-descripción>    |
|-----------------------------------------------------|

Para etiquetar las versiones de lanzamiento, adoptaremos el versionado semántico 2.0.0, que sigue la estructura:

| Mayor.Menor.Parche. |
|---------------------|

El último dígito (Parche) se refiere principalmente a correcciones de errores compatibles con versiones anteriores. El segundo dígito (Menor) aumenta cuando se agregan características compatibles con la versión anterior. El primer dígito (Mayor) se incrementa para cambios significativos que podrían no ser compatibles con la versión anterior.

Finalmente, implementaremos el uso de Conventional Commits para los mensajes de texto en cada commit. Estos mensajes seguirán la estructura:

| type: description |
|-------------------|

### 5.1.3 Source Code Style Guide & Conventions.

Nuestro objetivo es adherirnos a las normativas y pautas de codificación establecidas, provenientes de diversas fuentes como el HTML Style Guide and Coding Conventions, la Guía de Estilo de Codificación para JavaScript y las Convenciones Gherkin para Especificaciones Legibles.

**CONVENCIONES A SEGUIR**

**HTML*:

- Es crucial emplear nombres descriptivos para los archivos HTML.
- Se recomienda seguir una convención de nomenclatura consistente, como camelCase, para nombres de archivos y carpetas.
- Se debe utilizar los elementos HTML de manera semántica para una correcta descripción del contenido del sitio web, incluyendo el uso adecuado de etiquetas.
- Mantener una estructura de código clara y legible mediante una adecuada indentación.
- Se insta a utilizar un estilo de formato uniforme en todo el código para mejorar su mantenibilidad.

**CSS*:

- Se aconseja utilizar nombres de clases descriptivos y significativos para aplicar estilos a los elementos HTML.
- Se debe preferir nombres que reflejen la función o propósito del elemento en lugar de su apariencia.
- Evitar el uso de IDs para estilos, ya que puede resultar en especificidad excesiva y dificultar la reutilización de estilos.

**JavaScript*:

- Se seguirá la convención de camelCase para nombres de variables y funciones en JavaScript.
- Es importante utilizar espacios o tabulaciones de manera consistente, y asegurarse de mantener una línea de código por línea para mejorar la legibilidad.

**Gherkin*:

- Se recomienda utilizar las palabras clave de Gherkin como Given, When, Then para estructurar los escenarios de forma coherente y expresiva.

### 5.1.4 Software Deployment Configuration.

En esta sección, abordaremos la configuración del despliegue de nuestra solución, detallando los pasos necesarios para llevar el Landing Page desde los repositorios de código fuente hasta su implementación final.

Para comenzar, crearemos un repositorio en GitHub destinado a almacenar los archivos HTML, CSS y JavaScript pertinentes. Cada miembro del equipo trabajará en su propia rama "feature" para desarrollar componentes específicos del landing page. Una vez que se completa una característica, se fusionará con la rama "develop" para mantener actualizada la versión del landing page. Posteriormente, configuraremos GitHub Pages para publicar la página de destino, utilizando la rama "develop".

A continuación, detallamos los pasos necesarios para este despliegue en GitHub Pages:

- Creación de un repositorio público en GitHub y asignación de un nombre apropiado.
- Configuración de las ramas necesarias siguiendo el flujo de trabajo estándar de Gitflow, que incluye main, release, develop, features y hotfix.
- Acceso a la sección de ajustes del repositorio y selección de la pestaña Pages.
- Navegación hacia la sección de configuración para GitHub Pages.
- Seleccionar la rama "develop" como la rama de despliegue del landing page, manteniendo las demás configuraciones con sus valores predeterminados.
- Al seleccionar la rama correspondiente, se generará un enlace que proporcionará acceso al landing page. Cada modificación realizada en la rama "develop" se reflejará automáticamente en este enlace.
- Cada miembro del equipo trabajará en sus propias ramas de características.
- Se realizarán fusiones entre la rama "develop" y las ramas de características para integrar los avances.
- Se observarán los cambios reflejados en el enlace proporcionado por GitHub Pages.
- Finalmente, el landing page estará desplegado y listo para ser visualizado y utilizado.

## 5.2 Landing Page, Services & Applications Implementation.

A continuación, detallaremos nuestra estrategia para ejecutar la implementación, pruebas y lanzamiento de nuestro landing page, así como de los servicios web y la interfaz de usuario de la aplicación web en cada iteración de desarrollo. En relación al Sprint 1, nos concentraremos exclusivamente en explicar el procedimiento de implementación del landing page.

### 5.2.1 Sprint 1
### 5.2.1.1 Sprint Planning 1

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

### 5.2.1.2 Sprint Backlog 1

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
            <td>US01</td>
            <td>Titulo</td>
            <td>T01</td>
            <td>Titulo</td>
            <td>Decripcion</td>
            <td>40 minutos</td>
            <td>Mauricio</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US02</td>
            <td>Titulo</td>
            <td>T02</td>
            <td>Titulo</td>
            <td>Decripcion</td>
            <td>1 hora</td>
            <td>Moises</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US03</td>
            <td>Titulo</td>
            <td>T03</td>
            <td>Titulo</td>
            <td>Decripcion</td>
            <td>1 hora</td>
            <td>Miguel</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US04</td>
            <td>Titulo</td>
            <td>T04</td>
            <td>Titulo</td>
            <td>Decripcion</td>
            <td>1 hora</td>
            <td>Piero</td>
            <td>Done</td>
        </tr>
        <tr>
            <td>US05</td>
            <td>Titulo</td>
            <td>T05</td>
            <td>Titulo</td>
            <td>Decripcion</td>
            <td>50 minutos</td>
            <td>Elias</td>
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
