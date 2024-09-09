# Documentación del Proyecto ComerLogistics

## 1. Introducción
El proyecto ComerLogistics tiene como objetivo optimizar la gestión de inventarios y mejorar la trazabilidad de productos en una compañía de logística, mediante el uso de tecnologías avanzadas de análisis de datos. Se han implementado metodologías y herramientas que permiten un control integral de las operaciones comerciales, desde la adquisición y almacenamiento hasta la venta de productos. 

Para lograrlo, se han utilizado herramientas como **Python**, **SQL** y **Power BI**, integrando el análisis detallado de ventas, compras, y movimientos de inventario con el objetivo de mejorar la toma de decisiones estratégicas y operativas.

El enfoque ha sido diseñado para automatizar y optimizar el flujo de información, de modo que las decisiones relacionadas con los costos, la rotación de inventarios y la predicción de la demanda se tomen basadas en datos confiables y actualizados en tiempo real. Esto ha permitido la creación de **dashboards dinámicos** que facilitan la visualización de métricas críticas.

---

## 2. Configuración Inicial

### 2.1 Creación del Repositorio Público
**Acción Realizada:** Se creó un repositorio público en **GitHub** denominado **ComerLogistics**, el cual actúa como el núcleo colaborativo donde se alojan todos los scripts, notebooks y documentación necesaria para el desarrollo del proyecto. Este repositorio permite la interacción fluida entre los miembros del equipo, facilitando la revisión de código y el seguimiento de las modificaciones realizadas en tiempo real. 

El repositorio se puede encontrar en el siguiente enlace:  
[ComerLogistics - GitHub](https://github.com/Dapt01G2-Henry/ComerLogistics)

---

### 2.2 Estructura de Carpetas
**Acción Realizada:** Para mantener la organización del proyecto, se estructuró el repositorio con las siguientes carpetas:

- **DiagramaEntidadRelacion:** Contiene los diagramas ER (Entidad-Relación) que definen las relaciones entre las tablas principales de la base de datos.
- **Imágenes:** Almacena recursos visuales como logos, íconos y fondos utilizados en el proyecto.
- **Sprint_1:** Dentro de esta carpeta se encuentran los scripts y notebooks del proyecto, divididos en subcarpetas por funcionalidad:
    - **Conexion_SQL_Python:** Scripts relacionados con la conexión entre SQL y Python, permitiendo la automatización de los procesos de carga de datos.
    - **DataSet:** Contiene los archivos de datos utilizados en el proyecto. También incluye un archivo que referencia los datasets alojados en Google Drive.
    - **EDA y ETL:** Notebooks dedicados al análisis exploratorio de datos (EDA) y procesos de Extracción, Transformación y Carga (ETL).
    - **Web_Scraping:** Scripts utilizados para realizar scraping de sitios web, obteniendo datos adicionales necesarios para el análisis.
    - **Documentación.txt:** Archivo de texto que documenta cada paso realizado durante el desarrollo del proyecto.
---

## 3. Creación y Configuración de la Base de Datos

### 3.1 Creación de la Base de Datos
**Acción Realizada:** Se configuró una base de datos **SQL Server** llamada **COMERLOGISTICS**. Para interactuar con la base de datos desde Python, se utilizó **SQLAlchemy** y **PyODBC**, lo que permitió establecer una conexión robusta entre las aplicaciones. Esto facilita realizar operaciones **CRUD** (Create, Read, Update, Delete) en la base de datos y la manipulación de grandes volúmenes de información de manera automatizada.

---

### 3.2 Identificación de Entidades y Tablas
**Acción Realizada:** Tras un análisis exhaustivo de los datos y del modelo de negocio, se identificaron las principales entidades del sistema y las tablas correspondientes, entre las cuales se encuentran:

| Nombre Original             | Nombre Actual          |
| ----------------------------| -----------------------|
| **2017PurchasePricesDec**    | **Tabla_Producto**      |
| **BegInvFINAL12312016**      | **Tabla_InventarioInicial** |
| **EndInvFINAL12312016**      | **Tabla_InventarioFinal** |
| **InvoicePurchases12312016** | **Tabla_Compras**       |
| **PurchasesFINAL12312016**   | **Tabla_DetalleCompras**|
| **SalesFINAL12312016**       | **Tabla_VentasFinal**   |

- **Tabla_Compras:** Contiene el registro de todas las compras realizadas.
- **Tabla_DetalleCompras:** Incluye los detalles específicos de cada compra, como los productos adquiridos y sus respectivas cantidades.
- **Tabla_InventarioInicial:** Representa el inventario al inicio del período de análisis.
- **Tabla_InventarioFinal:** Representa el inventario al final del período de análisis.
- **Tabla_Producto:** Contiene información detallada de cada producto gestionado por la compañía.
- **Tabla_VentasFinal:** Registra todas las ventas realizadas.

---

### 3.3 Creación de Tablas y Objetos SQL
**Acción Realizada:** Se crearon las tablas mencionadas anteriormente en la base de datos **SQL Server**. Las relaciones entre las tablas fueron definidas mediante el uso de claves primarias y foráneas, con base en el modelo de datos en **copo de nieve**, seleccionado para facilitar las consultas y mejorar el rendimiento del sistema.

Los diagramas ER en la carpeta **DiagramaEntidadRelacion** muestran claramente cómo estas tablas se relacionan entre sí, permitiendo un fácil acceso y comprensión del modelo.

---

## 4. Flujo de Ingesta de Datos

### 4.1 Extracción, Transformación y Carga de Datos (ETL)
**Acción Realizada:** Se implementó un proceso **ETL** utilizando **Python**. Este proceso fue desarrollado y documentado en el notebook **EDA y ETL.ipynb** y se divide en las siguientes fases:

- **Extracción:** Lectura de archivos de datos en diferentes formatos (principalmente CSV), transformando y normalizando la información.
- **Transformación:** Incluye el manejo de valores nulos, la limpieza de datos y la realización de operaciones aritméticas para asegurar la calidad de los datos. Se establecieron estándares en el formato de fechas y se unificaron tipos de datos en todas las columnas.
- **Carga:** Los datos transformados fueron cargados en la base de datos **SQL Server** a través de la conexión establecida previamente.

---

### 4.2 Validación del Proceso
**Acción Realizada:** Para asegurar la calidad del proceso, se realizaron pruebas de acceso para todos los miembros del equipo. Se verificó que el proceso **ETL** funcionara de forma fluida y sin interrupciones, garantizando que los datos fueran cargados de forma correcta y sin duplicaciones.

---
## 5. Automatización de la Ingesta de Datos Nuevos

### 5.1 Implementación de la Automatización
**Acción Realizada:** Se creó un script automatizado en Python (disponible en el notebook [AutomatizacionDatosNuevos.ipynb](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/be299b2f53546f7104b273e4f546a02a9e0b3559/Sprint_1/Conexion_SQL_Python/AutomatizacionDatosNuevos.ipynb)) para realizar la ingesta incremental de nuevos datos. Este script se encarga de verificar los registros ya existentes en la base de datos y agregar solo los nuevos, evitando duplicidades.

---

### 5.2 Ejecución Automática
**Acción Realizada:** Para garantizar la actualización constante de los datos, se programó un script `.bat` que es ejecutado automáticamente por el Task Scheduler de Windows semanalmente. Este archivo ejecuta el script de Python en los intervalos programados.

---

### 5.3 Validación y Monitorización
**Acción Realizada:** Se realizaron pruebas para verificar la ejecución correcta del proceso automatizado, asegurándose de que no hubiera duplicados y que todos los datos nuevos fueran ingresados correctamente en la base de datos.

---

## 6. Análisis Exploratorio y Transformación de Datos (EDA)

### 6.1 Análisis Exploratorio
**Acción Realizada:** Se realizó un análisis exhaustivo de los datos mediante los notebooks [EDA y ETL.ipynb](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/4af09eba8ed8b2a3f9a07d60f767dfc9b4cbb47d/Sprint_1/EDA%20y%20ETL) y [AnalisisTablas.ipynb](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/Sprint_1/EDA%20y%20ETL/AnalisisTablas.ipynb), donde se exploraron distribuciones, se detectaron valores atípicos (outliers), y se identificaron tendencias clave en los datos.

---

### 6.2 Transformación y Limpieza
**Acción Realizada:** Durante el proceso de transformación, los datos fueron formateados y preparados para ser cargados en la base de datos y utilizados en los informes. Se aplicaron procedimientos de limpieza para eliminar errores, normalizar los datos y enriquecer los registros con información relevante.

---

## 7. Visualización de Datos y Dashboard en Power BI

### 7.1 Diseño del Dashboard
**Acción Realizada:** Se diseñó un dashboard interactivo en Power BI, el cual permite visualizar de forma dinámica las ventas, inventarios y otras métricas clave de la compañía. Este dashboard fue pensado para proporcionar una narrativa clara del rendimiento de **ComerLogistics**, destacando las áreas de oportunidad en la gestión de inventarios. Puedes acceder al archivo del dashboard en [ComerLogistics.pbix](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/be299b2f53546f7104b273e4f546a02a9e0b3559/Sprint_2/ComerLogistics.pbix).

---

### 7.2 Funcionalidades del Dashboard
**Acción Realizada:** El dashboard incluye una variedad de gráficos interactivos, como gráficos de barras y líneas de tendencia, además de tablas dinámicas. También cuenta con segmentadores y filtros que permiten a los usuarios ajustar la visualización de los datos en tiempo real, analizando los inventarios y ventas por ciudad, tienda o producto.

---

### 7.3 Interactividad y Análisis
**Acción Realizada:** Se añadieron funcionalidades interactivas que permiten desglosar los datos hasta el nivel más detallado, facilitando a los usuarios realizar análisis en tiempo real y tomar decisiones basadas en datos. Estas funcionalidades ayudan a los responsables de la gestión del inventario a visualizar patrones y tendencias de compra.

---

## 8. Conclusión y Próximos Pasos

### 8.1 Conclusión
Se ha implementado un sistema integral que abarca desde la ingesta de datos hasta la visualización de los resultados en dashboards interactivos.  
El sistema desarrollado para **ComerLogistics** ha permitido optimizar la gestión de inventarios, la trazabilidad de productos y la toma de decisiones estratégicas mediante la automatización de procesos. Gracias a la integración de herramientas como **Python**, **SQL** y **Power BI**, se ha logrado crear un flujo continuo de datos desde la extracción hasta la visualización, lo cual mejora significativamente la capacidad de análisis y predicción de la compañía.

Además, la automatización en la ingesta de nuevos datos garantiza que el sistema se mantenga actualizado sin intervención manual, lo que proporciona un alto nivel de confianza en la información presentada. Los dashboards en **Power BI** ofrecen una visión clara y concisa de los datos críticos, permitiendo a los usuarios interactuar con la información y tomar decisiones informadas basadas en las métricas clave.

---

### 8.2 Próximos Pasos
A continuación, se describen los próximos pasos recomendados para seguir optimizando y expandiendo el proyecto **ComerLogistics**:

- **Refinamiento del Pipeline de Datos:** Continuar optimizando el flujo de ingesta y transformación de datos para mejorar la eficiencia y reducir los tiempos de procesamiento. Se puede explorar el uso de tecnologías adicionales como **Apache Spark** para manejar grandes volúmenes de datos de manera más rápida y eficiente.

- **Implementación de Alertas de Anomalías:** Integrar un sistema de alertas automáticas en tiempo real para detectar irregularidades o anomalías en los inventarios o ventas. Esto permitiría actuar de manera preventiva ante posibles problemas en la cadena de suministro o gestionar la reposición de productos con mayor efectividad.

- **Mejora de las Visualizaciones en Power BI:** Incorporar nuevos tipos de visualizaciones avanzadas que proporcionen mayor profundidad en el análisis, como gráficos de dispersión y matrices de correlación. Adicionalmente, se puede mejorar el diseño del dashboard para hacerlo aún más intuitivo y amigable para los usuarios.

- **Integración con Machine Learning:** Implementar modelos predictivos basados en **Machine Learning** para anticipar tendencias de venta y demanda, lo que permitirá una planificación más precisa del inventario y la optimización de los niveles de stock. Esto podría ayudar a mejorar la rotación de inventarios y reducir costos asociados a productos obsoletos o sobrestock.

- **Pruebas de Calidad del Informe y Presentación del Sprint 2:** Llevar a cabo una validación exhaustiva de la funcionalidad y precisión del dashboard, asegurándose de que los cálculos y visualizaciones sean correctos. Posteriormente, realizar la presentación formal del Sprint 2, donde se mostrará todo el trabajo realizado hasta el momento, con énfasis en la visualización de datos y las decisiones estratégicas que se pueden tomar con la información proporcionada.

- **Documentación Detallada del Proyecto:** Mantener actualizada la documentación del proyecto, detallando cada fase del desarrollo y asegurando que toda la información sobre el flujo de trabajo esté disponible para futuras referencias.

- **Capacitación de Usuarios:** Realizar sesiones de capacitación para los usuarios finales del dashboard, ayudándoles a comprender las funcionalidades disponibles y cómo interpretar los datos para tomar decisiones efectivas.

_____

# Informe del Sprint 2 - ComerLogistics


## Objetivo
El objetivo del **Sprint 2** en el proyecto **ComerLogistics** fue la creación y desarrollo de un archivo `.pbix` en Power BI que permitiera analizar y visualizar datos de inventarios, ventas, compras y productos. El enfoque principal incluyó la importación de datos, limpieza y transformación, la creación de relaciones entre las tablas, la definición de medidas personalizadas utilizando DAX y el diseño de reportes visuales que ofrecieran una vista clara de las métricas clave del negocio.

El resultado final es un panel de control interactivo que proporciona a los usuarios una comprensión profunda de las operaciones comerciales, lo que facilita la toma de decisiones estratégicas.

## 1. Creación del archivo .pbix
El archivo central del proyecto fue creado en **Power BI Desktop** y almacenado como **ComerLogistics.pbix**. Este archivo contendrá todas las fuentes de datos, transformaciones y visualizaciones desarrolladas a lo largo del proyecto.

### Especificaciones Técnicas:
- **Formato:** .pbix
- **Software utilizado:** Power BI Desktop
- **Versión de Power BI Desktop:** [Especificar la versión]
- **Estructura de carpetas:** El archivo fue almacenado en el repositorio del equipo en **GitHub**, siguiendo una estructura ordenada para facilitar el acceso.
  - Carpeta del sprint: `/Sprint_2/`
  - Nombre del archivo: **ComerLogistics.pbix**

Este archivo actuará como el contenedor principal de todos los datos y análisis a lo largo del desarrollo del proyecto.

## 2. Importación de los datos
Los datos fueron importados a Power BI desde archivos **CSV**. Se seleccionaron seis fuentes de datos críticas para el análisis del inventario y las ventas de la empresa.

### Archivos importados:
- **BegInvFINAL12312016.csv**: Datos de inventario inicial.
- **EndInvFINAL12312016.csv**: Datos de inventario final.
- **PurchasesFINAL12312016.csv**: Datos de compras.
- **SalesFINAL12312016.csv**: Datos de ventas.
- **2017PurchasePricesDec.csv**: Precios de los productos en el inventario.
- **InvoicePurchases12312016.csv**: Datos de facturación de compras.

### Especificaciones del proceso de importación:
- Se utilizó la función **Obtener datos** en Power BI.
- Todos los archivos fueron revisados antes de la importación para asegurar que estuvieran completos y en el formato adecuado.
- Los archivos fueron cargados como tablas independientes, cada una con su propio conjunto de campos.
- Se verificó que no hubiera conflictos de tipos de datos ni problemas de formato, asegurando la integridad de los datos desde la importación.

## 3. Limpieza y transformación de datos
Una vez importados los datos, se procedió a realizar un proceso exhaustivo de limpieza y transformación. Esto es esencial para garantizar la calidad de los datos y facilitar un análisis preciso.

### Proceso de transformación:
- **Revisión de tipos de datos:** Cada columna fue revisada para asegurarse de que tuviera el tipo de datos correcto (números enteros, decimales, fechas, texto, etc.).
- **Tratamiento de valores nulos:** Se identificaron y corrigieron los valores faltantes o nulos. Por ejemplo, se observó que algunas columnas de ciudades tenían datos faltantes en el inventario final, por lo que se implementaron reglas para manejar dichos valores.
- **Renombrado de columnas:** Las columnas fueron renombradas según la convención acordada en el proyecto. Ejemplo:
  - `Brand` -> `MarcaID`
  - `SalesDollars` -> `Venta_Total`
- **Eliminación de duplicados:** Se eliminaron filas duplicadas en los archivos que lo requerían, específicamente en las tablas de compras y ventas.
- **Creación de columnas calculadas:** Se añadieron columnas adicionales donde fue necesario para facilitar análisis posteriores.

### Detalle de cambios realizados:
- **Inventario inicial:** Se ajustaron las descripciones de productos y se verificaron las fechas para asegurar que correspondieran con el período bajo análisis.
- **Compras y ventas:** Se unificaron los formatos de las fechas y se corrigieron discrepancias en la nomenclatura de productos.

## 4. Creación de relaciones, medidas y columnas calculadas
El siguiente paso fue establecer las relaciones entre las tablas para permitir un análisis cruzado, y se crearon medidas personalizadas mediante **DAX** para cálculos avanzados.

### Relaciones establecidas:
- La tabla **SalesFINAL12312016.csv** (Ventas) se relacionó con la tabla **BegInvFINAL12312016.csv** (Inventario inicial) y la tabla **EndInvFINAL12312016.csv** (Inventario final) a través de las columnas `MarcaID` y `Tienda`.
- La tabla **PurchasesFINAL12312016.csv** (Compras) también se conectó a las tablas de inventario y ventas para permitir un análisis holístico del flujo de inventario.

### Medidas creadas con DAX:
- **TotalVentas:** Suma de las ventas totales de cada tienda utilizando la columna `Venta_Total` de la tabla de ventas.
  ```DAX
  TotalVentas = SUM(SalesFINAL[Venta_Total])

_____