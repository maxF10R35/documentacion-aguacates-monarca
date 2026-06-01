# Fluctuación Histórica de Precios

Una vez determinada la capacidad productiva de los cultivos de origen, el siguiente pilar para asegurar la continuidad operativa de "Aguacates Monarca" es el análisis del mercado secundario de abastecimiento. Durante las temporadas de baja producción en Michoacán, la empresa debe recurrir a la Central de Abasto de Iztapalapa (CDMX) para surtir su inventario y cumplir con sus compromisos comerciales. Dado que el aguacate Hass es un _commodity_ altamente sensible a factores externos, comprender la estructura de precios en este mercado es vital para mitigar el riesgo de sobrecostos.

Para entender el panorama general, se analizó inicialmente la fluctuación histórica del precio promedio nacional por kilogramo. Como se observa en la Figura 7, el mercado ha mantenido una tendencia inflacionaria constante a lo largo de las últimas dos décadas, salpicada por picos de volatilidad agresivos. Sin embargo, para que el modelo financiero de la empresa sea operativo, fue necesario "aterrizar" esta macroeconomía a la unidad de compra real: la caja de 9 kilogramos en la Central de Abasto de CDMX.

<figure><img src=".gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

> _Figura 7: Fluctuación Histórica del Precio Promedio Nacional del Aguacate Hass (MXN/kg)._ Elaboración propia.

Al aislar los registros del Sistema Nacional de Información e Integración de Mercados (SNIIM) para la presentación de 9 kg durante el periodo 2018-2025, la volatilidad en los costos de adquisición se hace evidente (Figura 8). Las severas oscilaciones demuestran que planificar el presupuesto de compras para las temporadas de escasez basándose en promedios simples representa un riesgo inaceptable para el flujo de caja de la empresa.

<figure><img src=".gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

> _Figura 8: Fluctuación Histórica del Precio Frecuente (Caja 9kg) en CDMX (2018-2025)._ Elaboración propia con datos del SNIIM.

Para decodificar este comportamiento errático del costo de inventario, la serie de tiempo fue sometida a un algoritmo de descomposición estacional aditiva (Figura 9), revelando los tres componentes fundamentales del mercado mayorista:

1. Tendencia Macroeconómica: Muestra la base inflacionaria del costo de la caja de 9 kg a lo largo de los años, indicando un encarecimiento generalizado del abastecimiento externo.
2. Ciclo Estacional: Revela una onda cíclica y repetitiva que dicta automáticamente ventanas de sobreprecio. Esta inteligencia de mercado es crucial: permite a la empresa identificar exactamente cuántos pesos adicionales costará surtir el inventario en Iztapalapa durante los meses de déficit productivo local.
3. Ruido y Anomalías: Aísla los choques externos (crisis climáticas, desabasto o bloqueos logísticos), destacando periodos atípicos donde el costo de adquisición sufrió distorsiones masivas e impredecibles.

<figure><img src=".gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

> _Figura 9: Descomposición de la Serie de Tiempo (Caja 9kg). Análisis de tendencia, estacionalidad y ruido de mercado._ Elaboración propia.









