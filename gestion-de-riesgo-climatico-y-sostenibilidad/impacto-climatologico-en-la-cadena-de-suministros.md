# Impacto Climatológico en la cadena de suministros

### Modelado Estocástico de la Variabilidad Climática en Zitácuaro y su Impacto en la Cadena de Suministro

#### El Clima como Factor Crítico de Riesgo Operativo

En el sector agroindustrial, y específicamente en la cadena de valor del aguacate Hass, la meteorología no es una variable secundaria; es el motor biológico y logístico que determina la disponibilidad del producto, el precio en el mercado mayorista y la calidad en el punto de venta de Tláhuac. La región de Zitácuaro, Michoacán, cuenta con microclimas excepcionales que permiten cosechas continuas a lo largo de sus cuatro olas fenológicas (Loca, Aventajada, Normal y Marceña). Sin embargo, esta misma riqueza geográfica expone a la PyME a una fuerte incertidumbre climatológica.

Para transicionar de una gestión reactiva y empírica hacia una estrategia de **Inteligencia de Abastecimiento**, implementamos un análisis predictivo basado en Cadenas de Markov de tiempo discreto. El objetivo central de este modelo es decodificar la probabilidad de transición diaria entre tres estados meteorológicos fundamentales: Soleado (s\_1), Sol/Lluvia (s\_2) y Lluvia Continua (s\_3), cubriendo un horizonte temporal crítico de 91 días (correspondiente al trimestre de transición productiva).

***

#### &#x20;Matriz de Transición del clima de Zitacuaro

El análisis estocástico se fundamenta en la recopilación de frecuencias y transiciones reales observadas en la zona durante un muestreo base de 30 días, el cual registró un comportamiento inicial de 12 días soleados, 16 días mixtos y 2 días lluviosos. A partir de estos registros, la matriz de transición de estados P queda correctamente definida por su notación decimal pulcra, garantizando la condición de cerradura donde cada fila (intensidad de probabilidad de cambio) suma exactamente 1:

$$P = \begin{pmatrix} 0.667 & 0.333 & 0.000 \\ 0.200 & 0.667 & 0.133 \\ 0.000 & 1.000 & 0.000 \end{pmatrix}$$

Al ejecutar la simulación multi-paso mediante el producto estocástico ( $$v_{t+1} = v_t / P$$ ), el sistema estabiliza sus tendencias rápidamente a partir de la segunda semana, convergiendo de manera óptima hacia un **Estado Estable** definitivo para el trimestre:

**Probabilidad de días Mixtos ($s\_2$):** 50.0% (Mañanas soleadas con intervalos de chubascos vespertinos).

**Probabilidad de días Soleados (s\_1):** 37.5% (Alta radiación solar limpia).

**Probabilidad de días Lluviosos (s\_3):** 12.5% (Precipitaciones continuas o tormentas).

***

#### El Impacto Operativo Interconectado: De la Simulación a la Acción Comercial

La importancia de este 62.5% de probabilidad conjunta de eventos pluviales (sumando el estado mixto y de lluvia continua) radica en cómo sus consecuencias se conectan directamente con los módulos logísticos y comerciales que resolvimos previamente en nuestro proyecto:

**Optimización del Fertirriego y Conservación de Suelos**

Los suelos de Zitácuaro son de origen volcánico (Andosoles), caracterizados por una excelente porosidad pero altamente susceptibles a la lixiviación. El modelo estocástico nos advierte que un 12.5% de días bajo tormentas continuas provocará el "lavado" de macroelementos esenciales (nitrógeno y potasio) hacia capas profundas del subsuelo, lejos de la zona radicular activa del árbol. Esta alerta matemática permite a la empresa anticipar planes de fertirriego inmediato y colocar coberturas vegetales orgánicas (_mulch_) en el cajete para mitigar la erosión y el aborto mecánico del fruto.

&#x20;**Reducción de Costos Energéticos vs. Presión Fitosanitaria**

El aporte hídrico natural del trimestre beneficia el llenado y calibre del aguacate sin necesidad de activar sistemas de bombeo artificial, disminuyendo drásticamente el costo de energía eléctrica de la organización. No obstante, el 50% de probabilidad en el estado mixto (s\_2) genera un "efecto incubadora" (humedad relativa elevada combinada con temperaturas templadas) idóneo para la proliferación del hongo _Phytophthora cinnamomi_ (tristeza del aguacate). El modelo actúa aquí como un sistema de alerta temprana para calendarizar aplicaciones preventivas de control biológico antes de que se afecte el estándar de calidad comercial.

**Sincronización Logística y Suministro en Piso de Venta**

Finalmente, este modelo se acopla de forma armónica con nuestra programación lineal diaria. Cuando las Cadenas de Markov proyectan días bajo el estado soleado (s\_1), las carreteras de la ruta Zitácuaro-CDMX se reportan seguras y el fruto alcanza su firmeza premium óptima para traslado en la Nissan de 1 tonelada. Esto expande geométricamente nuestra **Región Factible** de compra, otorgando luz verde para ejecutar la carga óptima calculada de 16 cajas en Michoacán y 10 cajas en la Central de Abasto, maximizando la ganancia real de $3,811.40 MXN sin comprometer la seguridad logística ni saturar la capacidad del almacén comercial. <br>

#### Nota Técnica: Glosario de Conceptos Agronómicos y Fenológicos

Para facilitar la comprensión del impacto que tienen las Cadenas de Markov y la variabilidad climática en la operación de **Aguacates Monarca**, se detallan a continuación los fundamentos científicos de los términos clave utilizados en este estudio:

**Lixiviación:** Es el proceso de lavado, separación o disolución de los nutrientes solubles del suelo (como el nitrógeno y el potasio) debido al paso vertical del agua de lluvia intensa.En los suelos de Zitácuaro, las precipitaciones continuas arrastran estos elementos hacia capas profundas del subsuelo donde las raíces del aguacate ya no pueden absorberlos, provocando deficiencias nutricionales si no se mitiga a tiempo.

**Fruto Climatérico:** Es una clasificación biológica que reciben los frutos (como el aguacate Hass) capaces de seguir madurando de manera acelerada una vez que han sido recolectados o cortados del árbol. Esta maduración se debe a un aumento endógeno en la producción de gas etileno y en la tasa de respiración celular del fruto, lo que exige una estricta coordinación logística y de cadena de frío para evitar que el producto llegue sobremadurado al punto de venta en Tláhuac.

**Olas Fenológicas:** Se refiere a las distintas etapas o fases visibles del ciclo de desarrollo biológico de la planta a lo largo del año (como la floración, el amarre y el crecimiento del fruto). En Michoacán, las condiciones del suelo y los microclimas permiten la coexistencia de cuatro olas de producción anuales conocidas localmente como: _Loca, Aventajada, Normal y Marceña_.

**Suelos Andosoles:** Son suelos de origen volcánico altamente fértiles, caracterizados por una estructura oscura, ligera, con una alta porosidad y una excelente capacidad de retención de humedad. Aunque son ideales para el cultivo del aguacate, su textura los vuelve vulnerables a la pérdida de nutrientes por escorrentía o lixiviación ante tormentas continuas.

* **Presión Fitosanitaria:** Es el grado de riesgo o la fuerza con la que los agentes biológicos nocivos (como plagas, insectos o enfermedades fúngicas) amenazan la salud y productividad de un cultivo en un momento determinado. En nuestro modelo, el estado mixto de Sol/Lluvia eleva esta presión al crear las condiciones de humedad y temperatura perfectas para la incubación de hongos patógenos.
* **Phytophthora cinnamomi (Tristeza del Aguacate):** Es un organismo de la clase de los oomicetos (comúnmente clasificado como hongo) que ataca de forma agresiva el sistema radicular del árbol de aguacate. Destruye las raíces encargadas de absorber agua y nutrientes, provocando marchitamiento, caída del fruto y, en casos graves, la muerte del árbol. Su monitoreo es vital durante los meses con alta probabilidad de humedad estagnada.

