# gustos de los clientes

Tenemos como propósito aplicar los principios y técnicas de la minería de datos sobre la información recolectada a través de la encuesta realizada sobre los hábitos, preferencias y percepciones de compra del aguacate, con el objetivo de comprender a fondo cómo funciona este mercado local, identificando  las asimetrías, desigualdades y retos que enfrentan tanto vendedores como consumidores, y proponer acciones orientadas a construir una mejor experiencia, transparente y equitativo. Partiremos organizando, limpiando y estructurando toda la información obtenida, siguiendo las etapas clásicas de extracción, transformación y carga, para convertir datos crudos en información confiable y útil, considerando siempre la realidad del entorno rural y comercial, donde suelen existir registros incompletos, informalidad y diferencias en el acceso a la información. Posteriormente, aplicaremos metodologías como CRISP‑DM para buscar patrones, relaciones y tendencias en las respuestas, analizando aspectos como la influencia del precio, los lugares de compra, las características que más se valoran y la forma en que las personas se informan, lo que nos permitirá detectar dónde se generan las ventajas o desventajas entre los distintos actores de la cadena. Todo este análisis se realizará con una mirada crítica y ética, cuestionando de dónde viene la información, qué sesgos puede tener y cómo su interpretación puede favorecer o perjudicar a ciertos grupos, para finalmente utilizar ese conocimiento como base para diseñar estrategias y soluciones que no solo mejoren la eficiencia del comercio, sino que también fortalezcan a los pequeños productores y comerciantes, acerquen la información a los consumidores y contribuyan a un desarrollo más justo, conectado y beneficioso para toda la comunidad.

Para esta materia, usaremos la encuesta que hicimos para conocer en que se fijan los clientes al momento de comprar aguacate.

<img src="../.gitbook/assets/unknown (2).png" alt="Obtuvimos 101 resultados. Imagen propia" height="144" width="602">

En Marketing digital los datos nos sirvieron para conocer los gustos de los clientes, pero también puede servir para dar con patrones que pueden ser de importancia.

<img src="../.gitbook/assets/unknown (3).png" alt="La dispersión de los diferentes gustos que tienen los clientes. Imagen propia" height="461" width="602">

Los grupos están bien separados, lo que significa que realmente hay diferentes tipos de consumidores de aguacate

El grupo azul  (Cluster 1) parece ser el más grande o el más concentrado

Los grupos amarillo y verde están más dispersos, lo que podría indicar que tienen preferencias más variadas o que hay menos clientes de esos tipos.

minería de patrones: market basket analysis

Se analizó la encuesta de clientes de aguacate para entender cómo se comportan los diferentes grupos de edad. Se revisaron las respuestas de tres preguntas clave: dónde compran, si el precio les parece accesible y qué harían si el precio sube.

<img src="../.gitbook/assets/unknown (4).png" alt="&#x22;Los adultos jóvenes (18 a 29 años) perciben el precio del aguacate como poco accesible y ante una subida reducirían su consumo, mientras que los adultos de 30 a 49 años lo consideran justo y también moderarían su compra; ambos grupos cambiarían su cantidad, pero no dejarían de comprar.&#x22;. Imagen propia" height="361" width="602">

<img src="../.gitbook/assets/unknown (5).png" alt="&#x22;Más de la mitad de los adultos mayores de 50 años perciben el precio del aguacate es poco accesible y frente a un aumento reducirían su consumo, pero sin dejar de comprarlo, manteniéndose fieles a las recauderías o locales establecidos.&#x22; imagen propia" height="163" width="602">

Para hacer el análisis, se separaron los clientes por edad: jóvenes de 18 a 29 años, adultos de 30 a 49 años y mayores de 50 años. En cada grupo se identificó la respuesta más común, es decir, lo que la mayoría dijo.

Los resultados mostraron que los tres grupos coinciden en algo importante: todos sienten que el precio actual del aguacate no es accesible. Sin embargo, cada grupo reacciona diferente ante un posible aumento.

minería de marketing:

se construyó el perfil del cliente típico. Este se obtiene calculando la respuesta más frecuente en cada pregunta, lo que se conoce estadísticamente como la moda. El resultado mostró que el cliente más común tiene entre 18 y 29 años, compra en tianguis, prefiere el aguacate maduro, valora principalmente la frescura, compra con frecuencia de dos a tres veces por semana y considera que el precio actual no es accesible. Luego se analizaron los segmentos por edad por separado, porque cada grupo se comporta de manera distinta. Los jóvenes de 18 a 29 años compran en tianguis, sienten el precio caro y ante una subida dejarían de comprar hasta que baje. Los adultos de 30 a 49 años compran en recauderías, también sienten el precio caro, pero su reacción sería comprar menos cantidad, no dejar de comprar por completo. Los mayores de 50 años compran en puestitos de la calle, también perciben el precio como no accesible y, al igual que los jóvenes, dejarían de comprar si el precio aumenta.

<img src="../.gitbook/assets/unknown (6).png" alt="El tianguis es el canal de compra preferido por los clientes de aguacate, con 41 compradores, seguido por las recauderías con 28 y los puestos callejeros con 25, mientras que el supermercado es el menos utilizado con solo 6 clientes. Imagen propia" height="299" width="602">

<img src="../.gitbook/assets/unknown (7).png" alt="&#x22;Ante un aumento en el precio del aguacate, la mayoría de los clientes (47) optaría por comprar menos cantidad, mientras que 28 lo buscarían más barato en otro lugar, 22 dejarían de comprarlo temporalmente y solo 3 mantendrían su consumo sin cambios.&#x22; Imagen propia" height="373" width="602">

Cliente tipico: 18 a 29, compra en tianguis, busca que tenga un tamaño adecuado

Canal principal: tianguis con 41 clientes

problema principal: 54 de 100 clientes sienten el precio caro

Riesgo: 22 clientes dejarian de comprar si el precio sube

Oportunidad: Los jovenes son 59 de 100 clientes (59%)

RECOMENDACIONES:

&#x20; atraer a los clientes que comprar en el tianguis

&#x20; Dirigir ofertas a jovenes de 18 a 29 años (mayor segmento)

&#x20; Destacar frescura y sabor en la comunicacion

&#x20; Ofrecer promociones por volumen para retener a los sensibles al precio

\
\
\
\
<br>
