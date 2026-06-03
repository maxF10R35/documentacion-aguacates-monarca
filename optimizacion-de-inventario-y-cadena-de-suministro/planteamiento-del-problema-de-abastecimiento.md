# Planteamiento del Problema de Abastecimiento

### Sincronización Logística: El Rol del Almacenamiento Estacional (Cold Storage)

#### Dinámica Operativa del Flujo de Inventario

Para garantizar la máxima frescura del aguacate Hass en nuestro punto de venta ubicado en la alcaldía Tláhuac, la cadena de suministro de **Aguacates Monarca** opera bajo dos horizontes temporales complementarios: el ciclo de optimización diario en piso de venta (ejecutado mediante Programación Lineal) y la planeación de abastecimiento estratégico mensual (guiada por nuestro modelo econométrico SARIMAX).

Nuestra infraestructura local en Ciudad de México cuenta con una restricción de espacio físico fija, delimitada a un máximo de 35 cajas de inventario diario en bodega. Esta capacidad instalada está diseñada para cubrir de forma eficiente el flujo de transeúntes regular y los picos de demanda del fin de semana (sábados y domingos) , operando bajo una filosofía de _Just-In-Time_ para evitar mermas por sobremaduración, dado el comportamiento climatérico del fruto.

#### Integración de Ventanas de Oportunidad Macro-Económicas

El verdadero valor de integrar analítica predictiva en la PyME radica en la capacidad de anticipar anomalías y choques estacionales en el mercado de la Central de Abasto. Nuestro modelo de series de tiempo **SARIMAX $(1,0,2) \times (1,0,1)\_{12}$** identificó con un 95% de confianza que durante el mes de mayo de 2026 el precio frecuente de la caja de 9 kg se situó en un suelo histórico atípico de $350 MXN.

La inercia estacional capturada por el algoritmo predice un incremento acelerado en los costos de adquisición para el tercer trimestre del año debido a la baja producción estacional.Por ello, el sistema activa una directriz de **compra estratégica de inventario de respaldo** para congelar los costos operativos en $350 MXN antes de la corrección al alza del mercado.

#### Implementación Logística: Habilitación de Cold Storage Externo

Para ejecutar esta estrategia de protección financiera sin saturar la capacidad física de nuestra bodega comercial en Los Olivos, el diseño de nuestra cadena de suministro contempla la transición hacia un esquema híbrido mediante la **renta temporal de un espacio de almacenamiento en frío externo (Cold Storage)**.

Esta decisión de ingeniería logística se fundamenta en dos variables críticas:

* **Control Fenológico:** Mantener el stock de respaldo en una atmósfera refrigerada externa (entre 4°C y 5°C) ralentiza el metabolismo del aguacate, preservando la firmeza de la pulpa y deteniendo el proceso de maduración para asegurar que el fruto conserve su calidad premium al momento de ser introducido al mercado de Tláhuac.
* **Análisis de Trade-Off Financiero:** El costo marginal que representa el arrendamiento temporal del espacio de refrigeración de terceros se absorbe por completo por el diferencial de precios proyectado por el modelo SARIMAX. Adquirir volumen a gran escala bajo el costo de oportunidad de $350 MXN  y sumarle la tasa de almacenamiento externo resulta drásticamente más rentable que realizar compras spot ("al día") durante los meses de alta inflación del tercer trimestre.

A través de esta arquitectura unificada, los modelos predictivos dictan las alertas macroeconómicas, permitiéndonos expandir temporalmente nuestras fronteras físicas de almacenamiento para blindar el capital de trabajo y potenciar la rentabilidad general de la empresa.
