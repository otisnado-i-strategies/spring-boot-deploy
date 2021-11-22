<img src="media/image1.png" style="width:1.95in;height:1.96806in" />

DOCUMENTACIÓN TÉCNICA

SOP - DELSUR

<img src="media/image2.png" style="width:2.97829in;height:1.77165in" />

# Contenido

[1. BASES DE DATOS [3](#bases-de-datos)](#bases-de-datos)

[1.1. ESQUEMAS [3](#esquemas)](#esquemas)

[1.1.1. SEC_USR [3](#sec_usr)](#sec_usr)

[1.1.2. SOP [3](#sop)](#sop)

[1.1.2.1. Tablas Creadas [3](#tablas-creadas)](#tablas-creadas)

[Tablas Modificadas: [4](#tablas-modificadas)](#tablas-modificadas)

[1.1.2.2. Secuencias Creadas
[4](#secuencias-creadas)](#secuencias-creadas)

[1.1.2.3. Secuencias Modificadas
[4](#secuencias-modificadas)](#secuencias-modificadas)

[1.1.2.4. Disparadores Creados
[5](#disparadores-creados)](#disparadores-creados)

[1.1.2.5. Disparadores Modificados
[5](#disparadores-modificados)](#disparadores-modificados)

[1.1.2.6. Paquetes Creados [5](#paquetes-creados)](#paquetes-creados)

[1.1.2.7. Paquetes Modificados
[6](#paquetes-modificados)](#paquetes-modificados)

[2. SERVICIOS [6](#servicios)](#servicios)

[1.2. FIRMAS [6](#firmas)](#firmas)

[1.2.1. Servidor de Reporting Services
[6](#servidor-de-reporting-services)](#servidor-de-reporting-services)

[1.2.2. Acceso a carpeta compartida para guardado de firmas
[7](#acceso-a-carpeta-compartida-para-guardado-de-firmas)](#acceso-a-carpeta-compartida-para-guardado-de-firmas)

[1.3. CARPETA PARA GENERACIÓN DE LOGS
[9](#carpeta-para-generación-de-logs)](#carpeta-para-generación-de-logs)

[1.3.1. Tarea Programada [9](#tarea-programada)](#tarea-programada)

[3. APLICACIÓN [10](#aplicación)](#aplicación)

[1.4. MENU PRINCIPAL [10](#menu-principal)](#menu-principal)

[1.4.1. Elementos Creados [10](#elementos-creados)](#elementos-creados)

# <img src="media/image3.png" style="width:0.30751in;height:0.3189in" />BASES DE DATOS

** **

## ESQUEMAS

-   SEC_USR: Seguridad, Autenticación y Roles. 

-   SOP: Datos asociados a la aplicación SOP. 

#### ** **

### SEC_USR 

> En esta parte solo se ingresaron nuevos registros en la tabla
> SEC_USR.ORA_ASPNET_SITEMAP para mostrar nuevos elementos en el menú de
> SOP: 
>
> <img src="media/image4.png" style="width:5.62662in;height:1.50935in" alt="Graphical user interface, application, table Description automatically generated" /> 
>
>  

2.  ### SOP 

    1.  ### Tablas Creadas 

-   SOP_ANEXO_BDI 

-   SOP_ANEXO_HORASEJECUCION 

-   SOP_CONDICION_DEFI 

-   SOP_CONDICIONES_FLUJO 

<!-- -->

-   SOP_EMERGENCIA 

-   SOP_ESTADO 

-   SOP_FIRMA_USUARIO 

-   SOP_LIMITESDEINGRESO 

-   SOP_MENSAJE_PERSONALIZADO 

<!-- -->

-   SOP_TICKET_OMS 

-   SOP_TIPO_INSTALACION 

-   SOP_VOLUMEN_TRABAJO 

> ** **

### Tablas Modificadas: 

-   SOP_ANEXO_PUB 

-   SOP_AREA 

-   SOP_CIRCUITO_OP 

-   SOP_EMPLEADO 

-   SOP_EQUIPO_ORDEN 

<!-- -->

-   SOP_FERIADO 

-   SOP_ORDEN_OPERACION 

-   SOP_SEG_ORDEN 

> ** **

### Secuencias Creadas 

-   SOP_SEQ_CONDICIONES_FLUJO 

-   SOP_SEQ_CONDICION_DEFI 

-   SOP_SEQ_IDANEXODES 

-   SOP_SEQ_IDANEXO_HORASEJECUCION 

<!-- -->

-   SOP_SEQ_IDESTADO 

-   SOP_SEQ_IDLIMITESDEINGRESO 

-   SOP_SEQ_ID_EMERGENCIA 

-   SOP_SEQ_ID_FIRMA_USUARIO 

-   SOP_SEQ_ID_INSTALACION 

<!-- -->

-   SOP_SEQ_ID_TICKET_OMS 

-   SOP_SEQ_ID_VOLUMEN_TRABAJO 

-   SOP_SEQ_MENSAJE_PERSONALIZADO 

> ** **

### Secuencias Modificadas 

-   SOP_SEQ_IDEQUIPO_ORD 

> ** **

### Disparadores Creados 

-   SOP_TR_ID_ANEXO_CAL 

-   SOP_TR_ID_ANEXO_DES 

<!-- -->

-   SOP_TR_ID_ANEXO_HORASEJECUCION 

-   SOP_TR_ID_ANEXO_PUB 

-   SOP_TR_ID_CONDICIONES_FLUJO 

-   SOP_TR_ID_CONDICION_DEFI 

-   SOP_TR_ID_EMERGENCIA 

<!-- -->

-   SOP_TR_ID_ESTADO 

-   SOP_TR_ID_FIRMA_USUARIO 

-   SOP_TR_ID_LIMITESDEINGRESO 

-   SOP_TR_ID_MENSAJE_PERSONALIZADO 

-   SOP_TR_ID_TICKET_OMS 

<!-- -->

-   SOP_TR_ID_TIPO_INSTALACION 

-   SOP_TR_ID_VOLUMEN_TRABAJO 

> ** **

### Disparadores Modificados 

-   SOP_TR_ID_EQUIPO_ORD 

<!-- -->

-   SOP_TR_ID_AREA 

> ** **

### Paquetes Creados 

-   SOP_PKG_CONDICIONES_FLUJO 

-   SOP_PKG_CONDICION_DEFI 

<!-- -->

-   SOP_PKG_EMERGENCIA 

-   SOP_PKG_ESTADO 

-   SOP_PKG_FIRMA_USUARIO 

-   SOP_PKG_FLUJO_DETALLE_ALTERNO 

-   SOP_PKG_LIMITESDEINGRESO 

<!-- -->

-   SOP_PKG_LOG_FILE 

-   SOP_PKG_MENSAJE_PERSONALIZADO 

-   SOP_PKG_TICKET_OMS 

-   SOP_PKG_TIPO_INSTALACION 

-   SOP_PKG_VALIDAR_ENVIO_BDI 

<!-- -->

-   SOP_PKG_VOLUMEN_TRABAJO 

** **

### Paquetes Modificados 

-   SOP_PKG_REPORTE 

-   SOP_PKG_ORDEN_OPERACION 

<!-- -->

-   SOP_PKG_SEG_ORDEN 

-   SOP_PKG_ANEXO_DESCONEX 

-   SOP_PKG_ANEXO_ORDEN 

-   SOP_PKG_AREA 

-   SOP_PKG_CIRCUITO_OP 

<!-- -->

-   SOP_PKG_FLUJO_DETALLE 

-   SOP_PKG_MAIL 

-   SOP_PKG_ANEXO_CALIFICACION 

-   SOP_PKG_ANEXO_BDI 

-   SOP_PKG_ANEXO 

<!-- -->

-   SOP_PKG_BACKLOG 

** **

>  

2.  # SERVICIOS

    1.  ## FIRMAS

        1.  ### Servidor de Reporting Services

> Es necesario contar con un servidor de Reporting Services en donde se
> almacene el reporte siguiente:
>
> OrdenOp:
>
> <img src="media/image5.png" style="width:6.07292in;height:2.55903in" alt="Graphical user interface, application Description automatically generated" />
>
> La ubicación del servidor de reportes y del servidor de imágenes se
> debe definir en el archivo web.config (Para el caso de este ejemplo,
> el servidor de reportes y el servidor de imágenes son el mismo
> SERVIDOR, pero podrían variar):
>
> \<add key="FolderSharedUrl" value="http://SERVIDOR/" />
>
> \<add key="FolderShared" value="\\\\SERVIDOR\\" />
>
> \<add key="REPORT_SERVER" value="http://SERVIDOR/ReportServer">\</add>

### Acceso a carpeta compartida para guardado de firmas

>  
>
> Es necesario contar con un servidor web en donde se almacenen las
> imágenes que representan las firmas digitales que ingresen los
> usuarios al momento de autorizar órdenes o desde el mantenimiento de
> firmas:
>
> Autorización:
>
> <img src="media/image6.png" style="width:2.83688in;height:3.49057in" alt="Graphical user interface, text, application Description automatically generated" />
>
> Mantenimiento de Firmas:
>
> <img src="media/image7.png" style="width:5.37736in;height:2.07598in" alt="Graphical user interface, text, application, email Description automatically generated" />
>
> Servidor Web:
>
> <img src="media/image8.png" style="width:6.01042in;height:2.03067in" alt="A screenshot of a computer Description automatically generated with medium confidence" />
>
> Carpeta Compartida:
>
> \\\\SERVIDOR\\images
>
> <img src="media/image9.png" style="width:6.1375in;height:2.25069in" alt="Graphical user interface, application Description automatically generated" />
>
>  
>
> **Consideración Especial:**
>
> En el servidor donde se almacenarán imágenes de las firmas, se debe
> contemplar el permiso de lectura/escritura para el usuario del
> servidor web. En el caso presentado anteriormente, tanto el servidor
> de Reporting Services, como el Servidor Web, son el mismo.
>
> En el caso en que los servidores sean diferentes, al usuario con el
> cual se configure IIS, donde se instale la aplicación, debe brindar
> acceso de lectura-escritura a la carpeta C:\\IMAGES, al usuario de IIS
> dentro de ese servidor, y permiso de lectura para todos los demás
> usuarios, debido a que las imágenes deben ser accesibles vía web, para
> todos los usuarios del sistema SOP.

2.  ## CARPETA PARA GENERACIÓN DE LOGS

    1.  ### Tarea Programada 

> Se ha implementado una tarea programada llamada
> “CORREO_BDI_AUTOMATICO_JOB”, la cual necesita una carpeta en el
> servidor de Base de Datos de Oracle donde se encuentre el esquema
> “SOP”.
>
> Se recomienda que la carpeta se llame “C:\\LOG_FILE”.
>
> <img src="media/image10.png" style="width:4.61458in;height:0.5625in" alt="A picture containing shape Description automatically generated" />

3.  # APLICACIÓN

    1.  ## MENU PRINCIPAL

        1.  ### Elementos Creados

> Se han agregado los elementos siguientes (con sus correspondientes
> registros en la tabla “ORA_ASPNET_SITEMAP” del Esquema de Base de
> Datos “SEC_USR”):

-   Configuración:

    -   Estado instalación.

    -   Acciones por workflow.

    -   Estados de Órdenes.

    -   Firmas.

    -   Mensajes de Correo.

    -   Tipos BDI:

        -   Tipos de Instalación.

        -   Volumen de Trabajo.

        -   Emergencia.

    -   Sincronizar Datos.

    -   Condiciones Predefinidas.

-   Reportes:

    -   Visor de Trabajos Programados.

    -   Planificación de Trabajos.

-   Consulta BDI:

    -   Datos Notificados BDI.

-   Búsqueda de Órdenes.

> <img src="media/image11.png" style="width:6.1375in;height:2.55208in" alt="Graphical user interface, text Description automatically generated" />
>
> <img src="media/image12.png" style="width:6.1375in;height:2.70486in" alt="Graphical user interface, text, application Description automatically generated" />
>
> <img src="media/image13.png" style="width:6.1375in;height:1.69792in" alt="Graphical user interface, text, application Description automatically generated" />
> <img src="media/image14.png" style="width:6.1375in;height:1.28958in" alt="Graphical user interface, text, application Description automatically generated" />
>
> <img src="media/image15.png" style="width:6.1375in;height:1.4375in" alt="Graphical user interface, text, application, website Description automatically generated" />
>
> <img src="media/image16.png" style="width:6.1375in;height:1.28056in" alt="Background pattern Description automatically generated with medium confidence" />
