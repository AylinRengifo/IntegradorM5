###   <center> TRABAJO INTEGRADOR MODULO 5 
###   <center>  CALL CENTER 


<!DOCTYPE html>
<html>
<head>
<style>
.center-image {
  display: flex;
  justify-content: center;
  height: 25vh;
}
</style>
</head>
<body>
<div class="center-image">
  <img src="https://media.tenor.com/WEl1mDNm4tYAAAAi/pretty-cute.gif" alt="wink">
</div>

# Índice 
<details>
  <summary>Tabla de contenido</summary>
  <ol>  
    <li><a href="#Introducción">Introducción</a></li>
    <li><a href="#ETL">ETL</a></li>
    <li><a href="#EDA">EDA</a></li>
    <li><a href="#KPIs">KPIs</a></li>
    <li><a href="#Dashboard">Dashboard</a></li>
    <li><a href="#Conclusiones">Conclusiones</a></li>
  </ol>
</details>

</body>
</html>


## Introducción

En este proyecto integrador, se llevó a cabo un análisis exhaustivo del Call Center del banco Anonymous Bank, ubicado en Israel. El Call Center desempeña un papel fundamental en el servicio al cliente, ya que es el principal punto de contacto para resolver consultas, brindar asistencia y gestionar reclamos.El análisis se basó en un conjunto de datos que contenía información sobre las llamadas registradas durante todo un año. Se examinaron diversos aspectos, como el tiempo de espera en la cola, el tiempo de atención, la prioridad otorgada a los clientes y los tipos de servicios brindados durante las llamadas.

Para llevar a cabo este análisis, se utilizó el lenguaje de programación Python, aprovechando diversas bibliotecas como Pandas, Seaborn y Matplotlib, entre otras. El proceso comenzó con la extracción, transformación y carga de los datos (ETL), seguido de un análisis exploratorio de datos (EDA). A continuación, se extrajo la información relevante y se utilizó Power BI para crear un panel de control con indicadores clave de rendimiento (KPIs).

En resumen, este proyecto integrador combinó el análisis de datos utilizando Python y diversas bibliotecas, junto con el uso de Power BI para crear un panel de control con KPIs, con el objetivo de comprender y optimizar el rendimiento del Call Center del banco Anonymous Bank.

## ETL (Extracción, Transformación, Carga)

En el proceso de ETL, se llevaron acabo los siguientes pasos para extraer y transformar los datos del archivo CSV:

- <b>Extracción:</b> Se extrajeron los datos del archivo CSV utilizando las herramientas adecuadas. Esto implicó leer el archivo y cargarlo en un dataframe para su posterior procesamiento.

- <b>Transformación:</b> Durante esta etapa, se aplicaron diversas operaciones para limpiar y preparar el dataset. A continuación, se detallan algunas de las transformaciones realizadas:

 <ul>Limpieza de valores nulos: Se verificó la presencia de valores nulos en el dataset y se tomaron las medidas necesarias para manejarlos adecuadamente. En este caso, se encontró que no había valores nulos en el dataset.

 Tratamiento de valores negativos: Se identificaron valores negativos en el dataset y se decidió cambiarlos por el valor 0 para evitar distorsiones en los cálculos y análisis posteriores.

 Eliminación de valores duplicados: Se detectaron valores duplicados en el dataset y se tomó la decisión de crear una nueva columna en la tabla que combinara dos columnas existentes para identificar y eliminar los duplicados.

 Análisis y ajuste de tipos de datos: Se examinaron los tipos de datos de cada columna y se les asignó el dtype adecuado para facilitar el procesamiento y análisis de los datos. Esto aseguró que los cálculos y operaciones se realizaran correctamente. </ul>

- <b>Carga:</b> Una vez finalizadas las transformaciones, se guardó el dataframe resultante en un nuevo archivo CSV. Esto permitió conservar los cambios realizados y tener una versión actualizada y lista para su posterior uso en análisis o visualizaciones.

En resumen, el proceso de ETL involucró la extracción de datos del archivo CSV, seguida de diversas transformaciones para limpiar y preparar el dataset. Se realizaron operaciones como la eliminación de valores nulos, el tratamiento de valores negativos, la eliminación de duplicados y el ajuste de tipos de datos. Finalmente, se guardó el dataframe transformado en un nuevo archivo CSV.


## EDA (Análisis de Datos Exploratorio)

Después de completar el proceso de ETL, se realizó un Análisis Exploratorio de Datos (EDA) para obtener una comprensión más profunda de los datos. Durante el EDA, se llevaron a cabo las siguientes tareas:

- <b> Visualización detallada de cada variable: </b>  Se examinó cada variable en el dataframe para comprender su distribución y características. Se utilizaron diferentes tipos de gráficos, como histogramas, gráficos de dispersión, diagramas de caja, gráficos de barras y gráficos de torta, entre otros. Estas visualizaciones permitieron identificar patrones, tendencias, relaciones y posibles valores atípicos en los datos.

- <b> Cálculo de estadísticas descriptivas: </b>  Se utilizaron medidas estadísticas básicas, como la media, la mediana, la desviación estándar, el mínimo y el máximo, para obtener una comprensión más precisa de la distribución y la variabilidad de los datos. Estas estadísticas proporcionaron información sobre la tendencia central, la dispersión y los valores extremos de cada variable.

- <b> Identificación y manejo de valores atípicos: </b>  Durante el EDA, se identificaron valores atípicos o outliers en los datos. Estos valores se consideraron inusuales o extremos en comparación con el resto de los datos. En la mayoría de los casos, se decidió eliminar estos valores atípicos, ya que no representaban un porcentaje significativo del conjunto de datos y podrían distorsionar los resultados del análisis posterior.

El EDA es una etapa importante para comprender la naturaleza de los datos y tomar decisiones informadas sobre el análisis posterior. Al realizar visualizaciones detalladas, calcular estadísticas descriptivas y manejar valores atípicos, se obtiene una visión más completa y precisa de los datos.


## KPIs

En este proyecto, se utilizaron los siguientes KPIs (Indicadores Clave de Desempeño):

- <b>Tiempo promedio de espera en la cola: </b>  Este KPI mide la eficiencia del call center en términos del tiempo que los clientes esperan en la cola antes de ser atendidos por un agente.

- <b>Tiempo promedio de servicio: </b>  Este KPI proporciona información sobre la eficiencia de los agentes del call center al atender las solicitudes de los clientes. Mide el tiempo promedio que se tarda en resolver cada solicitud.

- <b>Tasa de abandono de llamada:</b>  Este KPI representa el porcentaje de llamadas que se cortan sin recibir ningún servicio. Puede indicar la satisfacción de los clientes y la eficiencia del call center en la gestión de las llamadas entrantes.

- <b>Distribución de tipos de servicios:</b>  Este KPI analiza la proporción de los diferentes tipos de servicios solicitados por los clientes. Ayuda a identificar las áreas de mayor demanda y asignar los recursos adecuadamente.

- <b>Distribución de prioridades de los clientes: </b>  Este KPI permite comprender la proporción de clientes de alta prioridad en comparación con los clientes regulares y cómo se gestionan sus solicitudes.

Estos KPIs son herramientas importantes para evaluar el desempeño y la eficiencia del call center. Proporcionan información clave sobre el tiempo de espera, la calidad del servicio y la gestión de las llamadas, lo que ayuda a tomar decisiones informadas para mejorar la atención al cliente.

## Dashboard

Se creó un hermoso panel de control en Power BI para resumir visualmente la información obtenida en este proyecto. Este panel de control integra elementos visuales interactivos que permiten apreciar los cambios y detalles al hacer clic en cada uno de ellos. El objetivo principal de este panel de control es facilitar la explicación de los conocimientos adquiridos durante el proyecto. Al presentar la información de manera visual, se logra una comprensión más clara y accesible para todos los interesados.

El uso de elementos visuales interactivos en el panel de control brinda una experiencia dinámica y atractiva. Al hacer clic en cada elemento, se pueden explorar los detalles y obtener una visión más profunda de los datos. Este panel de control en Power BI es una herramienta poderosa que permite comunicar de manera efectiva los hallazgos y conclusiones del proyecto. Facilita la presentación de información compleja de una manera visualmente atractiva y comprensible.


## Conclusiones

Después de realizar un análisis exhaustivo del Call Center del banco Anonymous Bank, se han obtenido varias conclusiones importantes. A continuación se presentan algunas de las conclusiones más relevantes:

- <b> Nivel de servicio para los clientes prioritarios: </b> Los clientes prioritarios reciben un trato preferencial en el Call Center. Se les asigna un tiempo de espera más corto al comienzo de su llamada y están exentos de pagar una tarifa mensual. Esto demuestra que el banco se preocupa por brindar un servicio de calidad a sus clientes prioritarios, el tiempo promedio de espera para los clientes de alta prioridad es de 86 segundos.

- <b> Comparación con los clientes normales: </b> Los clientes prioritarios reciben un mejor servicio en términos de tiempo de espera y atención. Sin embargo, es importante tener en cuenta que los clientes normales también reciben un nivel de servicio adecuado.

- <b>Volumen de llamadas atendidas:</b> Durante el período analizado, el Call Center del banco Anonymous Bank atendió un alto volumen de llamadas. Se registraron entre 20.000 y    30.000 llamadas por mes, lo que indica una alta demanda de servicios por parte de los clientes, en promedio se atienden 37 mil llamadas por mes

- <b>Identificación de cuellos de botella:</b>  Durante el análisis, se identificaron ciertos días y bandas horarias en las que se producían cuellos de botella en el Call Center. Estos períodos de alta demanda podrían requerir una mayor dotación de personal o una mejor distribución de recursos para garantizar un servicio eficiente.

- <b> Tipos de servicio más recurrentes:</b> Durante el análisis, se identificaron los tipos de servicio más recurrentes en el Call Center. Esto puede ayudar al banco a enfocar sus esfuerzos en mejorar la calidad y eficiencia de estos servicios específicos, el 68% de los clientes fueron atendidos por Actividades Regulares

En resumen, el análisis exhaustivo del Call Center del banco Anonymous Bank ha proporcionado información valiosa sobre el nivel de servicio, volumen de llamadas, eficiencia de los agentes y otros aspectos clave. Estas conclusiones pueden servir como base para tomar decisiones estratégicas y mejorar la calidad y eficiencia del servicio brindado a los clientes.