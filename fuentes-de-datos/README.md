# Fuentes de Datos

Se consultaron en el Sistema Nacional de Información e Integración de Mercados (SNIIM) los precios del aguacate Hass de primera, abarcando el periodo desde 2001 hasta 2026. Mediante un proceso de _web scraping_ utilizando la librería BeautifulSoup de Python, se lograron extraer 717,114 registros conformados por 8 columnas: Fecha, Presentación, Origen, Destino, Precio Min, Precio Max, Precio Frec y Obs.

Para la limpieza de la base de datos, se eliminaron 478,076 registros duplicados. Tras esta depuración, se conservaron 239,038 registros, los cuales representan el 33.33% del total extraído inicialmente. Al analizar la distribución de valores nulos, se observó que en la columna 'Obs' el 73.19% de los campos estaban vacíos. Al tratarse de datos de tipo _string_, no existía un método de imputación efectivo, a diferencia del resto de las columnas cuyo porcentaje de nulos no superaba el 5%; por lo tanto, se tomó la decisión de descartar la columna 'Obs'.

Antes de eliminarla definitivamente, se aplicó minería de textos a las observaciones que contenían información. En el primer conteo de palabras se detectaron cifras numéricas con formato de precio. Al inspeccionar a detalle los registros con estas anomalías, se descubrió que la información de un bloque considerable de filas se había desplazado, dejando la columna 'Precio Min' vacía. Esto explicaba la alta concentración de valores nulos en dicha variable. Después de realinear los registros a sus columnas correspondientes, se realizó un nuevo conteo de palabras en 'Obs', concluyendo que no aportaba información relevante para el estudio.

Para finalizar la limpieza, se eliminaron las filas que aún contenían valores nulos, consolidando un conjunto final de 231,678 registros. Esto representa una tasa de retención del 96.92% respecto a la base libre de duplicados.

Dado que los precios registrados estaban en función de diferentes presentaciones, pesos y empaques, los patrones resultaban inconsistentes para el modelado matemático. Para dar solución a esto y homogeneizar la información, se derivó una nueva variable denominada 'Precio Kg', la cual estandariza el costo por kilogramo. Asimismo, para facilitar la partición temporal, se agregaron dos columnas correspondientes al mes y al año.

Finalmente, el _dataset_ procesado se exportó en formato `.parquet`. De forma paralela, se extrajo una subtabla con las fechas y el precio promedio por kilogramo, creando así la serie temporal estructurada que alimentará la regresión del modelo ARIMA y el posterior entrenamiento de la red neuronal LSTM

{% embed url="http://www.economia-sniim.gob.mx/nuevo/Home.aspx" %}

En el caso de la producción de Aguacate, se consultó al Servicio Nacional de Sanidad, Inocuidad y Calidad Agroalimentaria. Dado que los datos eran solicitados a una API de Power BI, se usó el análisis de las respuestas en formato json y se recolectaron 405 registros que van desde el 2001 hasta el 2023. Las columnas que conforman este dataset son: Estado, Superficie Sembrada en hectáreas (ha), Volumen Cocechado en Toneladas, Valor que tiene la Cocecha en Pesos Mexicanos y Año de análisis.



{% embed url="https://dj.senasica.gob.mx/sias/Statistics/Transversal/EstadisticaProduccionAguacate" %}

