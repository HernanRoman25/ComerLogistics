
# **Entregables Sprint 2**

## Objetivo General del Sprint 2

El objetivo principal de este sprint fue desarrollar un informe interactivo y funcional en Power BI que permitiera a los usuarios realizar un análisis detallado de las operaciones de ComerLogistics. El informe debía proporcionar visualizaciones claras y concisas de los datos clave, permitiendo tomar decisiones informadas basadas en métricas precisas.

Para lograr este objetivo, se realizaron una serie de pasos que abarcan desde la creación del archivo .pbix hasta la validación final del informe. Este sprint se enfocó en asegurar que todas las etapas, desde la importación de datos hasta la generación de reportes y gráficos, se llevaran a cabo con la máxima precisión y profesionalismo.

_____

## **1. Crear el archivo .pbix**

En el inicio del **Sprint 2**, el primer paso crítico fue la creación del archivo **.pbix** en **Power BI Desktop**. Este archivo es fundamental, ya que funciona como el contenedor que almacena todos los datos, cálculos, y visualizaciones necesarias para desarrollar el dashboard interactivo y los informes finales.

El archivo **.pbix** no solo es un archivo de datos, sino que también sirve como el entorno de desarrollo dentro del cual se lleva a cabo todo el trabajo de análisis, transformación de datos y diseño visual. Es aquí donde se establecen las conexiones a las distintas fuentes de datos, se crean las medidas calculadas utilizando el lenguaje **DAX**, y se diseñan los gráficos e informes que permiten a los usuarios finales interactuar de manera efectiva con los datos.

### **Detalles de la acción realizada:**
- **Creación del archivo**: Se creó un archivo en blanco en **Power BI Desktop** con el nombre **ComerLogisticsDashNube.pbix**. Este archivo fue configurado desde el principio para organizar los datos y facilitar su posterior procesamiento y análisis.
- **Configuración inicial**: El archivo se configuró con el formato de proyecto adecuado, permitiendo múltiples conexiones a fuentes de datos externas, tales como bases de datos **SQL Server**, **archivos Excel**, y **archivos CSV**. Cada fuente de datos fue seleccionada de acuerdo con los requisitos de análisis de **ComerLogistics**.
- **Estructura del archivo**: Dentro del archivo **.pbix**, se crearon secciones organizadas para gestionar los datos importados, las transformaciones aplicadas, y las medidas calculadas. Además, se incluyeron áreas específicas para los distintos dashboards y páginas de informes que se desarrollarían a lo largo del proyecto. Esta estructura ordenada permite que los desarrolladores trabajen de manera eficiente y coherente, asegurando que todos los componentes del análisis estén bien integrados.

### **Valor de este paso para el proyecto:**
- **Base para el análisis**: Este archivo es la base para todo el análisis y visualización que se lleva a cabo en Power BI. Sin un archivo **.pbix** bien estructurado, el proyecto carecería de un marco que conecte los datos con las visualizaciones y los cálculos.
- **Facilita la colaboración**: La creación de este archivo no solo permite que un desarrollador trabaje en los datos, sino que facilita el trabajo colaborativo, ya que múltiples personas pueden agregar, modificar y actualizar las visualizaciones, medidas, y cálculos, manteniendo la coherencia del análisis.
- **Preparación para la interacción**: Con la estructura base establecida en el archivo **.pbix**, se puede comenzar a trabajar en los elementos interactivos que permitirán a los usuarios finales explorar los datos en profundidad. El archivo **.pbix** está diseñado para soportar filtros, segmentadores y otros elementos visuales que ayudan a personalizar el análisis según las necesidades del negocio.

### **Conexión con otros pasos del sprint:**
Este paso inicial es crucial porque, una vez que el archivo está creado, se puede proceder con las siguientes etapas del desarrollo, como la importación de datos, limpieza, transformación, creación de medidas y visualizaciones. Cada una de estas acciones se lleva a cabo dentro del entorno proporcionado por el archivo **.pbix**, lo que asegura que todo el proceso esté centralizado y sea fácil de gestionar.

### **Siguiente paso:**
Tras la creación del archivo, el siguiente paso fue la **importación de datos** desde diferentes fuentes, que permitió comenzar a trabajar con la información real de **ComerLogistics** y llevar a cabo el análisis necesario.

[Repositorio ComerLogistics en GitHub](https://github.com/Dapt01G2-Henry/ComerLogistics)

_____

## **Punto 2: Importación de Datos a Power BI**

La importación de datos en Power BI fue un paso fundamental para comenzar a trabajar con la información disponible de **ComerLogistics** y dar inicio al análisis de los datos. Este proceso involucró la importación de archivos CSV, bases de datos SQL y otros orígenes de datos, de manera que se pudiera trabajar con ellos en el entorno de Power BI.

### **2. Importación de Datos a Power BI**

**Objetivo**: El objetivo de esta fase fue centralizar y cargar todos los datos relevantes en Power BI para realizar las transformaciones necesarias, análisis y posteriormente diseñar las visualizaciones interactivas.

### **Detalles de la acción realizada**:

1. **Selección de orígenes de datos**:
   - Los datos fueron recopilados de múltiples fuentes, entre ellas archivos CSV que contenían los datos históricos de inventarios, ventas, compras y productos, así como de una base de datos SQL que almacenaba registros clave del negocio.
   - El equipo decidió cargar todos los datos en Power BI desde estas fuentes para poder trabajar con ellos de manera centralizada.

2. **Importación de datos clave**:
   - **Inventario Inicial (BegInvFINAL12312016.csv)**: Representa el inventario al comienzo del período de análisis. Estos datos fueron esenciales para tener una referencia de las unidades disponibles y el valor del inventario en ese momento.
   - **Inventario Final (EndInvFINAL12312016.csv)**: Inventario registrado al final del período de análisis. Estos datos permitieron comparar la evolución del inventario y analizar su rotación.
   - **Compras (PurchasesFINAL12312016.csv)**: Registros de todas las compras realizadas por ComerLogistics durante el período. Se importaron los detalles de cada transacción, como las cantidades adquiridas, precios y fechas.
   - **Ventas (SalesFINAL12312016.csv)**: Datos de las ventas realizadas en el período. Estos archivos contienen información como productos vendidos, cantidades, precios y tiendas involucradas.
   - **Precios de Compra (2017PurchasePricesDec.csv)**: Archivo que contiene los precios de compra de los productos adquiridos, esencial para calcular los costos y márgenes.

3. **Estructuración y unificación de los datos**:
   - Durante la importación, se realizaron algunas modificaciones para asegurar que los datos de diferentes fuentes fueran compatibles entre sí y estuvieran listos para su análisis. Se realizó un mapeo de campos para asegurarse de que las tablas compartieran las claves necesarias (por ejemplo, *MarcaID* y *Tienda*).
   - Cada archivo fue importado como una tabla independiente en **Power BI**, y se crearon relaciones entre ellas utilizando campos comunes, como *InventarioInicialID* o *MarcaID*. Esta estructura permitió realizar análisis cruzados entre las diferentes fuentes de datos.

4. **Integración de bases de datos SQL**:
   - Se estableció una conexión directa a la base de datos **SQL Server** donde se almacenan los registros históricos de la empresa. A través de esta conexión, los datos de **ComerLogistics** fueron importados automáticamente, asegurando que estuvieran siempre actualizados sin la necesidad de cargar manualmente archivos CSV adicionales.
   - Las tablas de SQL importadas incluyen:
     - **Tabla_InventarioInicial**
     - **Tabla_InventarioFinal**
     - **Tabla_Compras**
     - **Tabla_VentasFinal**
     - **Tabla_Producto**

5. **Documentación de la importación**:
   - Se generó documentación en el archivo `documentacion.md` del repositorio de GitHub, explicando los pasos seguidos para la importación de datos, las tablas involucradas, y las relaciones creadas entre ellas. Este archivo de documentación es clave para que todos los miembros del equipo comprendan cómo se ha estructurado la información dentro de Power BI.
   - [Consulta el archivo de documentación en GitHub](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/documentacion.md).

### **Importancia de este paso en el proyecto**:

- **Centralización de datos**: Al importar todos los datos relevantes a Power BI desde diferentes fuentes, se logró centralizar la información en una única plataforma. Esto facilita el análisis y permite a todos los miembros del equipo trabajar con los mismos datos actualizados.
  
- **Relaciones entre tablas**: La creación de relaciones entre las diferentes tablas importadas permitió realizar análisis más complejos y cruzados, como el impacto de las compras en el inventario final o la relación entre las ventas y los niveles de inventario en las tiendas.

- **Automatización de la actualización de datos**: La conexión a la base de datos **SQL Server** permitió que los datos estuvieran siempre actualizados en **Power BI** sin necesidad de carga manual. Esto mejora la eficiencia del análisis y asegura que los informes siempre se basen en los datos más recientes.

### **Siguientes pasos**:
Con los datos ya importados y listos para su uso en **Power BI**, el siguiente paso fue la limpieza y transformación de los datos para asegurar su calidad y adecuarlos a los análisis que se realizarán en los reportes.

[Repositorio ComerLogistics en GitHub](https://github.com/Dapt01G2-Henry/ComerLogistics)

_____


## **3. Limpieza y Transformación de los Datos en Power BI**

El tercer paso en el desarrollo del **Sprint 2** fue la **limpieza** y **transformación** de los datos importados. Esta fase es crítica, ya que asegura que los datos estén libres de errores y en un formato que permita su análisis efectivo. A través de las herramientas de **Power Query** de Power BI, se realizaron diferentes transformaciones y operaciones de limpieza para preparar los datos para el análisis.

### **Objetivo**:
El objetivo de esta etapa fue realizar la limpieza y transformación de los datos, asegurando que todos los valores fueran correctos, sin duplicados, y en los formatos adecuados para su análisis. Además, se generaron columnas calculadas que agregaron valor a los reportes y medidas para el análisis posterior.

### **Detalles de la acción realizada**:

1. **Uso de Power Query para la limpieza de datos**:
   - Una vez importados los datos, el siguiente paso fue cargar todas las tablas en **Power Query Editor**. Aquí se realizaron las primeras operaciones de limpieza:
     - **Eliminación de duplicados**: Se revisaron las tablas para identificar y eliminar registros duplicados que pudieran generar distorsiones en el análisis. Esto fue especialmente importante en las tablas de compras y ventas, donde errores en la carga podrían llevar a una interpretación incorrecta de los volúmenes de transacciones.
     - **Relleno de valores faltantes**: Se identificaron columnas que tenían valores faltantes y, dependiendo de la naturaleza del dato, se decidió si se rellenaban con valores predeterminados (por ejemplo, cero en el caso de cantidades) o si se eliminaban aquellos registros donde faltaba información crítica.
     - **Corrección de errores tipográficos y formateo**: En las columnas de texto, como nombres de productos y tiendas, se unificaron los nombres que estaban mal escritos o con diferentes formatos. Esto incluyó la normalización de mayúsculas y minúsculas para evitar inconsistencias en el análisis.
   
2. **Transformación de tipos de datos**:
   - Se corrigieron los tipos de datos de varias columnas para asegurar que las operaciones aritméticas y las agregaciones funcionaran correctamente:
     - **Fechas**: Se aseguraron de que todas las columnas que contenían fechas, como *Fecha de Compra*, *Fecha de Venta*, y *Fecha de Inventario*, estuvieran correctamente tipificadas como fechas en **Power BI**. Esto es esencial para realizar análisis temporales y comparaciones de períodos.
     - **Números y valores decimales**: Las columnas de cantidades, precios y totales se formatearon correctamente para permitir cálculos precisos, como sumas y promedios.
     - **Texto**: Las columnas que contenían descripciones de productos, tiendas y marcas se verificaron para asegurarse de que estuvieran correctamente tipificadas como texto y sin errores.

3. **Normalización y estandarización de los datos**:
   - Uno de los retos de este proyecto fue trabajar con múltiples fuentes de datos, lo que significa que algunos nombres y formatos variaban entre tablas. Para solucionar esto, se realizó un proceso de normalización:
     - **Estandarización de nombres de productos y tiendas**: Se crearon reglas para que los nombres de productos y tiendas fueran consistentes entre las diferentes tablas. Esto incluyó la eliminación de espacios innecesarios, la corrección de errores tipográficos y la unificación del uso de mayúsculas y minúsculas.
     - **Unificación de formatos de fecha**: Todos los formatos de fecha fueron unificados para asegurar que se pudieran realizar comparaciones de manera precisa. Las fechas fueron formateadas como **"AAAA-MM-DD"** en todas las tablas para evitar confusiones con diferentes formatos regionales.
     - **Tratamiento de valores faltantes y datos atípicos (outliers)**: Se revisaron las tablas para identificar datos atípicos, como precios extremadamente bajos o altos, y se tomaron decisiones sobre cómo manejarlos (por ejemplo, reemplazarlos con valores promedio o descartarlos si no eran representativos).

4. **Creación de columnas calculadas**:
   - Durante el proceso de transformación, se crearon varias **columnas calculadas** que añadieron valor al análisis y facilitaron la interpretación de los datos:
     - **Unidades Disponibles por Producto y Tienda**: Se calculó una columna que indicaba las unidades disponibles por cada producto en cada tienda, combinando los datos del inventario inicial y las compras realizadas.
     - **Valor Total del Inventario**: Se creó una columna que multiplicaba las unidades disponibles por el precio de compra de cada producto, permitiendo obtener el valor total del inventario en cada tienda y por cada producto.
     - **Margen de Utilidad**: Se calculó el margen de utilidad para cada producto, restando el costo de compra al precio de venta, y dividiendo por el precio de venta. Este margen permitió identificar los productos más rentables para **ComerLogistics**.

5. **Creación de medidas clave**:
   - Se utilizaron fórmulas **DAX** (Data Analysis Expressions) para crear medidas que pudieran ser reutilizadas en diferentes visualizaciones y cálculos en el informe final. Entre las medidas creadas están:
     - **Total Unidades Compradas**: `SUM(Tabla_Compras[CantidadComprada])`
     - **Total Unidades Vendidas**: `SUM(Tabla_VentasFinal[CantidadVendida])`
     - **Total Valor del Inventario**: `SUM(Tabla_InventarioFinal[Valor_total])`
     - **Promedio de Margen de Utilidad**: `AVERAGE(Tabla_Producto[Margen_Utilidad])`
     Estas medidas proporcionaron información clave sobre las transacciones y permitieron realizar comparaciones y análisis agregados.

6. **Documentación del proceso de transformación**:
   - Se documentaron todos los pasos de limpieza y transformación en el archivo **`documentacion.md`** del repositorio, proporcionando una descripción clara y detallada de cada operación realizada. Esta documentación es esencial para que todos los miembros del equipo puedan entender las decisiones tomadas durante el proceso de limpieza y transformación de los datos.
   - [Consulta la documentación en GitHub](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/documentacion.md).

### **Importancia de este paso en el proyecto**:

- **Calidad de los datos**: Al limpiar y transformar los datos, se aseguró que los análisis y reportes producidos en **Power BI** fueran precisos y reflejaran correctamente la situación del negocio. Los datos incorrectos o duplicados pueden llevar a decisiones erróneas, por lo que esta fase fue fundamental.
  
- **Facilitación del análisis**: Las columnas calculadas y las medidas creadas simplificaron el proceso de análisis en **Power BI**, permitiendo realizar cálculos complejos y visualizar rápidamente métricas importantes, como las unidades disponibles o el valor total del inventario.

- **Automatización y escalabilidad**: Al automatizar la limpieza y transformación de los datos en **Power Query**, se aseguró que este proceso fuera reproducible para futuras cargas de datos. Esto significa que, cuando se agreguen nuevos datos, la misma lógica de limpieza se aplicará automáticamente, manteniendo la coherencia y calidad en los datos.

### **Siguientes pasos**:
Tras la limpieza y transformación de los datos, el equipo procederá a **crear las relaciones necesarias** entre las tablas y diseñar las **visualizaciones** para los informes en **Power BI**.

---

[Repositorio ComerLogistics en GitHub](https://github.com/Dapt01G2-Henry/ComerLogistics)

_____

## **4. Creación de Medidas, Columnas Calculadas y Relaciones en Power BI**

En este punto del **Sprint 2**, nos centramos en la creación de **medidas DAX**, **columnas calculadas** y el establecimiento de **relaciones** entre las tablas de datos. Estos elementos son fundamentales para que **Power BI** pueda realizar cálculos y análisis de forma dinámica y precisa.

### **Objetivo**:
El objetivo principal de esta etapa fue generar medidas y columnas que permitieran realizar cálculos específicos que no estaban presentes en los datos crudos, así como definir las relaciones entre las tablas para habilitar un análisis cruzado. Con estas herramientas, se logró preparar los datos para su uso en las visualizaciones y gráficos del informe final.

### **Detalles de la acción realizada**:

1. **Creación de Medidas DAX**:
   - Las **medidas** son esenciales en **Power BI** para realizar cálculos complejos y agregar datos de manera dinámica. A continuación, se detallan las principales medidas creadas:
     - **Total Unidades Iniciales**:
       - Esta medida calcula el total de unidades disponibles al inicio del período analizado.
       ```DAX
       Total Unidades Iniciales = SUM(Tabla_InventarioInicial[Unidad_disponible])
       ```
       Esta medida permitió visualizar la cantidad de inventario inicial disponible en cada tienda y para cada producto.
     
     - **Total Unidades Finales**:
       - Similar a la medida anterior, pero aplicada al inventario final.
       ```DAX
       Total Unidades Finales = SUM(Tabla_InventarioFinal[Unidad_disponible])
       ```
       Esta medida permitió analizar cómo evolucionó el inventario a lo largo del tiempo y en las diferentes ubicaciones.

     - **Total Compras**:
       - Mide el total de productos comprados durante el período analizado.
       ```DAX
       Total Compras = SUM(Tabla_Compras[CantidadComprada])
       ```
       Esta medida proporcionó una visión detallada de las compras por tienda y producto, permitiendo analizar patrones de compra.

     - **Total Ventas**:
       - Calcula la suma total de unidades vendidas en el período.
       ```DAX
       Total Ventas = SUM(Tabla_VentasFinal[CantidadVendida])
       ```
       Esta medida fue clave para analizar los productos más vendidos y las tiendas con mayor volumen de ventas.

     - **Valor Monetario Total del Inventario**:
       - Calcula el valor monetario total del inventario, multiplicando las unidades disponibles por el precio de compra de cada producto.
       ```DAX
       Valor Monetario Total = SUMX(Tabla_InventarioFinal, Tabla_InventarioFinal[Unidad_disponible] * RELATED(Tabla_Productos[Precio_compra]))
       ```
       Esta medida permitió evaluar el valor económico de los productos almacenados en las distintas ubicaciones.

     - **Margen de Utilidad por Producto**:
       - Calcula el margen de utilidad por producto, restando el precio de compra del precio de venta, y dividiendo por el precio de venta.
       ```DAX
       Margen de Utilidad = DIVIDE(SUM(Tabla_Producto[Precio_venta] - Tabla_Producto[Precio_compra]), SUM(Tabla_Producto[Precio_venta]))
       ```
       Esta medida fue importante para identificar los productos más rentables y para evaluar el desempeño financiero de cada línea de productos.

2. **Creación de Columnas Calculadas**:
   - A diferencia de las medidas, las **columnas calculadas** se generan en el nivel de fila y son útiles cuando se necesita realizar cálculos dentro de una tabla en particular. Algunas de las columnas creadas incluyen:
     
     - **Valor Total del Inventario**:
       - Esta columna calcula el valor total del inventario disponible en cada tienda para cada producto.
       ```DAX
       Valor Total Inventario = Tabla_InventarioFinal[Unidad_disponible] * RELATED(Tabla_Productos[Precio_compra])
       ```

     - **Rotación de Inventario**:
       - Se creó una columna para calcular la rotación de inventario, que permite evaluar qué tan rápido se están vendiendo los productos en relación con el inventario disponible.
       ```DAX
       Rotación de Inventario = DIVIDE(Tabla_VentasFinal[CantidadVendida], Tabla_InventarioFinal[Unidad_disponible])
       ```

     - **Dias en Inventario**:
       - Esta columna permitió calcular cuántos días en promedio se mantiene un producto en el inventario antes de venderse.
       ```DAX
       Dias en Inventario = Tabla_VentasFinal[Fecha_Venta] - Tabla_InventarioInicial[Fecha_Inventario]
       ```

3. **Establecimiento de Relaciones entre Tablas**:
   - En **Power BI**, las relaciones permiten conectar diferentes tablas a través de campos comunes, lo que habilita el análisis cruzado entre diferentes conjuntos de datos. Para **ComerLogistics**, las relaciones clave se establecieron de la siguiente manera:
     
     - **Relación entre Inventario y Productos**:
       - Se utilizó la columna `MarcaID` para conectar la tabla de inventario (inicial y final) con la tabla de productos. Esto permitió analizar cuántas unidades de cada marca estaban disponibles en el inventario y su respectivo valor.
     
     - **Relación entre Compras y Ventas**:
       - Se estableció una relación entre las tablas de compras y ventas mediante el campo `ProductoID`, lo que permitió comparar directamente los productos comprados con los vendidos y calcular métricas como el margen de utilidad y la rotación del inventario.

     - **Relación entre Tiendas y Compras/Ventas**:
       - La tabla de tiendas fue relacionada con las tablas de compras y ventas mediante la columna `TiendaID`. Esto habilitó el análisis de las transacciones por ubicación geográfica, permitiendo comparar el desempeño de las diferentes tiendas.

4. **Documentación y Optimización del Modelo de Datos**:
   - Para asegurar la claridad en el manejo de los datos, se documentó todo el proceso de creación de medidas, columnas y relaciones en el archivo **`documentacion.md`**. Esto incluyó descripciones detalladas de cada medida y columna, así como las decisiones tomadas para establecer las relaciones entre las tablas.
   - Además, se realizaron ajustes en el modelo de datos para optimizar el rendimiento de las consultas y mejorar la experiencia del usuario al interactuar con el **dashboard**. Esto incluyó la eliminación de columnas no utilizadas, la optimización de las relaciones, y la revisión de las medidas DAX para asegurar un cálculo eficiente.
   
   - [Consulta la documentación en GitHub](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/documentacion.md).

### **Importancia de este paso en el proyecto**:

- **Análisis dinámico y detallado**: Las medidas y columnas calculadas permitieron realizar un análisis profundo de las transacciones y el inventario, brindando una visión clara de la relación entre compras, ventas y el inventario disponible.
  
- **Flexibilidad en las visualizaciones**: Al establecer relaciones entre las diferentes tablas, se logró flexibilidad para crear visualizaciones y gráficos en **Power BI**, donde los usuarios pueden explorar los datos desde diferentes perspectivas y filtrar por variables como tienda, producto o marca.

- **Toma de decisiones basada en datos**: Las medidas generadas proporcionaron métricas clave para la toma de decisiones, como el valor total del inventario, la rotación de productos y el margen de utilidad, que fueron esenciales para identificar áreas de mejora en la gestión del inventario y las ventas.

### **Siguientes pasos**:
Con las medidas, columnas calculadas y relaciones correctamente configuradas, el equipo procederá a diseñar las visualizaciones y gráficos interactivos que presentarán la información de manera clara y eficiente para los usuarios finales.

---

[Repositorio ComerLogistics en GitHub](https://github.com/Dapt01G2-Henry/ComerLogistics)

_____

## **5. Diseño de reportes y gráficos en Power BI**

El diseño de reportes y gráficos es una fase crítica dentro del **Sprint 2**, ya que es el momento en el que los datos procesados se transforman en visualizaciones interactivas y accesibles que permiten la toma de decisiones basada en datos. En esta etapa, el equipo se concentró en crear un dashboard que no solo fuera visualmente atractivo, sino que también contara con la capacidad de proporcionar insights clave sobre las ventas, compras, y gestión de inventarios de **ComerLogistics**.

### **Objetivo del paso**:
El objetivo de este paso fue crear un conjunto de reportes y gráficos interactivos en **Power BI** que permitieran al equipo de **ComerLogistics** analizar su rendimiento operativo y financiero en tiempo real. Estos reportes ofrecen un análisis detallado sobre ventas, inventarios, y compras, proporcionando al usuario final una herramienta que les permite identificar tendencias, patrones y áreas de mejora.

### **Detalles de la acción realizada**:

1. **Creación de un Dashboard Principal**:
   - El **dashboard principal** se diseñó con el propósito de ofrecer una **visión general del rendimiento del negocio**. Contiene **indicadores clave de rendimiento (KPIs)** que permiten realizar un seguimiento en tiempo real de las métricas más importantes para **ComerLogistics**.
   - **Elementos clave del dashboard principal**:
     - **KPIs de ventas y compras**: Estos indicadores proporcionan un resumen rápido de los ingresos totales, costos de las compras, y el margen de utilidad.
     - **Gráfico de líneas comparativo**: Se incluyó un gráfico de líneas que muestra la evolución de las ventas y compras durante el período analizado. Este gráfico permite identificar tendencias y patrones a lo largo del tiempo, facilitando la toma de decisiones estratégicas sobre la gestión del inventario y la planificación de compras.
     - **Tabla de inventario por tienda**: Una tabla dinámica que muestra el inventario disponible en cada tienda, desglosado por producto. Esta tabla es interactiva y permite a los usuarios aplicar filtros por ciudad, marca, y producto para profundizar en los detalles de las tiendas que les interesan.

2. **Diseño de gráficos interactivos**:
   - Se diseñaron una serie de gráficos interactivos que permitieron al usuario **explorar los datos de manera intuitiva**. Cada gráfico fue cuidadosamente seleccionado para representar la información más relevante de manera clara y visualmente atractiva.
   
   - **Gráficos clave diseñados**:
     - **Gráfico de barras de ventas por tienda**:
       - Este gráfico muestra la distribución de las ventas entre las diferentes tiendas de **ComerLogistics**. Permite comparar el rendimiento de las tiendas entre sí y analizar qué ubicaciones generaron mayores ingresos.
       - Además, se añadió la posibilidad de **filtrar** las ventas por categorías de productos, marcas, y períodos de tiempo específicos.
     - **Gráfico de barras de productos más vendidos**:
       - Este gráfico destaca los **productos más vendidos** durante el período analizado, mostrando cuántas unidades de cada producto se vendieron. También se incluye un análisis por **categoría de productos**, lo que permite identificar las categorías más rentables para la empresa.
     - **Gráfico de dispersión de rotación de inventario**:
       - Este gráfico fue clave para identificar qué productos tienen la **mayor rotación de inventario**, ayudando a **ComerLogistics** a identificar aquellos productos que se venden más rápidamente y ajustar su estrategia de reposición y almacenamiento.
   
3. **Incorporación de mapas interactivos**:
   - Se incluyó un **mapa interactivo** que muestra la distribución geográfica de las tiendas y el inventario disponible en cada una de ellas. Este mapa permite al usuario visualizar de manera intuitiva dónde se encuentran las tiendas con mayor cantidad de inventario, facilitando el análisis geoespacial de la distribución de productos.
   
   - **Elementos del mapa**:
     - Cada punto en el mapa representa una tienda y su tamaño varía dependiendo de la cantidad de inventario disponible.
     - Los usuarios pueden aplicar **filtros** para visualizar los datos por marca, ciudad, o rango de fechas, lo que permite un análisis detallado por ubicación geográfica.

4. **Diseño de segmentadores y filtros interactivos**:
   - Para mejorar la **interactividad del dashboard**, se añadieron segmentadores que permiten a los usuarios **personalizar los reportes** y **focalizar el análisis** en los datos más relevantes para ellos.
   
   - **Segmentadores clave añadidos**:
     - **Segmentador de tiempo**: Permite seleccionar el período de tiempo a analizar, lo que da flexibilidad para observar datos históricos y tendencias a largo plazo o realizar análisis detallados sobre períodos cortos.
     - **Segmentador por ciudad y tienda**: Este segmentador permite a los usuarios filtrar los datos por ciudad y tienda, facilitando el análisis comparativo entre ubicaciones.
     - **Segmentador por producto y marca**: Los usuarios pueden filtrar los resultados por productos específicos o marcas, lo que permite identificar cuáles productos están generando mayor rendimiento en ventas o cuáles necesitan una estrategia de marketing adicional.

5. **Optimización de la interfaz de usuario**:
   - Se cuidó cada detalle del diseño para asegurar que el dashboard fuera no solo **visualmente atractivo**, sino también **intuitivo** y fácil de usar. El enfoque fue en **mejorar la experiencia del usuario** (UX), permitiendo que cualquier persona con acceso al informe pudiera interactuar con los datos de manera eficiente, sin necesidad de conocimientos técnicos avanzados.
   
   - **Elementos optimizados**:
     - **Paleta de colores**: Se seleccionó una paleta de colores que hiciera contraste entre las diferentes visualizaciones y que facilitara la interpretación rápida de la información.
     - **Diseño responsive**: Se aseguró que los gráficos y visualizaciones fueran adaptables y fáciles de visualizar en diferentes tamaños de pantalla, desde computadoras de escritorio hasta dispositivos móviles.
     - **Botones de navegación**: Se añadieron botones interactivos que permitían navegar de manera eficiente entre las diferentes secciones del dashboard. Esto mejora la fluidez y facilita la experiencia del usuario al recorrer los reportes.

6. **Documentación y presentación del diseño**:
   - Todo el proceso de diseño fue documentado, y se incluyó una sección en el archivo **[documentacion.md](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/documentacion.md)** del repositorio en **GitHub**, donde se describen los **gráficos**, **medidas** y **segmentadores** utilizados en cada uno de los reportes. La documentación está orientada a permitir que los usuarios finales y futuros desarrolladores puedan comprender fácilmente la estructura y funcionalidad del dashboard.
   
   - Además, el equipo se preparó para presentar el dashboard ante los stakeholders de **ComerLogistics**, explicando cómo los diferentes reportes y visualizaciones permiten a la compañía tomar decisiones basadas en datos, mejorando la eficiencia operativa y la gestión del inventario.

### **Importancia de este paso**:
El diseño de los reportes y gráficos en **Power BI** fue fundamental para transformar los datos procesados en insights valiosos que ayudaran a **ComerLogistics** a **optimizar su cadena de suministro**, mejorar la **gestión de inventarios** y maximizar las **ventas**. Las visualizaciones interactivas proporcionaron una vista integral del negocio, lo que permitió a los tomadores de decisiones explorar los datos en detalle y obtener respuestas rápidas a preguntas críticas.

### **Siguientes pasos**:
Con el diseño de los reportes completado, el siguiente paso es realizar **pruebas de calidad** para asegurarse de que todos los gráficos interactúen correctamente y que el dashboard esté optimizado para un rendimiento óptimo.

---

[Repositorio ComerLogistics en GitHub](https://github.com/Dapt01G2-Henry/ComerLogistics)

_____

## 6. Etapa de Pruebas de Calidad del Reporte

El proceso de pruebas de calidad es un paso crucial para asegurar que el informe desarrollado en **Power BI** cumpla con los requisitos funcionales, técnicos y visuales establecidos. Este paso no solo valida que los cálculos y visualizaciones sean correctos, sino que también garantiza que la experiencia del usuario sea óptima, evitando problemas de rendimiento y asegurando la coherencia de la información.

### **Objetivo del paso**:
El objetivo de esta etapa es asegurar que todas las interacciones y visualizaciones en el **dashboard** de **ComerLogistics** funcionen de manera fluida, sin errores en las relaciones de las tablas ni en los cálculos. Además, se busca optimizar el rendimiento del informe, revisando las consultas y asegurándose de que los tiempos de carga sean mínimos. Finalmente, se revisa la precisión y coherencia de los datos presentados, garantizando que cada visualización responda correctamente a las consultas realizadas por los usuarios.

### **Acciones Realizadas:**

1. **Validación de Cálculos y Medidas DAX**:
   - Se revisaron **todas las medidas y columnas calculadas** para garantizar que los resultados presentados sean correctos y coherentes con los datos originales. 
   
   - **Detalles de la validación**:
     - Las **medidas clave** como *Total Unidades Iniciales*, *Total Unidades Finales*, *Total Compras* y *Total Ventas* fueron comparadas contra los datos originales de los datasets para verificar que las fórmulas en DAX fueran precisas.
     - También se revisaron las **columnas calculadas** que se habían creado para análisis adicionales, como la **Unidad Disponible** por producto y tienda, asegurando que se calcularan correctamente para cada período y categoría.

2. **Revisión de Relaciones entre Tablas**:
   - Se revisaron las **relaciones entre las tablas** (Inventario, Compras, Ventas, etc.) dentro del modelo de datos de **Power BI**. Este paso fue esencial para asegurar que los reportes y gráficos reflejaran la información correcta al realizar filtros o cruzar datos de diferentes fuentes.
   
   - **Revisión detallada**:
     - Se comprobó que las **relaciones uno-a-muchos** estuvieran configuradas correctamente entre las diferentes tablas.
     - También se verificaron las **claves foráneas**, como *MarcaID*, *Tienda* y *Fecha*, para confirmar que las tablas estuvieran conectadas de manera eficiente y precisa.

3. **Pruebas de Interacción de Filtros**:
   - Uno de los aspectos más importantes en **Power BI** es la interactividad de los gráficos y reportes. Durante esta etapa se revisaron todos los **segmentadores** y **filtros** interactivos que se implementaron en el dashboard. Se verificó que los filtros afectaran correctamente las visualizaciones, permitiendo a los usuarios obtener insights precisos al aplicar diferentes criterios de búsqueda.
   
   - **Detalles de las pruebas**:
     - Se probaron los **segmentadores de fecha**, asegurando que los gráficos respondieran de manera correcta a los diferentes rangos de tiempo seleccionados por el usuario.
     - También se realizaron pruebas con los **filtros por ciudad, tienda y producto**, confirmando que las visualizaciones respondieran de manera precisa al ser filtradas por estas categorías.
   
4. **Optimización del Rendimiento del Informe**:
   - Un aspecto clave de la experiencia del usuario es el tiempo de respuesta del informe. Para asegurar que el dashboard cargue de manera eficiente, se llevaron a cabo pruebas de rendimiento y se optimizaron las consultas y relaciones entre tablas para minimizar el tiempo de espera.
   
   - **Acciones de optimización**:
     - Se revisaron todas las **consultas de datos** para garantizar que fueran lo más eficientes posible, eliminando pasos innecesarios en el proceso de transformación de datos.
     - Se optimizaron las **relaciones** entre tablas, simplificando algunas relaciones donde era posible para reducir la cantidad de procesamiento necesario.
     - Se revisó la configuración de **carga incremental de datos**, lo que permite actualizar solo los datos nuevos en lugar de recargar todo el conjunto de datos, mejorando el tiempo de actualización del informe.

5. **Verificación de la Precisión de Datos en Gráficos**:
   - Se realizó una revisión exhaustiva de los gráficos y tablas dinámicas para asegurar que los datos mostrados fueran precisos y estuvieran alineados con los resultados esperados. Durante este paso, se hicieron pruebas para detectar posibles inconsistencias en las cifras presentadas en los gráficos.
   
   - **Validación de datos**:
     - Se compararon los valores presentados en los gráficos con los valores reales de los datasets importados, confirmando que los cálculos en **Power BI** coincidan con los datos originales.
     - También se revisaron las **visualizaciones geográficas**, como el mapa interactivo, asegurando que las coordenadas de cada tienda fueran precisas y que los valores de inventario por ubicación fueran correctos.

6. **Revisión Visual y de Experiencia de Usuario (UX)**:
   - Se realizaron revisiones detalladas para mejorar la experiencia del usuario final, garantizando que el dashboard fuera **intuitivo**, **fácil de usar** y estéticamente agradable.
   
   - **Mejoras en el diseño**:
     - Se ajustaron los tamaños de los gráficos y tablas para asegurarse de que los datos se visualicen de manera clara en diferentes tamaños de pantalla y dispositivos.
     - Se realizó una optimización de la **paleta de colores** y el **diseño visual**, asegurando que la visualización de las métricas fuera clara y que los usuarios pudieran interpretar rápidamente los resultados.
     - Se probaron las **navegaciones interactivas** y botones añadidos para facilitar la navegación entre diferentes secciones del dashboard.

7. **Documentación y Feedback**:
   - Se documentaron todos los cambios y mejoras realizadas en esta fase de pruebas. Además, se compartió el dashboard con el equipo para obtener feedback adicional y realizar ajustes finales antes de la entrega al cliente.
   
   - **Documentación**:
     - Todos los pasos de validación y optimización fueron registrados en el archivo **[documentacion.md](https://github.com/Dapt01G2-Henry/ComerLogistics/blob/main/documentacion.md)** del repositorio, detallando los cambios realizados en los cálculos y visualizaciones.
     - También se creó un plan de pruebas detallado que se utilizó para verificar cada una de las funcionalidades interactivas del dashboard, lo que asegura que cualquier error encontrado pueda ser resuelto de manera eficiente.

### **Importancia de este paso**:
La **etapa de pruebas de calidad** es esencial para garantizar que el informe final entregue resultados precisos y confiables. La validación de los cálculos y la interacción de los filtros son fundamentales para asegurar que el dashboard sea una herramienta útil y efectiva para la toma de decisiones en **ComerLogistics**. Además, la optimización del rendimiento y la experiencia de usuario garantizan que el equipo de **ComerLogistics** pueda utilizar el dashboard de manera eficiente y sin problemas técnicos.

### **Siguientes pasos**:
- Ajustar cualquier detalle visual o técnico identificado durante las pruebas.
- Preparar el dashboard para su presentación final al cliente y al equipo de **ComerLogistics**.
- Realizar un seguimiento continuo del rendimiento y actualizar el informe según las necesidades futuras del cliente.

---

[Repositorio ComerLogistics en GitHub](https://github.com/Dapt01G2-Henry/ComerLogistics)

_____
