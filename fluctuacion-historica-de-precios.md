# Fluctuación Histórica de Precios

Una vez determinada la capacidad productiva física de la tierra, el siguiente pilar para asegurar la viabilidad financiera de "Aguacates Monarca" es el análisis del comportamiento de los precios en su principal punto de venta: la Central de Abasto. El aguacate Hass es un _commodity_ agrícola caracterizado por una alta sensibilidad a factores externos, lo que genera una estructura de precios sumamente dinámica.

Para entender el panorama general, se analizó inicialmente la fluctuación histórica del precio promedio nacional por kilogramo. Como se observa en la Figura 7, el mercado ha mantenido una tendencia inflacionaria constante a lo largo de las últimas dos décadas, salpicada por picos de volatilidad agresivos. Sin embargo, para que el modelo financiero de la empresa sea operativo, fue necesario "aterrizar" esta macroeconomía a la unidad de comercialización real: la caja de 9 kilogramos proveniente de Michoacán.

<figure><img src=".gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

> _Figura 7: Fluctuación Histórica del Precio Promedio Nacional del Aguacate Hass (MXN/kg)._ Elaboración propia.

Al aislar los registros del Sistema Nacional de Información e Integración de Mercados (SNIIM) para la presentación de 9 kg durante el periodo 2018-2025, la volatilidad operativa se hace evidente (Figura 8). Las severas oscilaciones demuestran que la planeación financiera basada en promedios simples representa un riesgo inaceptable para la rentabilidad de la cadena de suministro.

<figure><img src=".gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

> _Figura 8: Fluctuación Histórica del Precio Frecuente (Caja 9kg) en CDMX (2018-2025)._ Elaboración propia con datos del SNIIM.

Para decodificar este comportamiento errático, la serie de tiempo fue sometida a un algoritmo de descomposición estacional aditiva (Figura 9), revelando los tres componentes fundamentales que dictan el mercado:

1. Tendencia Macroeconómica: Muestra la base inflacionaria y el valor de apreciación del producto, aislando los picos temporales.
2. Ciclo Estacional: Revela una onda cíclica y repetitiva que dicta automáticamente ventanas de sobreprecio y depreciación según el mes del año. Esta inteligencia de mercado es vital para la estrategia logística y comercial de la empresa.
3. Ruido y Anomalías: Aísla los choques externos (como crisis climáticas o logísticas), destacando periodos atípicos donde el precio sufrió distorsiones masivas.

<figure><img src=".gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

> _Figura 9: Descomposición de la Serie de Tiempo (Caja 9kg). Análisis de tendencia, estacionalidad y ruido de mercado._ Elaboración propia.









