# Capítulo 3: Requirements Specification
## 3.1 To-Be Scenario Mapping

CONDUCTOR:

![To-Be Conductor](/assets/chapter03/to-be%20transportistas.png)

EMPRESARIO:

![To-Be Empresario](/assets/chapter03/to-be%20empresarios.png)

## 3.2 User Stories
### 3.2.1 User Stories Web Aplication
<table>
    <tr>
        <th>Epic ID</th>
        <th>Descripcion</th>
        <th>User Story ID</th>
        <th>Descripcion</th>
        <th>Criterios de Aceptacion</th>
    </tr>
    <tr>
        <td rowspan="2">EP01</td>
        <td rowspan="2">Gestión de Rutas: Permitir al gerente asignar rutas específicas a los transportistas, asegurando una distribución eficiente de los envíos.</td>
        <td rowspan="2">US01</td>
        <td rowspan="2">Como gerente, quiero poder asignar rutas específicas a mis transportistas para distribuir eficientemente los envíos.</td>
        <td>Criterio 1: Dado que soy un gerente y estoy en el sistema de gestión de rutas, Cuando selecciono un transportista de la lista de disponibles, Luego puedo asignarle una ruta específica predefinida para distribuir los envíos de manera eficiente.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que soy un gerente y he asignado una ruta específica a un transportista, Cuando reviso la lista de transportistas y sus asignaciones en el sistema de gestión de rutas, Luego puedo confirmar que la ruta ha sido correctamente asignada al transportista seleccionado para distribuir eficientemente los envíos.</td>
    </tr>
<!-- SEPARACION DE EPIC -->
    <tr>
        <td rowspan="2">EP02</td>
        <td rowspan="2">Estadísticas de Transportistas: Proporcionar al gerente estadísticas detalladas sobre el rendimiento de los transportistas.</td>
        <td rowspan="2">US02</td>
        <td rowspan="2">Como gerente, quiero ver estadísticas detalladas sobre el rendimiento de mis transportistas, incluyendo viajes exitosos, infracciones vehiculares reportadas y problemas con los paquetes.</td>
        <td>Criterio 1: Dado que soy un gerente y deseo ver estadísticas detalladas sobre el rendimiento de mis transportistas, Cuando accedo al sistema de gestión de transporte, Luego puedo ver un informe que muestra el número de viajes exitosos completados por cada transportista.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que soy un gerente y quiero analizar las infracciones vehiculares reportadas por mis transportistas, Cuando accedo al sistema de gestión de transporte, Luego puedo ver un resumen que muestra el número y tipo de infracciones vehiculares reportadas por cada transportista.</td>
    </tr>
<!-- SEPARACION DE EPIC -->
    <tr>
        <td rowspan="4">EP03</td>
        <td rowspan="4">Configuración de Perfil: Permitir a gerentes y transportistas configurar su perfil.</td>
        <td rowspan="2">US03</td>
        <td rowspan="2">Como gerente, quiero poder modificar mi perfil, incluyendo nombre, número de contacto y correo electrónico.</td>
        <td>Criterio 1: Dado que soy un gerente y deseo modificar mi perfil, Cuando accedo a la configuración de mi cuenta en el sistema, Luego puedo editar y guardar un nuevo nombre para actualizar mi perfil con éxito.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que soy un gerente y necesito actualizar mi información de contacto, Cuando ingreso al apartado de configuración de mi cuenta en el sistema, Luego puedo modificar mi número de contacto y mi dirección de correo electrónico, asegurándome de que los cambios se guarden correctamente en mi perfil.
        </td>
    </tr>
    <tr>
        <td rowspan="2">US04</td>
        <td rowspan="2">Como transportista, quiero poder modificar mi perfil, incluyendo nombre, número de contacto y correo electrónico.</td>
        <td>Criterio 1: : Dado que soy un transportista y deseo modificar mi perfil, Cuando accedo a la configuración de mi cuenta en el sistema, Luego puedo editar y guardar un nuevo nombre para actualizar mi perfil con éxito.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que soy un transportista y necesito actualizar mi información de contacto, Cuando ingreso al apartado de configuración de mi cuenta en el sistema, Luego puedo modificar mi informacion de contacto, asegurándome de que los cambios se guarden correctamente en mi perfil.</td>
    </tr>
<!-- SEPARACION DE EPIC-->
    <tr>
        <td rowspan="4">EP04</td>
        <td rowspan="4">Gestión de Flotas: Permitir al gerente añadir y asignar flotas</td>
        <td rowspan="2">US05</td>
        <td rowspan="2">Como gerente, quiero añadir nuevas flotas a mi negociopara tener un control activo de mis flotas.</td>
        <td>Criterio 1: Dado que soy un gerente y quiero añadir una nueva flota a mi negocio, Cuando accedo al sistema de gestión de flotas, Luego puedo completar un formulario con los detalles de la nueva flota, como nombre, tipo de vehículos y capacidad, y confirmar su creación con éxito.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que he creado una nueva flota en el sistema, Cuando accedo a la sección de gestión de vehículos, Luego puedo seleccionar los vehículos disponibles y asignarlos a la nueva flota, garantizando un control activo de los recursos de mi negocio.</td>
    </tr>
    <tr>
        <td rowspan="2">US06</td>
        <td rowspan="2">Como gerente, quiero asignar flotas a mis transportistas para que pueda tener un mayor control sobre la organizacion de mis flotas.</td>
        <td>Criterio 1: Dado que soy un gerente y quiero asignar flotas a mis transportistas, Cuando accedo al sistema de gestión de flotas y transportistas, Luego puedo seleccionar un transportista específico y asignarle una o varias flotas disponibles en el sistema.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que he asignado flotas a mis transportistas en el sistema, Cuando reviso el perfil de un transportista en el sistema de gestión, Luego puedo ver claramente las flotas que le han sido asignadas.</td>
    </tr>
<!-- SEPARACION DE EPIC-->
    <tr>
        <td rowspan="8">EP05</td>
        <td rowspan="8">Reporte de Problemas: Permitir a los transportistas reportar problemas.</td>
        <td rowspan="2">US07</td>
        <td rowspan="2">Como transportista, quiero poder reportar problemas técnicos que surjan durante mis viajes para que el gerente pueda resolverlo lo antes posible.</td>
        <td>Criterio 1: Dado que soy un transportista en ruta y encuentro un problema técnico en mi vehículo, Cuando accedo a la aplicación, Luego puedo detallar el problema técnico y enviar un reporte para que pueda tomar medidas correctivas lo antes posible.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que soy un gerente y necesito mantener un registro de los problemas técnicos reportados por los transportistas, Cuando reviso el sistema de reporte de incidencias, Luego puedo acceder a un historial detallado que muestra todos los problemas técnicos reportados por los transportistas.</td>
    </tr>
    <tr>
        <td rowspan="2">US08</td>
        <td rowspan="2">Como transportista, quiero poder reportar infracciones vehiculares que ocurran durante mis viajes para que el gerente pueda tomar las medidas del caso.</td>
        <td>Criterio 1: Dado que soy un transportista en ruta y observo una infracción vehicular, Cuando tengo acceso a la aplicación o sistema de reporte de incidencias, Luego puedo documentar la infracción detalladamente y enviar un reporte al gerente para que pueda tomar las medidas adecuadas.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que soy un gerente y necesito gestionar reportes de infracciones vehiculares, Cuando reviso el sistema de reporte de incidencias, Luego puedo acceder a los reportes de infracciones enviados por los transportistas.</td>
    </tr>
    <tr>
        <td rowspan="2">US09</td>
        <td rowspan="2">Como transportista, quiero poder reportar accidentes en la carretera que ocurran durante mis viajes para que el gerente pueda organizar las futuras rutas.</td>
        <td>Criterio 1: Dado que soy un transportista en ruta y me encuentro con un accidente en la carretera, Cuando tengo acceso a la aplicación, Luego puedo registrar el accidente detalladamente, incluyendo la ubicación exacta, y enviar un reporte para que pueda tomar las medidas necesarias.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que soy un gerente y recibo un reporte de accidente en la carretera, Cuando reviso el sistema de reporte de incidencias, Luego puedo evaluar la gravedad del accidente, tomar las medidas necesarias para garantizar la seguridad de los transportistas y los envíos.</td>
    </tr>
    <tr>
        <td rowspan="2">US10</td>
        <td rowspan="2">Como transportista, quiero poder reportar problemas con los paquetes que transporto durante mis viajes para que el gerente pueda reportarlo al cliente.</td>
        <td>Criterio 1: Dado que soy un transportista en ruta y encuentro problemas con los paquetes que transporto, Cuando tengo acceso a la aplicación, Luego puedo registrar el problema específico encontrado en los paquetes y enviar un reporte para que pueda tomar las medidas necesarias.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que soy un gerente y recibo un reporte de problemas con los paquetes durante un viaje, Cuando reviso el sistema de reporte de incidencias, Luego puedo tomar medidas inmediatas para informar al cliente afectado.</td>
    </tr>
<!-- SEPARACION DE EPIC -->
    <tr>
        <td rowspan="2">EP06</td>
        <td rowspan="2">Visualización de Encargos: Permitir a los transportistas ver los encargos que les han sido asignados.</td>
        <td rowspan="2">US11</td>
        <td rowspan="2">Como transportista, quiero poder ver los encargos que me han sido asignados, incluyendo detalles sobre los envíos y destinos correspondientes para poder organizar mejor el orden de mis tareas.</td>
        <td>Criterio 1: Dado que soy un transportista y necesito ver los encargos asignados, Cuando accedo al sistema de gestión de encargos, Luego puedo ver una lista detallada de los encargos que me han sido asignados.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que soy un transportista y quiero obtener más detalles sobre un encargo asignado, Cuando selecciono un encargo específico de la lista de encargos asignados, Luego puedo acceder a información adicional.</td>
    </tr>
<!-- SEPARACION DE EPIC -->
    <tr>
        <td rowspan="2">EP07</td>
        <td rowspan="2">Visualización de Estadísticas Personales: Permitir a los transportistas ver sus propias estadísticas</td>
        <td rowspan="2">US12</td>
        <td rowspan="2">Como transportista, quiero poder ver mis propias estadísticas, incluyendo viajes completados, por completar y cancelados, así como los reportes enviados para tener un control de mi rendimiento.</td>
        <td>Criterio 1: Dado que soy un transportista y quiero ver mis propias estadísticas de viajes, Cuando accedo al sistema de gestión de transporte, Luego puedo ver un resumen de mis viajes completados, viajes por completar y viajes cancelados.</td>
    </tr>
    <tr>
        <td>Criterio 2: Dado que soy un transportista y deseo ver los reportes que he enviado, Cuando accedo a mi perfil en el sistema de gestión, Luego puedo ver una lista de todos los reportes que he enviado.</td>
    </tr>
<!-- SEPARACION DE EPIC -->
</table>

### 3.2.2 User Stories Landing Page

<table>
    <tr>
        <th>Epic ID</th>
        <th>Descripcion</th>
        <th>User Story ID</th>
        <th>Descripcion</th>
        <th>Criterios de Aceptacion</th>
    </tr>
    <!-- ENCABEZADOS -->
    <tr>
        <td rowspan="4">EP08</td>
        <td rowspan="4">Encabezado</td>
        <td rowspan="2">US13</td>
        <td rowspan="2">Como visitante quiero que la pagina me permita dirigirme directamente a la sección que más considere oportuna según la situación </td>
        <td>Criterio 1 - El visitante puede navegar por la pagina de presentación:<br>DADO el visitante se encuentra en la barra de navegación CUANDO haga clic en la opción de sección de su interés. ENTONCES se redirige automáticamente a la seccion en la pagina</td>
    </tr>
    <tr>
        <td>Criterio 2 - Error de navegacion: <br>DADO el visitante se encuentra en la barra de navegación CUANDO haga clic en la opción de sección de su interés.LUEGO la pagina no enonctrara el apartado elegido. ENTONCES se redirige automáticamente a una pagina de error</td>
    </tr>
    <tr>
        <td rowspan="2">US14</td>
        <td rowspan="2">Como visitante quiero que la pagina me permita dirigirme directamente a la aplicacion web principal para acceder rapidamente a la aplicacion principal.</td>
        <td>Criterio 1 - El visitante se redirige a la aplicacion:<br>DADO que el visitante se encuentra en la pagina de presentacion(landing page). Cuando de click al boton "Empezar", entonces se redirigira a la aplicacion</td>
    </tr>
    <tr>
        <td>Criterio 2 - Error de redireccion: <br>DADO el visitante se encuentra en la pagina de presentacion. Cuando le de click al boton "Empezar. Luego la pagina no encontrara la direccion asociada al boton. Entonces se redirigira a una pagina de error."</td>
    </tr>
    <!-- SEPARACION EPIC -->
    <tr>
        <td rowspan="2">EP09</td>
        <td rowspan="2">Contenido</td>
        <td rowspan="2">US15</td>
        <td rowspan="2">Como visitante quiero que la pagina me brinde información introductoria sobre lo que ofrece tales como servicios, precios y contacto</td>
        <td>Criterio 1 - El es redirigido segun la seccion elegida:<br>DADO el visitante se encuentra en la barra de navegación CUANDO haga clic en la opción de sección de su interés. ENTONCES se redirige automáticamente a la seccion en la pagina</td>
    </tr>
    <tr>
        <td>Criterio 2 - Error de navegacion: <br>DADO el visitante se encuentra en la barra de navegación CUANDO haga clic en la opción de sección de su interés.LUEGO la pagina no encontrara el apartado elegido. ENTONCES se redirige automáticamente a una pagina de error</td>
    </tr>
    <!-- SEPARACION EPIC -->
    <tr>
        <td rowspan="2">EP010</td>
        <td rowspan="2">Seccion footer</td>
        <td rowspan="2">US16</td>
        <td rowspan="2">Como visitante quiero que la pagina me brinde información sobre secciones de interés como redes sociales, una barra de navegación y contacto de la empresa</td>
        <td>Criterio 1 - Visitante recibe informacion adicional:<br>DADO el usuario se encuentra en la sección de “Contacto” CUANDO haga clic en la opción de su interés actual ENTONCES se redirige automáticamente a las redes sociales o se suscriba dejando su correo</td>
    </tr>
    <tr>
        <td>Criterio 2 - Error de navegacion: <br>DADO el visitante se encuentra en la seccion de footer CUANDO haga clic en la opción de sección de su interés.LUEGO la pagina no encontrara el apartado elegido. ENTONCES se redirige automáticamente a una pagina de error</td>
    </tr>
    <!-- SEPARACION EPIC -->
    
</table>

## 3.3 Impact Mapping
EMPRESARIO
![Impact Mapping Empresario 1](/assets/chapter03/ImpactMapGerente1.png)

![Impact Mapping Empresario 2](/assets/chapter03/ImpactMapGerente2.png)

![Impact Mapping Empresario 3](/assets/chapter03/ImpactMapGerente3.png)

TRANSPORTISTA
![Impact Maapping Transportista 1](/assets/chapter03/ImpactMapTrans1.png)

![Impact Maapping Transportista 2](/assets/chapter03/ImpactMapTrans2.png)

![Impact Maapping Transportista 3](/assets/chapter03/ImpactMapTrans3.png)

## 3.4 Product Backlog

| #Orden | User Story ID | Titulo | Descripcion | Story Points (1/2/3/5/8) |
|--------|---------------|--------|-------------|--------------------------|
| 1 | US14 | Landing - Dirigir a aplicacion web | Como visitante quiero que la pagina me permita dirigirme directamente a la aplicacion web principal para acceder rapidamente a la aplicacion principal. | 2 |
| 2 | US13 | Landing - Navegacion | Como visitante quiero que la pagina me permita dirigirme directamente a la sección que más considere oportuna según la situación | 2 |
| 3 | US15 | Landing - Encabezado | Como visitante quiero que la pagina me brinde información introductoria sobre lo que ofrece tales como servicios, precios y contacto | 2 |
| 4 | US16 | Landing - contactoFooter | Como visitante quiero que la pagina me brinde información sobre secciones de interés como redes sociales, una barra de navegación y contacto de la empresa | 2 |
| 5 | US01 | Gerente - AsignarRutas | Como gerente, quiero poder asignar rutas específicas a mis transportistas para distribuir eficientemente los envíos. | 5 |
| 6 | US06 | Gerente - Asignar Flotas | Como gerente, quiero asignar flotas a mis transportistas para que pueda tener un mayor control sobre la organizacion de mis flotas. | 5 |
| 7 | US11 | Transportista - EncargosAsignados | Como transportista, quiero poder ver los encargos que me han sido asignados, incluyendo detalles sobre los envíos y destinos correspondientes para poder organizar mejor el orden de mis tareas. | 3 |
| 8 | US05 | Gerente - Añadirflotas | Como gerente, quiero añadir nuevas flotas a mi negocio para tener un control activo de mis flotas. | 3 |
| 9 | US07 | Transportista - ReportarTecnico | Como transportista, quiero poder reportar problemas técnicos que surjan durante mis viajes para que el gerente pueda resolverlo lo antes posible. | 3 |
| 10 | US10 | Transportista - ReportarPaquete | Como transportista, quiero poder reportar problemas con los paquetes que transporto durante mis viajes para que el gerente pueda reportarlo al cliente. | 3 |
| 11 | US08 | Transportista - ReportarInfracciones | Como transportista, quiero poder reportar infracciones vehiculares que ocurran durante mis viajes para que el gerente pueda tomar las medidas del caso. | 3 |
| 12 | US09 | Transportista - ReportarAccidentes | Como transportista, quiero poder reportar accidentes en la carretera que ocurran durante mis viajes para que el gerente pueda organizar las futuras rutas. | 3 |
| 13 | US02 | Gerente - Estadisticas | Como gerente, quiero ver estadísticas detalladas sobre el rendimiento de mis transportistas, incluyendo viajes exitosos, infracciones vehiculares reportadas y problemas con los paquetes. | 2 |
| 14 | US12 | Transportista - Estadistica | Como transportista, quiero poder ver mis propias estadísticas, incluyendo viajes completados, por completar y cancelados, así como los reportes enviados para tener un control de mi rendimiento. | 2 |
| 15 | US03 | Gerente - Perfil | Como gerente, quiero poder modificar mi perfil, incluyendo nombre, número de contacto y correo electrónico. | 2 |
| 16 | US04 | Transportista - Perfil | Como transportista, quiero poder modificar mi perfil, incluyendo nombre, número de contacto y correo electrónico. | 2 |

Jira Software Imagen:
![Product Backlog](/assets/chapter03/Product%20backlog.png)
