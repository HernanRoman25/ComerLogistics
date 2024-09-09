# Entregables Sprint 1 

## 1. Crear el repositorio público y compartirlo con el equipo

### Descripción:
Uno de los pasos iniciales y fundamentales para la correcta organización del proyecto fue la creación de un repositorio público en GitHub, donde se centralizan todas las actividades de desarrollo y colaboración entre los miembros del equipo. Este repositorio funciona como el espacio de trabajo colaborativo en el que se almacenan todos los recursos del proyecto, incluidos scripts, notebooks, documentación, imágenes, y demás elementos necesarios para el correcto avance del proyecto.

Además, la implementación de control de versiones es esencial en un entorno colaborativo. GitHub permite el seguimiento de los cambios realizados en el código y la documentación, lo que asegura que todos los integrantes del equipo estén trabajando siempre con la versión más actualizada de los archivos y que se pueda retroceder a versiones anteriores en caso de errores.

### Acciones realizadas:

- **Creación del Repositorio en GitHub:**
   Se decidió utilizar GitHub como plataforma para alojar el repositorio debido a su amplia adopción en el ámbito profesional y sus funcionalidades de control de versiones, colaboración en tiempo real, y su integración con herramientas de desarrollo como Visual Studio Code. El repositorio fue creado bajo el nombre **ComerLogistics**, accesible en el siguiente enlace: [**ComerLogistics**](https://github.com/Dapt01G2-Henry/ComerLogistics). Desde este punto, todos los miembros del equipo fueron invitados como colaboradores para asegurar el acceso adecuado.

- **Configuración de Permisos de Acceso:**
   Se configuraron los permisos adecuados para garantizar que todos los miembros del equipo puedan clonar, modificar y contribuir activamente al repositorio. Cada colaborador cuenta con los permisos necesarios para realizar operaciones como *pull requests*, revisiones de código, y reportar *issues*. Esta estructura de permisos asegura un flujo de trabajo fluido y controlado, permitiendo a los líderes del proyecto aprobar o rechazar cambios críticos.

- **Control de Versiones:**
   La utilización de GitHub como sistema de control de versiones ha permitido a los desarrolladores mantener un historial detallado de todas las modificaciones realizadas. Esto facilita la identificación de cambios específicos, quién los realizó y cuándo se llevaron a cabo. Además, se han creado ramas (*branches*) para la experimentación y pruebas, lo que garantiza que el código en la rama principal (*main*) esté siempre en un estado funcional y estable.

   El uso de *pull requests* ha sido fundamental para asegurar que cualquier nuevo código o modificación sea revisado por otros miembros del equipo antes de ser fusionado en la rama principal. Esto también ha permitido una mayor colaboración, ya que los desarrolladores pueden comentar sobre los cambios, realizar revisiones de calidad y sugerir mejoras antes de que los cambios se hagan permanentes.

- **Documentación Inicial:**
   Se creó un archivo `README.md` que actúa como la página de inicio del repositorio. Este archivo proporciona información clave sobre el proyecto, como su propósito, cómo clonar el repositorio, y las instrucciones iniciales para la configuración del entorno de desarrollo. Además, incluye enlaces a los principales archivos y carpetas del proyecto, lo que facilita a los nuevos miembros del equipo la comprensión de la estructura del repositorio y el acceso a los recursos. Este archivo se actualiza periódicamente para reflejar el estado actual del proyecto y cualquier cambio relevante.

- **Estructura del Repositorio:**
   Para mantener una organización clara y accesible de los recursos del proyecto, se definió una estructura de carpetas desde el inicio. Las principales carpetas creadas dentro del repositorio incluyen:

   - **DiagramaEntidadRelacion:** Esta carpeta contiene los diagramas ER (Entidad-Relación) que definen las relaciones entre las tablas principales de la base de datos. [Ver carpeta](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/4af09eba8ed8b2a3f9a07d60f767dfc9b4cbb47d/DiagramaEntidadRelacion).
   
   - **Imágenes:** Se almacenan los recursos gráficos necesarios, como logotipos, iconos, y gráficos utilizados en la documentación y visualización de datos. [Ver carpeta](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/4af09eba8ed8b2a3f9a07d60f767dfc9b4cbb47d/Imagenes).

   - **Sprint_1:** Dentro de esta carpeta se organizan todos los scripts y notebooks utilizados durante el primer sprint del proyecto. Entre las subcarpetas más destacadas se encuentran:
      - **Conexion_SQL_Python:** Scripts relacionados con la conexión entre la base de datos SQL y Python. Esta conexión es fundamental para la automatización del flujo de datos. [Ver carpeta](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/be299b2f53546f7104b273e4f546a02a9e0b3559/Sprint_1/Conexion_SQL_Python).
      - **DataSet:** Contiene los archivos de datos utilizados durante el desarrollo del proyecto. Estos archivos fueron procesados y transformados para su carga en la base de datos SQL Server. [Ver carpeta](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/be299b2f53546f7104b273e4f546a02a9e0b3559/Sprint_1/DataSet).
      - **EDA y ETL:** Notebooks donde se realizó el análisis exploratorio de los datos (EDA) y el proceso de Extracción, Transformación y Carga (ETL), fundamental para asegurar la calidad de los datos antes de su análisis. [Ver carpeta](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/4af09eba8ed8b2a3f9a07d60f767dfc9b4cbb47d/Sprint_1/EDA%20y%20ETL).
      - **Web_Scraping:** Carpeta que almacena los scripts desarrollados para la obtención de datos adicionales a través de scraping web, complementando el dataset principal con información relevante. [Ver carpeta](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/4af09eba8ed8b2a3f9a07d60f767dfc9b4cbb47d/Web_Scraping).

- **Colaboración y Seguimiento del Proyecto:**
   A lo largo del proyecto, se utilizaron herramientas de seguimiento de issues y tareas proporcionadas por GitHub, lo que permitió llevar un control detallado de los avances del equipo, los obstáculos encontrados y las soluciones implementadas. Cada tarea asignada a los miembros del equipo estaba relacionada con un issue específico, lo que garantizó una adecuada trazabilidad y resolución de problemas.

- **Integración con Visual Studio Code:**
   Todo el equipo de desarrollo sincronizó el repositorio con **Visual Studio Code**, lo que facilitó la edición y el manejo de código en tiempo real. Esta integración permitió realizar *commits* directamente desde el entorno de desarrollo y mantener un flujo de trabajo ágil.

### Resultado Final:
Gracias a la creación del repositorio público y su adecuada configuración, el equipo ha logrado trabajar de manera colaborativa y eficiente. El control de versiones ha sido clave para asegurar que el desarrollo se realice de manera estructurada, mientras que la organización del repositorio ha permitido un fácil acceso a todos los recursos y archivos necesarios para el desarrollo del proyecto.

_____

## 2. Identificar los archivos a usar y armar la estructura de carpetas a usar en el repositorio

### Descripción:

En esta etapa inicial del proyecto, fue crucial realizar una identificación clara y precisa de los archivos de datos que se utilizarían para llevar a cabo el análisis y las operaciones de inventario, compras y ventas. La correcta identificación y organización de estos archivos permiten un flujo de trabajo eficiente y minimizan el riesgo de errores durante el desarrollo.

Además, se definió una estructura de carpetas en el repositorio que facilitara la colaboración entre los miembros del equipo, organizando los archivos de forma lógica y asegurando que cada sección del proyecto tuviera su propio espacio dentro del repositorio. Este enfoque garantiza que los desarrolladores puedan trabajar en diferentes aspectos del proyecto sin interferencias, manteniendo una separación clara entre scripts, datos, documentación y otros recursos.

### Acciones realizadas:

1. **Identificación de Archivos del DataSet Original:**
   El equipo comenzó con una revisión exhaustiva de todos los archivos disponibles en el dataset original proporcionado por la empresa. Estos archivos contenían información crítica sobre compras, ventas, productos y movimientos de inventario. Se realizó un análisis detallado de los archivos, y se procedió a renombrarlos para reflejar su propósito en el contexto del proyecto. Los archivos identificados fueron:

   - **Archivo Original:** `2017PurchasePricesDec` → **Nombre Actual:** `Tabla_Producto`
   - **Archivo Original:** `BegInvFINAL12312016` → **Nombre Actual:** `Tabla_InventarioInicial`
   - **Archivo Original:** `EndInvFINAL12312016` → **Nombre Actual:** `Tabla_InventarioFinal`
   - **Archivo Original:** `InvoicePurchases12312016` → **Nombre Actual:** `Tabla_Compras`
   - **Archivo Original:** `PurchasesFINAL12312016` → **Nombre Actual:** `Tabla_DetalleCompras`
   - **Archivo Original:** `SalesFINAL12312016` → **Nombre Actual:** `Tabla_VentasFinal`

2. **Revisión de Estructura y Tipos de Datos:**
   Tras la identificación de los archivos, se realizó una revisión exhaustiva de su estructura. El objetivo era asegurar que los tipos de datos fueran correctos y que las columnas estuvieran bien definidas. Se validaron aspectos como:

   - **Fechas:** Se revisaron los formatos de fecha para asegurarse de que fueran uniformes en todos los archivos.
   - **Claves Primarias y Foráneas:** Se identificaron los campos que servirían como claves primarias y foráneas para vincular las tablas entre sí.
   - **Consistencia de las Unidades:** Se verificó que las unidades de medida (como las cantidades de productos en inventario o vendidas) fueran consistentes en todos los archivos.

3. **Transformación de los Datos:**
   Se realizó un proceso de transformación para adecuar los datos a las necesidades del proyecto. Este proceso incluyó la normalización de los nombres de las columnas y la conversión de tipos de datos para facilitar su análisis posterior. Los detalles de esta transformación se documentaron en el notebook **EDA y ETL.ipynb**, donde cada archivo fue procesado, limpiado y preparado para ser cargado en la base de datos.

4. **Estructura de Carpetas en el Repositorio:**
   Una vez identificados y transformados los archivos, se definió una estructura de carpetas en el repositorio para organizar los diferentes aspectos del proyecto. La estructura establecida fue la siguiente:

   - **Sprint_1:**
     - **Conexion_SQL_Python:** Contiene scripts para la conexión entre SQL y Python.
     - **DataSet:** Almacena los archivos de datos originales y procesados.
     - **EDA y ETL:** Contiene notebooks para análisis exploratorio de datos (EDA) y transformación (ETL).
     - **Web_Scraping:** Scripts para obtener datos adicionales mediante scraping.
   
   - **DiagramaEntidadRelacion:** Contiene diagramas ER para las relaciones entre las tablas.
     - [Ver carpeta de Diagrama ER](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/4af09eba8ed8b2a3f9a07d60f767dfc9b4cbb47d/DiagramaEntidadRelacion).

5. **Documentación de Archivos y Procesos:**
   A medida que se iban identificando y procesando los archivos, se documentaron los pasos en el archivo `Documentación.md`. Este archivo contiene un registro detallado de cada paso realizado durante el desarrollo del proyecto.

### Resultado Final:

La identificación precisa de los archivos y la estructuración lógica de las carpetas en el repositorio han sido fundamentales para garantizar la fluidez del proyecto. Gracias a esta organización, el equipo pudo realizar un análisis profundo y coherente de los datos.

### Enlaces Relacionados:
- [Repositorio ComerLogistics en GitHub](https://github.com/Dapt01G2-Henry/ComerLogistics)
- [Carpeta DataSet en el Repositorio](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/be299b2f53546f7104b273e4f546a02a9e0b3559/Sprint_1/DataSet)
- [EDA y ETL Notebooks](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/4af09eba8ed8b2a3f9a07d60f767dfc9b4cbb47d/Sprint_1/EDA%20y%20ETL)

_____

## 3. Creación de la Base de Datos

### 3.1 Creación de la Base de Datos

**Descripción:**

La base de datos es el pilar fundamental sobre el cual se desarrolló todo el sistema de análisis de datos para **ComerLogistics**. En este proyecto, se optó por usar **SQL Server** como gestor de bases de datos por su robustez y capacidad para manejar grandes volúmenes de datos transaccionales.

El enfoque inicial fue crear una estructura de base de datos que permitiera almacenar de forma eficiente los datos de inventarios, compras y ventas, manteniendo una trazabilidad clara de cada operación realizada en el sistema. Se buscó una arquitectura que permitiera realizar consultas rápidas y eficaces, que brindaran insights útiles para la toma de decisiones.

#### Acciones Realizadas:

1. **Configuración del entorno SQL Server:**
   Se configuró un servidor de bases de datos utilizando **SQL Server**, asegurando que estuviera optimizado para realizar cargas de datos masivas y consultas complejas. La configuración inicial incluyó la instalación del servidor, la creación de usuarios y la configuración de permisos adecuados para los diferentes miembros del equipo de desarrollo y análisis.

2. **Creación de la base de datos `COMERLOGISTICS`:**
   Posteriormente, se creó una base de datos llamada **COMERLOGISTICS**. Esta base de datos fue diseñada para gestionar las tablas que contienen datos relacionados con el inventario, las compras y las ventas de productos, además de otras métricas clave.

3. **Conexión a la base de datos desde Python:**
   Se utilizó **SQLAlchemy** y **PyODBC** como intermediarios para establecer una conexión entre Python y SQL Server, lo que permitió integrar el procesamiento y análisis de datos con Python, así como la manipulación y consulta de los mismos directamente desde notebooks en **Jupyter**. Esta conexión facilitó la automatización de procesos que involucraban la manipulación de datos en la base de datos.

   - **SQLAlchemy:** Biblioteca de Python utilizada para la interacción con SQL Server, proporcionando una interfaz para la manipulación de datos y la ejecución de consultas.
   - **PyODBC:** Módulo que facilita la conexión a bases de datos SQL Server desde Python, utilizado en la configuración de las cadenas de conexión y en el manejo de las consultas SQL.

#### Enlaces Relacionados:
- [Carga_Datos_Finales_a_SQL.ipynb](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/Sprint_1/Conexion_SQL_Python/Carga_Datos_Finales_a_SQL.ipynb)

---

### 3.2 Identificación de Entidades y Tablas

**Descripción:**

La correcta identificación de las entidades y tablas fue crucial para el éxito del proyecto, ya que esto permitió la creación de un modelo de datos que reflejara con precisión las necesidades operativas y analíticas de **ComerLogistics**. Durante este proceso, se analizaron todos los aspectos del negocio, desde las compras hasta las ventas y la gestión de inventarios.

#### Acciones Realizadas:

1. **Análisis de las Operaciones del Negocio:**
   El equipo realizó un análisis exhaustivo de las operaciones de la empresa para determinar las entidades clave que debían ser modeladas en la base de datos. Se identificaron las operaciones críticas que afectan el inventario, tales como las compras y ventas, y se estableció un modelo de datos adecuado para almacenarlas.

2. **Entidades Identificadas:**
   A partir de este análisis, se identificaron las siguientes tablas principales, que cubren las necesidades de la empresa:

   - **Tabla_Compras:** Registra las compras realizadas por la empresa. Incluye información detallada sobre las transacciones con los proveedores.
   - **Tabla_DetalleCompras:** Registra los detalles de cada compra, desglosando las cantidades de productos comprados.
   - **Tabla_InventarioInicial:** Contiene los registros de los niveles de inventario al inicio del período analizado.
   - **Tabla_InventarioFinal:** Contiene los registros de los niveles de inventario al final del período analizado.
   - **Tabla_Producto:** Proporciona información detallada sobre cada producto, como la descripción y el precio.
   - **Tabla_VentasFinal:** Contiene las ventas realizadas por la empresa.

3. **Renombrado de Archivos y Normalización de Columnas:**
   Los archivos que inicialmente fueron proporcionados en el dataset original se renombraron para alinearse con las convenciones de nombres utilizados en la base de datos. Se revisaron y normalizaron las columnas de estos archivos para asegurar una integración sin problemas.

   - **2017PurchasePricesDec** → `Tabla_Producto`
   - **BegInvFINAL12312016** → `Tabla_InventarioInicial`
   - **EndInvFINAL12312016** → `Tabla_InventarioFinal`
   - **InvoicePurchases12312016** → `Tabla_Compras`
   - **PurchasesFINAL12312016** → `Tabla_DetalleCompras`
   - **SalesFINAL12312016** → `Tabla_VentasFinal`

4. **Diagrama Entidad-Relación (ER):**
   Para visualizar las relaciones entre las diferentes tablas, se generó un **Diagrama Entidad-Relación** (ER) que muestra cómo interactúan entre sí las entidades. Este diagrama fue clave para entender las dependencias y asegurarse de que el modelo de datos fuera coherente y eficiente.

   - [Ver Diagrama ER](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/4af09eba8ed8b2a3f9a07d60f767dfc9b4cbb47d/DiagramaEntidadRelacion)

---

### 3.3 Creación de Tablas y Objetos SQL

**Descripción:**

Una vez definidas las entidades clave, el siguiente paso fue la creación de las tablas en **SQL Server**. Cada tabla fue diseñada para reflejar la estructura de las entidades previamente identificadas. Se aplicaron reglas de normalización para evitar redundancias de datos y asegurar que cada tabla se mantuviera consistente con el modelo de datos establecido.

#### Acciones Realizadas:

1. **Definición de Estructura de Tablas:**
   Se definieron las columnas de cada tabla, asegurando que cada una incluyera la información relevante para el análisis. Se asignaron **tipos de datos** adecuados para cada columna, lo que permitió mejorar el rendimiento en las consultas y operaciones de base de datos.

2. **Implementación de Claves Primarias y Foráneas:**
   Se implementaron claves primarias en cada tabla para identificar de forma única los registros, y se establecieron claves foráneas para asegurar la integridad referencial entre las tablas. Esta relación permitió realizar consultas complejas que involucraban múltiples tablas, manteniendo la consistencia de los datos.

3. **Creación de Objetos SQL:**
   Adicionalmente, se crearon **índices** en las tablas más consultadas para mejorar el rendimiento de las consultas y facilitar el acceso a los datos de manera más rápida y eficiente. También se implementaron **vistas** para proporcionar una visión consolidada de los datos de inventario y ventas.

   El proceso de creación de estas tablas y objetos SQL fue documentado en el notebook **Carga_Datos_Finales_a_SQL.ipynb**.

#### Enlaces Relacionados:
- [Carga_Datos_Finales_a_SQL.ipynb](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/Sprint_1/Conexion_SQL_Python/Carga_Datos_Finales_a_SQL.ipynb)

_____


## Punto 4: Identificar las entidades/tablas a usar en la BD

**Descripción:**

El éxito del proyecto depende en gran medida de la correcta identificación de las entidades y tablas que reflejan las operaciones comerciales de **ComerLogistics**. En esta etapa, se llevó a cabo un análisis exhaustivo de los datos proporcionados por la empresa, con el objetivo de modelar el sistema de información a través de una base de datos robusta y eficiente que permitiera gestionar de forma adecuada los datos de inventarios, ventas y compras.

### Acciones Realizadas:

1. **Análisis de Datos y Procesos Operativos:**
   Se comenzó con un estudio detallado de las operaciones diarias de **ComerLogistics**, enfocándose en los procesos críticos de la empresa como el ciclo de compra-venta, la gestión de inventarios y la rotación de productos. El objetivo era asegurarse de que cada entidad de la base de datos representara un aspecto clave del negocio.

2. **Definición de las Entidades:**
   Se identificaron las principales entidades que serían modeladas en la base de datos, basadas en los datos proporcionados. Las entidades principales son:
   - **Productos:** Representa cada uno de los artículos que **ComerLogistics** gestiona, con información como marca, descripción y precio.
   - **Compras:** Contiene los registros de las transacciones realizadas para abastecer los inventarios.
   - **Ventas:** Almacena los registros de todas las ventas, detallando los productos vendidos, las cantidades y las tiendas involucradas.
   - **Inventario Inicial y Final:** Representan los niveles de inventario en un momento específico, permitiendo hacer un seguimiento de la evolución del stock.

3. **Tablas de Base de Datos Derivadas:**
   Una vez identificadas las entidades, se procedió a definir las tablas que albergarían los datos de estas entidades en la base de datos. Las principales tablas son:
   - **Tabla_Producto:** Que almacena información detallada sobre cada producto.
   - **Tabla_Compras:** Almacena las compras realizadas y las transacciones con proveedores.
   - **Tabla_DetalleCompras:** Almacena el desglose de las compras, especificando los productos adquiridos y las cantidades.
   - **Tabla_InventarioInicial y Tabla_InventarioFinal:** Registran los niveles de inventario al inicio y al final de cada periodo.
   - **Tabla_VentasFinal:** Registra todas las ventas realizadas por la empresa, detallando productos, cantidades y montos.

4. **Análisis de Dependencias y Relaciones:**
   Durante este proceso, se analizaron las dependencias entre las diferentes entidades, lo cual ayudó a definir las relaciones que debían existir entre las tablas. Esto incluye las relaciones entre productos y compras, entre productos y ventas, y entre compras y detalles de compras. Se definieron claves primarias y foráneas para asegurar la integridad de los datos, permitiendo un fácil acceso y consulta a través de SQL.

5. **Uso de Diagrama ER (Entidad-Relación):**
   Con el fin de visualizar mejor las relaciones entre las tablas y validar la estructura del sistema, se creó un **Diagrama Entidad-Relación (ER)**. Este diagrama no solo facilita la comprensión del modelo de datos por parte del equipo de desarrollo, sino que también proporciona una representación clara para futuras consultas y mejoras en el sistema.

### Enlaces Relacionados:
- [Identificación de Entidades y Tablas en el Proyecto](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/Sprint_1/DataSet/DataSets%20en%20Drive.txt)
- [Diagrama ER](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/4af09eba8ed8b2a3f9a07d60f767dfc9b4cbb47d/DiagramaEntidadRelacion)

_____

## Punto 5: Crear las tablas y objetos SQL necesarios

**Descripción:**

Una vez identificadas las entidades principales y las tablas necesarias, el siguiente paso fue implementar estas tablas en la base de datos **SQL Server**. Este proceso incluyó la definición detallada de las columnas de cada tabla, así como la configuración de relaciones mediante claves foráneas, asegurando la integridad referencial de los datos.

### Acciones Realizadas:

1. **Definición de Estructura de Tablas:**
   Se definieron las tablas en **SQL Server** utilizando las entidades previamente identificadas. Cada tabla fue cuidadosamente diseñada para almacenar los datos clave de **ComerLogistics**, respetando la normalización y asegurando que cada entidad reflejara adecuadamente los procesos de negocio.

   - **Tabla_Producto:** Almacena la información esencial de cada producto, como el nombre, marca, tamaño y precio.
   - **Tabla_Compras:** Registra cada transacción de compra realizada, permitiendo rastrear las fechas de compra y los proveedores.
   - **Tabla_DetalleCompras:** Registra los detalles de cada compra, desglosando los productos comprados y las cantidades.
   - **Tabla_InventarioInicial y Tabla_InventarioFinal:** Estas tablas almacenan los registros de los inventarios al inicio y al final del periodo, respectivamente.
   - **Tabla_VentasFinal:** Registra todas las ventas, proporcionando información detallada sobre las transacciones realizadas con los clientes.

2. **Configuración de Claves Primarias y Foráneas:**
   Para asegurar la integridad de los datos, cada tabla fue configurada con **claves primarias** que garantizan la unicidad de los registros. Adicionalmente, se configuraron **claves foráneas** que aseguran la relación entre diferentes tablas, como la relación entre productos y compras, o entre productos y ventas.

3. **Creación de Vistas e Índices:**
   Con el objetivo de mejorar el rendimiento y facilitar las consultas frecuentes, se crearon **vistas** que permiten tener acceso rápido a datos de múltiples tablas a la vez. Además, se crearon **índices** en las tablas más consultadas, lo que permitió optimizar las consultas y reducir los tiempos de respuesta al ejecutar operaciones en la base de datos.

4. **Documentación del Proceso SQL:**
   Todas las operaciones relacionadas con la creación de las tablas, claves y vistas fueron documentadas en el notebook **Carga_Datos_Finales_a_SQL.ipynb**, el cual detalla paso a paso la creación de las tablas y los scripts SQL utilizados para el despliegue de la base de datos.

### Enlaces Relacionados:
- [Carga_Datos_Finales_a_SQL.ipynb](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/Sprint_1/Conexion_SQL_Python/Carga_Datos_Finales_a_SQL.ipynb)

_____

## Punto 6: Crear el flujo que importe los datos a la base de datos

**Descripción:**

El proceso de creación del flujo que permita la importación de datos a la base de datos fue una de las etapas clave para garantizar la fiabilidad y la precisión en la gestión de la información dentro de **ComerLogistics**. Este flujo de datos fue diseñado para cargar de manera eficiente las compras, ventas, y los movimientos de inventario en el sistema, permitiendo que la empresa tenga acceso a datos en tiempo real. El enfoque fue asegurar que los datos se procesaran, transformaran y cargaran en la base de datos con la máxima integridad y sin pérdida de información.

### Acciones Realizadas:

1. **Desarrollo del Proceso de Ingesta de Datos (ETL):**
   El flujo de ingesta de datos fue diseñado como un **proceso ETL (Extracción, Transformación y Carga)**. La idea detrás de este proceso es simple pero poderosa: extraer los datos de los archivos originales, transformarlos para que sigan un formato estándar y luego cargarlos en la base de datos SQL Server. Este proceso se desarrolló utilizando Python y las bibliotecas **Pandas** y **SQLAlchemy**, asegurando flexibilidad y escalabilidad.

2. **Extracción de los Datos:**
   Se comenzaron a extraer datos de múltiples fuentes (principalmente archivos CSV) correspondientes a inventarios iniciales, ventas y compras. Esta fase de extracción implicó la lectura de archivos y la captura de datos en bruto que luego serían procesados y preparados para su integración en la base de datos.

   - **Tabla_Compras:** Contiene los registros de las compras realizadas, especificando la fecha, tienda y proveedor.
   - **Tabla_DetalleCompras:** Detalla los productos comprados, las cantidades y los precios.
   - **Tabla_InventarioInicial y Tabla_InventarioFinal:** Almacenan los niveles de inventario en el inicio y fin del periodo analizado.
   - **Tabla_VentasFinal:** Contiene las ventas por tienda y producto, especificando cantidades vendidas y montos.

3. **Transformación de los Datos:**
   Durante la fase de transformación, se llevaron a cabo las siguientes acciones:
   - **Normalización de datos:** Se garantizaron tipos de datos consistentes en todas las tablas. Por ejemplo, se uniformizaron formatos de fecha, tipos de columnas numéricas y cadenas de texto.
   - **Limpieza de datos:** Se manejaron los valores nulos, asegurando que no existieran inconsistencias en los datos que pudieran afectar los análisis posteriores. Se eliminaron filas duplicadas y se completaron valores faltantes utilizando métodos como la imputación de datos.
   - **Cálculo de métricas adicionales:** Se implementaron cálculos adicionales, como la suma de cantidades compradas y vendidas, lo que facilitó la integración y posterior análisis de los datos.
   - **Relaciones de claves:** Se aseguraron las relaciones entre las tablas, respetando la integridad referencial en todas las entidades.

4. **Carga de Datos a la Base de Datos:**
   Una vez los datos fueron transformados, se procedió a la carga en la base de datos SQL Server. Este proceso de carga fue automatizado a través de scripts en Python que establecieron la conexión con la base de datos utilizando **SQLAlchemy** y **PyODBC**. Los datos se insertaron en las tablas correspondientes asegurando que los índices y claves foráneas estuvieran correctamente configurados para optimizar las consultas y mantener la integridad de los datos.

   - **Automatización del proceso de carga:** Se utilizó un script de Python, el cual ejecuta el proceso de carga cada vez que se actualizan los datos o se reciben nuevos registros. Esto garantiza que la base de datos esté siempre actualizada y los informes generados en Power BI reflejen la información más reciente.

5. **Validación del Proceso de Carga:**
   Después de cargar los datos, se realizaron pruebas de validación para verificar que la información se había ingresado correctamente. Se utilizaron consultas SQL para verificar que los datos fueran precisos y que no se hubiera producido pérdida de información o duplicación de registros.

6. **Documentación del Flujo de Importación de Datos:**
   Todo el proceso fue documentado en el notebook **Carga_Datos_Finales_a_SQL.ipynb**, el cual incluye todos los scripts utilizados para la conexión a la base de datos, la transformación y la carga de los datos. La documentación también incluye ejemplos prácticos de cómo se realizó la validación de la integridad de los datos.

### Desafíos y Soluciones:

1. **Grandes volúmenes de datos:** Uno de los principales retos fue manejar grandes volúmenes de datos sin afectar el rendimiento. Se implementaron técnicas como el procesamiento por lotes, lo cual permitió cargar los datos en pequeñas partes para no sobrecargar la memoria o los recursos del servidor.
2. **Integridad de los datos:** Otro desafío fue garantizar que no hubiera pérdida de datos durante la transformación y la carga. Esto se logró mediante la validación en cada paso del proceso y el uso de claves primarias y foráneas bien definidas para mantener la coherencia entre las tablas.

### Enlaces Relacionados:
- [Carga_Datos_Finales_a_SQL.ipynb](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/Sprint_1/Conexion_SQL_Python/Carga_Datos_Finales_a_SQL.ipynb)

_____

## 7. Validar que todos tengan acceso a dicha base de datos y que puedan extraer datos sin problemas

### Acción Realizada:

Una vez establecida la base de datos SQL Server y cargados todos los datos, el siguiente paso clave fue garantizar que todos los miembros del equipo tuvieran acceso sin problemas a dicha base de datos y pudieran extraer los datos requeridos para el análisis en tiempo real.

Se realizaron pruebas de acceso y conectividad con cada miembro del equipo para verificar que todos pudieran interactuar con la base de datos a través de sus propios entornos locales y herramientas. Estas pruebas incluyeron la verificación de los permisos de lectura y escritura, asegurándose de que cada miembro pudiera realizar consultas SQL, extraer datasets, y ejecutar scripts para alimentar el análisis en Python y Power BI sin interrupciones.

Se generaron credenciales personalizadas para cada miembro del equipo, otorgando los permisos necesarios para asegurar que cada uno tuviera los privilegios adecuados para trabajar sobre la base de datos sin comprometer la integridad de la misma.

### Pruebas Realizadas:
1. **Prueba de Conectividad**: Se verificó que todos los usuarios pudieran conectarse a la base de datos COMERLOGISTICS a través de la VPN establecida, garantizando un acceso seguro.
2. **Pruebas de Consulta y Extracción de Datos**: Se probaron consultas SQL básicas y avanzadas, confirmando que todos los usuarios pudieran acceder a los datos requeridos, extraer tablas completas o subconjuntos específicos de información.
3. **Pruebas de Escritura (con permisos restringidos)**: A los usuarios con permisos de escritura se les concedió la capacidad de cargar nuevos datos para asegurar que la base de datos se mantuviera actualizada sin duplicaciones ni errores de carga.

El equipo de **ComerLogistics** utilizó las siguientes herramientas y scripts para verificar el acceso a la base de datos:
- Conexión SQL/Python para ejecutar scripts que extraían datos de la base de datos a Python [Enlace a Script de Conexión SQL/Python](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/main/Sprint_1/Conexion_SQL_Python)
- SQL Server Management Studio para acceder y visualizar los datos directamente desde SQL Server.

**Repositorio Relacionado:**
- [Validación de Acceso a la Base de Datos en el Repositorio de ComerLogistics](https://github.com/Dapt01G2-Henry/ComerLogistics/tree/main)

**Conclusión**:
La validación del acceso a la base de datos se completó con éxito. Todos los miembros del equipo pueden ahora acceder, extraer y manipular los datos necesarios para el análisis, lo que asegura un flujo continuo de trabajo en el proceso de análisis de datos y visualización en Power BI.

_____

## 8. Crear el método de automatización de ingesta de datos nuevos

### Acción Realizada:

El equipo de **ComerLogistics** implementó un método automatizado para la ingesta de datos nuevos que garantiza la actualización constante de la base de datos sin intervención manual. Este proceso es clave para mantener la integridad y actualidad de los datos en todo momento, asegurando que el sistema refleje la información más reciente, tanto en el análisis de inventarios como en las métricas de ventas y compras.

El flujo de automatización se estructuró en varias fases críticas, todas documentadas y validadas:

1. **Desarrollo del Script en Python**:
   Se diseñó y desarrolló un script en Python utilizando las bibliotecas `pandas` y `sqlalchemy`, las cuales permiten gestionar la conexión con la base de datos SQL Server. Este script se encargó de automatizar la ingesta de datos incrementales, de tal forma que solo los registros nuevos sean cargados en la base de datos.

   El proceso comenzó con la definición de una lista de archivos (por ejemplo, `Tabla_Compras.csv`, `Tabla_Ventas.csv`, etc.), la cual el script analiza cada vez que se ejecuta. Para cada archivo, el sistema verifica si los registros ya existen en la base de datos, evitando duplicados y sobrecargas innecesarias. Si se encuentran nuevos registros, estos son agregados a las tablas correspondientes en SQL Server.

   El código relevante para la ingesta incremental puede revisarse en este [notebook de Automatización de Datos Nuevos](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/Sprint_1/Conexion_SQL_Python/AutomatizacionDatosNuevos.ipynb).

2. **Configuración de la Ejecución Automática**:
   Para garantizar que el proceso de ingesta de datos nuevos se ejecute sin intervención manual, se configuró un archivo por lotes `.bat` en Windows que ejecuta el script de Python de manera periódica. Esta tarea programada se configuró para ejecutarse semanalmente a una hora específica mediante el **Task Scheduler** de Windows. Esto permite que el sistema sea autosuficiente, cargando nuevos datos de manera regular sin que un usuario tenga que ejecutar el proceso manualmente.

3. **Pruebas y Validación del Proceso**:
   Se realizaron pruebas exhaustivas para garantizar que el sistema funcione correctamente y que solo los registros nuevos sean cargados. Estas pruebas incluyeron la inserción de datos simulados y reales para validar que no hubiera duplicaciones ni errores en la base de datos. También se monitoreó el rendimiento del sistema para asegurar que la ingesta se realizara de manera eficiente, sin comprometer el tiempo de respuesta del sistema.

   Las pruebas se documentaron en el [notebook de Automatización de Datos Nuevos](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/Sprint_1/Conexion_SQL_Python/AutomatizacionDatosNuevos.ipynb), donde se incluyó un registro de los resultados obtenidos en cada ejecución del script.

4. **Monitorización Continua**:
   Además de las pruebas iniciales, se estableció un mecanismo de monitorización continua para detectar cualquier fallo en el proceso de ingesta. Esta monitorización incluye la captura de logs de cada ejecución del script, lo que permite al equipo de desarrollo verificar rápidamente si hubo problemas durante la ejecución de una tarea programada.

   En caso de errores, el sistema está configurado para enviar alertas automáticas al equipo, lo que permite una rápida intervención y resolución de problemas.

### Herramientas Utilizadas:
- **Python**: Para el desarrollo del script automatizado.
- **Pandas y SQLAlchemy**: Para la manipulación de datos y la conexión con la base de datos SQL Server.
- **Task Scheduler de Windows**: Para la automatización de la ejecución del script.
- **SQL Server**: Base de datos en la que se almacenan los datos extraídos.

### Resultados:
Con la automatización de la ingesta de datos nuevos, se ha conseguido un sistema eficiente, que se actualiza periódicamente y mantiene la base de datos sincronizada con las operaciones diarias de **ComerLogistics**. Esto permite a los analistas y tomadores de decisiones acceder siempre a información actualizada, mejorando así la calidad y rapidez en las decisiones estratégicas.

### Conclusión:
El método de automatización de ingesta de datos nuevos implementado para **ComerLogistics** ha demostrado ser robusto, escalable y eficiente, garantizando que el sistema de análisis de datos funcione con la información más actual sin necesidad de intervención manual. Este enfoque permitirá a la compañía continuar con la expansión de su sistema de información a medida que crece su negocio, sin sacrificar la calidad ni la integridad de los datos.

### Enlaces Relacionados:
- [Notebook de Automatización de Datos Nuevos](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/Sprint_1/Conexion_SQL_Python/AutomatizacionDatosNuevos.ipynb)

_____