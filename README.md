# DOCUMENTACIÓN TÉCNICA

# SOP - DELSUR


## Contenido

- 1. BASES DE DATOS
   - 1.1. ESQUEMAS
      - 1.1.1. SEC_USR
      - 1.1.2. SOP
      - 1.1.2.1. Tablas Creadas
      - Tablas Modificadas:
      - 1.1.2.2. Secuencias Creadas.................................................................................................
      - 1.1.2.3. Secuencias Modificadas
      - 1.1.2.4. Disparadores Creados
      - 1.1.2.5. Disparadores Modificados
      - 1.1.2.6. Paquetes Creados
      - 1.1.2.7. Paquetes Modificados
- 2. SERVICIOS
   - 1.2. FIRMAS
      - 1.2.1. Servidor de Reporting Services
      - 1.2.2. Acceso a carpeta compartida para guardado de firmas
   - 1.3. CARPETA PARA GENERACIÓN DE LOGS
      - 1.3.1. Tarea Programada
- 3. APLICACIÓN
   - 1.4. MENU PRINCIPAL
      - 1.4.1. Elementos Creados


## 1. BASES DE DATOS

### 1.1. ESQUEMAS

- SEC_USR: Seguridad, Autenticación y Roles.
- SOP: Datos asociados a la aplicación SOP.

#### 1.1.1. SEC_USR

```
En esta parte solo se ingresaron nuevos registros en la tabla
SEC_USR.ORA_ASPNET_SITEMAP para mostrar nuevos elementos en el
menú de SOP:
```
#### 1.1.2. SOP

#### 1.1.2.1. Tablas Creadas

##### • SOP_ANEXO_BDI

##### • SOP_ANEXO_HORASEJECUCION

##### • SOP_CONDICION_DEFI

##### • SOP_CONDICIONES_FLUJO

##### • SOP_EMERGENCIA

##### • SOP_ESTADO

##### • SOP_FIRMA_USUARIO

##### • SOP_LIMITESDEINGRESO

##### • SOP_MENSAJE_PERSONALIZADO

##### • SOP_TICKET_OMS

##### • SOP_TIPO_INSTALACION

##### • SOP_VOLUMEN_TRABAJO


#### Tablas Modificadas:

##### • SOP_ANEXO_PUB

##### • SOP_AREA

##### • SOP_CIRCUITO_OP

##### • SOP_EMPLEADO

##### • SOP_EQUIPO_ORDEN

##### • SOP_FERIADO

##### • SOP_ORDEN_OPERACION

##### • SOP_SEG_ORDEN

#### 1.1.2.2. Secuencias Creadas.................................................................................................

##### • SOP_SEQ_CONDICIONES_FLUJO

##### • SOP_SEQ_CONDICION_DEFI

##### • SOP_SEQ_IDANEXODES

##### • SOP_SEQ_IDANEXO_HORASEJECUCION

##### • SOP_SEQ_IDESTADO

##### • SOP_SEQ_IDLIMITESDEINGRESO

##### • SOP_SEQ_ID_EMERGENCIA

##### • SOP_SEQ_ID_FIRMA_USUARIO

##### • SOP_SEQ_ID_INSTALACION

##### • SOP_SEQ_ID_TICKET_OMS

##### • SOP_SEQ_ID_VOLUMEN_TRABAJO

##### • SOP_SEQ_MENSAJE_PERSONALIZADO

#### 1.1.2.3. Secuencias Modificadas

##### • SOP_SEQ_IDEQUIPO_ORD


#### 1.1.2.4. Disparadores Creados

##### • SOP_TR_ID_ANEXO_CAL

##### • SOP_TR_ID_ANEXO_DES

##### • SOP_TR_ID_ANEXO_HORASEJECUCION

##### • SOP_TR_ID_ANEXO_PUB

##### • SOP_TR_ID_CONDICIONES_FLUJO

##### • SOP_TR_ID_CONDICION_DEFI

##### • SOP_TR_ID_EMERGENCIA

##### • SOP_TR_ID_ESTADO

##### • SOP_TR_ID_FIRMA_USUARIO

##### • SOP_TR_ID_LIMITESDEINGRESO

##### • SOP_TR_ID_MENSAJE_PERSONALIZADO

##### • SOP_TR_ID_TICKET_OMS

##### • SOP_TR_ID_TIPO_INSTALACION

##### • SOP_TR_ID_VOLUMEN_TRABAJO

#### 1.1.2.5. Disparadores Modificados

##### • SOP_TR_ID_EQUIPO_ORD

##### • SOP_TR_ID_AREA

#### 1.1.2.6. Paquetes Creados

##### • SOP_PKG_CONDICIONES_FLUJO

##### • SOP_PKG_CONDICION_DEFI

##### • SOP_PKG_EMERGENCIA

##### • SOP_PKG_ESTADO

##### • SOP_PKG_FIRMA_USUARIO

##### • SOP_PKG_FLUJO_DETALLE_ALTERNO

##### • SOP_PKG_LIMITESDEINGRESO

##### • SOP_PKG_LOG_FILE

##### • SOP_PKG_MENSAJE_PERSONALIZADO

##### • SOP_PKG_TICKET_OMS

##### • SOP_PKG_TIPO_INSTALACION

##### • SOP_PKG_VALIDAR_ENVIO_BDI

##### • SOP_PKG_VOLUMEN_TRABAJO


#### 1.1.2.7. Paquetes Modificados

##### • SOP_PKG_REPORTE

##### • SOP_PKG_ORDEN_OPERACION

##### • SOP_PKG_SEG_ORDEN

##### • SOP_PKG_ANEXO_DESCONEX

##### • SOP_PKG_ANEXO_ORDEN

##### • SOP_PKG_AREA

##### • SOP_PKG_CIRCUITO_OP

##### • SOP_PKG_FLUJO_DETALLE

##### • SOP_PKG_MAIL

##### • SOP_PKG_ANEXO_CALIFICACION

##### • SOP_PKG_ANEXO_BDI

##### • SOP_PKG_ANEXO

##### • SOP_PKG_BACKLOG

## 2. SERVICIOS

### 1.2. FIRMAS

#### 1.2.1. Servidor de Reporting Services

```
Es necesario contar con un servidor de Reporting Services en donde se
almacene el reporte siguiente:
```
```
OrdenOp:
```

```
La ubicación del servidor de reportes y del servidor de imágenes se debe
definir en el archivo web.config (Para el caso de este ejemplo, el servidor de
reportes y el servidor de imágenes son el mismo SERVIDOR, pero podrían
variar):
```
```
<add key="FolderSharedUrl" value="http://SERVIDOR/" />
<add key="FolderShared" value="\\SERVIDOR\" />
<add key="REPORT_SERVER" value="http://SERVIDOR/ReportServer"></add>
```
#### 1.2.2. Acceso a carpeta compartida para guardado de firmas

```
Es necesario contar con un servidor web en donde se almacenen las
imágenes que representan las firmas digitales que ingresen los usuarios al
momento de autorizar órdenes o desde el mantenimiento de firmas:
```
```
Autorización:
```

Mantenimiento de Firmas:

Servidor Web:

Carpeta Compartida:
\\SERVIDOR\images


```
Consideración Especial:
En el servidor donde se almacenarán imágenes de las firmas, se debe
contemplar el permiso de lectura/escritura para el usuario del servidor
web. En el caso presentado anteriormente, tanto el servidor de Reporting
Services, como el Servidor Web, son el mismo.
```
```
En el caso en que los servidores sean diferentes, al usuario con el cual se
configure IIS, donde se instale la aplicación, debe brindar acceso de lectura-
escritura a la carpeta C:\IMAGES, al usuario de IIS dentro de ese servidor, y
permiso de lectura para todos los demás usuarios, debido a que las
imágenes deben ser accesibles vía web, para todos los usuarios del sistema
SOP.
```
### 1.3. CARPETA PARA GENERACIÓN DE LOGS

#### 1.3.1. Tarea Programada

```
Se ha implementado una tarea programada llamada
“CORREO_BDI_AUTOMATICO_JOB”, la cual necesita una carpeta en el
servidor de Base de Datos de Oracle donde se encuentre el esquema “SOP”.
```
```
Se recomienda que la carpeta se llame “C:\LOG_FILE”.
```

## 3. APLICACIÓN

### 1.4. MENU PRINCIPAL

#### 1.4.1. Elementos Creados

```
Se han agregado los elementos siguientes (con sus correspondientes
registros en la tabla “ORA_ASPNET_SITEMAP” del Esquema de Base de
Datos “SEC_USR”):
```
- Configuración:
    o Estado instalación.
    o Acciones por workflow.
    o Estados de Órdenes.
    o Firmas.
    o Mensajes de Correo.
    o Tipos BDI:
       ▪ Tipos de Instalación.
       ▪ Volumen de Trabajo.
       ▪ Emergencia.
    o Sincronizar Datos.
    o Condiciones Predefinidas.
- Reportes:
    o Visor de Trabajos Programados.
    o Planificación de Trabajos.
- Consulta BDI:
    o Datos Notificados BDI.
- Búsqueda de Órdenes.



