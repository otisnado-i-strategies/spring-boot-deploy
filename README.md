![](RackMultipart20211122-4-15ie4z6_html_19519eafc905a0c0.jpg)

![](RackMultipart20211122-4-15ie4z6_html_6d28cf41d8dff0d7.png)

# DOCUMENTACIÓN TÉCNICA

# SOP - DELSUR

![](RackMultipart20211122-4-15ie4z6_html_918aea6943676f6d.png)

# Contenido

_**[1.](#_Toc88458025)**__ **BASES DE DATOS 3** _

**[1.1.](#_Toc88458026)****ESQUEMAS 3**

[1.1.1. SEC\_USR 3](#_Toc88458027)

[1.1.2. SOP 3](#_Toc88458028)

[1.1.2.1. Tablas Creadas 3](#_Toc88458029)

[Tablas Modificadas: 4](#_Toc88458030)

[1.1.2.2. Secuencias Creadas 4](#_Toc88458031)

[1.1.2.3. Secuencias Modificadas 4](#_Toc88458032)

[1.1.2.4. Disparadores Creados 5](#_Toc88458033)

[1.1.2.5. Disparadores Modificados 5](#_Toc88458034)

[1.1.2.6. Paquetes Creados 5](#_Toc88458035)

[1.1.2.7. Paquetes Modificados 6](#_Toc88458036)

_**[2.](#_Toc88458037)**__ **SERVICIOS 6** _

**[1.2.](#_Toc88458038)****FIRMAS 6**

[1.2.1. Servidor de Reporting Services 6](#_Toc88458039)

[1.2.2. Acceso a carpeta compartida para guardado de firmas 7](#_Toc88458040)

**[1.3.](#_Toc88458041)****CARPETA PARA GENERACIÓN DE LOGS 9**

[1.3.1.Tarea Programada 9](#_Toc88458042)

_**[3.](#_Toc88458043)**__ **APLICACIÓN 10** _

**[1.4.](#_Toc88458044)****MENU PRINCIPAL 10**

[1.4.1. Elementos Creados 10](#_Toc88458045)

1.
# B ![](RackMultipart20211122-4-15ie4z6_html_324a8b6d3380e89f.png) ASES DE DATOS

  1.
## ESQUEMAS

- SEC\_USR: Seguridad, Autenticación y Roles.
- SOP: Datos asociados a la aplicación SOP.

####

    1.
### SEC\_USR

En esta parte solo se ingresaron nuevos registros en la tabla SEC\_USR.ORA\_ASPNET\_SITEMAP para mostrar nuevos elementos en el menú de SOP:

![](RackMultipart20211122-4-15ie4z6_html_4895ab306cd174e6.png)

    1.
### SOP

      1.
### Tablas Creadas

- SOP\_ANEXO\_BDI
- SOP\_ANEXO\_HORASEJECUCION
- SOP\_CONDICION\_DEFI
- SOP\_CONDICIONES\_FLUJO

- SOP\_EMERGENCIA
- SOP\_ESTADO
- SOP\_FIRMA\_USUARIO
- SOP\_LIMITESDEINGRESO
- SOP\_MENSAJE\_PERSONALIZADO

- SOP\_TICKET\_OMS
- SOP\_TIPO\_INSTALACION
- SOP\_VOLUMEN\_TRABAJO

### Tablas Modificadas:

- SOP\_ANEXO\_PUB
- SOP\_AREA
- SOP\_CIRCUITO\_OP
- SOP\_EMPLEADO
- SOP\_EQUIPO\_ORDEN

- SOP\_FERIADO
- SOP\_ORDEN\_OPERACION
- SOP\_SEG\_ORDEN

      1.
### Secuencias Creadas

- SOP\_SEQ\_CONDICIONES\_FLUJO
- SOP\_SEQ\_CONDICION\_DEFI
- SOP\_SEQ\_IDANEXODES
- SOP\_SEQ\_IDANEXO\_HORASEJECUCION

- SOP\_SEQ\_IDESTADO
- SOP\_SEQ\_IDLIMITESDEINGRESO
- SOP\_SEQ\_ID\_EMERGENCIA
- SOP\_SEQ\_ID\_FIRMA\_USUARIO
- SOP\_SEQ\_ID\_INSTALACION

- SOP\_SEQ\_ID\_TICKET\_OMS
- SOP\_SEQ\_ID\_VOLUMEN\_TRABAJO
- SOP\_SEQ\_MENSAJE\_PERSONALIZADO

      1.
### Secuencias Modificadas

- SOP\_SEQ\_IDEQUIPO\_ORD

      1.
### Disparadores Creados

- SOP\_TR\_ID\_ANEXO\_CAL
- SOP\_TR\_ID\_ANEXO\_DES

- SOP\_TR\_ID\_ANEXO\_HORASEJECUCION
- SOP\_TR\_ID\_ANEXO\_PUB
- SOP\_TR\_ID\_CONDICIONES\_FLUJO
- SOP\_TR\_ID\_CONDICION\_DEFI
- SOP\_TR\_ID\_EMERGENCIA

- SOP\_TR\_ID\_ESTADO
- SOP\_TR\_ID\_FIRMA\_USUARIO
- SOP\_TR\_ID\_LIMITESDEINGRESO
- SOP\_TR\_ID\_MENSAJE\_PERSONALIZADO
- SOP\_TR\_ID\_TICKET\_OMS

- SOP\_TR\_ID\_TIPO\_INSTALACION
- SOP\_TR\_ID\_VOLUMEN\_TRABAJO

      1.
### Disparadores Modificados

- SOP\_TR\_ID\_EQUIPO\_ORD

- SOP\_TR\_ID\_AREA

      1.
### Paquetes Creados

- SOP\_PKG\_CONDICIONES\_FLUJO
- SOP\_PKG\_CONDICION\_DEFI

- SOP\_PKG\_EMERGENCIA
- SOP\_PKG\_ESTADO
- SOP\_PKG\_FIRMA\_USUARIO
- SOP\_PKG\_FLUJO\_DETALLE\_ALTERNO
- SOP\_PKG\_LIMITESDEINGRESO

- SOP\_PKG\_LOG\_FILE
- SOP\_PKG\_MENSAJE\_PERSONALIZADO
- SOP\_PKG\_TICKET\_OMS
- SOP\_PKG\_TIPO\_INSTALACION
- SOP\_PKG\_VALIDAR\_ENVIO\_BDI

- SOP\_PKG\_VOLUMEN\_TRABAJO

      1.
### Paquetes Modificados

- SOP\_PKG\_REPORTE
- SOP\_PKG\_ORDEN\_OPERACION

- SOP\_PKG\_SEG\_ORDEN
- SOP\_PKG\_ANEXO\_DESCONEX
- SOP\_PKG\_ANEXO\_ORDEN
- SOP\_PKG\_AREA
- SOP\_PKG\_CIRCUITO\_OP

- SOP\_PKG\_FLUJO\_DETALLE
- SOP\_PKG\_MAIL
- SOP\_PKG\_ANEXO\_CALIFICACION
- SOP\_PKG\_ANEXO\_BDI
- SOP\_PKG\_ANEXO

- SOP\_PKG\_BACKLOG



1.
# SERVICIOS

  1.
## FIRMAS

    1.
### Servidor de Reporting Services

Es necesario contar con un servidor de Reporting Services en donde se almacene el reporte siguiente:

OrdenOp:

![](RackMultipart20211122-4-15ie4z6_html_e143014c056f4917.png)

La ubicación del servidor de reportes y del servidor de imágenes se debe definir en el archivo web.config (Para el caso de este ejemplo, el servidor de reportes y el servidor de imágenes son el mismo SERVIDOR, pero podrían variar):

\&lt;addkey=&quot;FolderSharedUrl&quot;value=&quot;http://SERVIDOR/&quot; /\&gt;

\&lt;addkey=&quot;FolderShared&quot;value=&quot;\\SERVIDOR\&quot; /\&gt;

\&lt;addkey=&quot;REPORT\_SERVER&quot;value=&quot;http://SERVIDOR/ReportServer&quot;\&gt;\&lt;/add\&gt;

    1.
### Acceso a carpeta compartida para guardado de firmas

Es necesario contar con un servidor web en donde se almacenen las imágenes que representan las firmas digitales que ingresen los usuarios al momento de autorizar órdenes o desde el mantenimiento de firmas:

Autorización:

![](RackMultipart20211122-4-15ie4z6_html_4494fd3809579542.png)

Mantenimiento de Firmas:

![](RackMultipart20211122-4-15ie4z6_html_459f00e32f160ef5.png)

Servidor Web:

![](RackMultipart20211122-4-15ie4z6_html_b1534b4fee715daf.png)

Carpeta Compartida:

\\SERVIDOR\images

![](RackMultipart20211122-4-15ie4z6_html_e130edc8c7542488.png)

**Consideración Especial:**

En el servidor donde se almacenarán imágenes de las firmas, se debe contemplar el permiso de lectura/escritura para el usuario del servidor web. En el caso presentado anteriormente, tanto el servidor de Reporting Services, como el Servidor Web, son el mismo.

En el caso en que los servidores sean diferentes, al usuario con el cual se configure IIS, donde se instale la aplicación, debe brindar acceso de lectura-escritura a la carpeta C:\IMAGES, al usuario de IIS dentro de ese servidor, y permiso de lectura para todos los demás usuarios, debido a que las imágenes deben ser accesibles vía web, para todos los usuarios del sistema SOP.

  1.
## CARPETA PARA GENERACIÓN DE LOGS

    1.
### Tarea Programada

Se ha implementado una tarea programada llamada &quot;CORREO\_BDI\_AUTOMATICO\_JOB&quot;, la cual necesita una carpeta en el servidor de Base de Datos de Oracle donde se encuentre el esquema &quot;SOP&quot;.

Se recomienda que la carpeta se llame &quot;C:\LOG\_FILE&quot;.

![](RackMultipart20211122-4-15ie4z6_html_a354edb3e211e1c0.png)

1.
# APLICACIÓN

  1.
## MENU PRINCIPAL

    1.
### Elementos Creados

Se han agregado los elementos siguientes (con sus correspondientes registros en la tabla &quot;ORA\_ASPNET\_SITEMAP&quot; del Esquema de Base de Datos &quot;SEC\_USR&quot;):

- Configuración:
  - Estado instalación.
  - Acciones por workflow.
  - Estados de Órdenes.
  - Firmas.
  - Mensajes de Correo.
  - Tipos BDI:
    - Tipos de Instalación.
    - Volumen de Trabajo.
    - Emergencia.
  - Sincronizar Datos.
  - Condiciones Predefinidas.
- Reportes:
  - Visor de Trabajos Programados.
  - Planificación de Trabajos.
- Consulta BDI:
  - Datos Notificados BDI.
- Búsqueda de Órdenes.

![](RackMultipart20211122-4-15ie4z6_html_da042d45ba97b4ce.png)

![](RackMultipart20211122-4-15ie4z6_html_c3f0147900d4acd4.png)

![](RackMultipart20211122-4-15ie4z6_html_e2fbd9f9863ac49.png) ![](RackMultipart20211122-4-15ie4z6_html_dffff82ec8143f64.png)

![](RackMultipart20211122-4-15ie4z6_html_bf65bc83acf0c5e3.png)

![](RackMultipart20211122-4-15ie4z6_html_26e46b511ee9f510.png)

15

![](RackMultipart20211122-4-15ie4z6_html_6f724ba18cb75ac3.jpg)
