---
description: >-
  Modelo para predecir el volumen de toneladas por hectárea en función del
  estado y la superficie sembrada.
---

# Proyección de Rendimiento (Árbol de Regresión)

Tras identificar que la expansión territorial del cultivo de aguacate en Michoacán enfrenta una desaceleración natural, el enfoque estratégico del análisis debe transitar hacia la eficiencia operativa. El objetivo central de esta fase es determinar la capacidad productiva esperada por cada unidad de tierra sembrada. Para modelar el Rendimiento Agrícola (Toneladas / Hectáreas), se optó por un algoritmo de Árbol de Regresión (Decision Tree Regressor). A diferencia de los modelos lineales o polinomiales, los árboles de decisión son idóneos para detectar "umbrales" o "escalones" operativos, aislando los periodos exactos en los que la industria experimentó cambios drásticos en su eficiencia.

Al entrenar el modelo limitando su profundidad para evitar el sobreajuste (_overfitting_), se obtuvo un Coeficiente de Determinación (R2) de 0.7604 y un Error Cuadrático Medio (RMSE) de 0.29 Ton/Ha. Estas métricas indican que el modelo captura el 76% de la varianza histórica, logrando un poder predictivo sumamente alto con un margen de error estadístico mínimo (apenas 290 kilogramos por hectárea de desviación promedio).

La estructura de los nodos del árbol revela el verdadero comportamiento del mercado michoacano a través de distintas épocas productivas:

* Periodo histórico base (Año <= 2018.5): La industria mantuvo un umbral de rendimiento promedio de 9.97 Ton/Ha, con un error muy bajo (RMSE = 0.17).
* Fase de transición (Año <= 2022.5): Se observa una consolidación en torno a las 10.06 Ton/Ha, marcando una década de eficiencia estable pero sin crecimientos disruptivos.
* El salto de eficiencia reciente (Año > 2022.5): El nodo terminal más reciente del modelo revela un quiebre operativo extraordinario. Para los registros posteriores a 2022, el rendimiento promedio se dispara a 12.13 Ton/Ha.

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

> _Figura 6: Estructura del Árbol de Regresión. Umbrales históricos de rendimiento agrícola en Michoacán._ Elaboración propia.

**Proyección Operativa para "Aguacates Monarca"**

El algoritmo no solo describe la historia, sino que funciona como un simulador directo para las proyecciones logísticas y financieras de la empresa. Tomando como anclaje predictivo el nodo terminal más reciente (12.13 Ton/Ha), se dimensionó la capacidad productiva de las 10 hectáreas operadas por "Aguacates Monarca" en el municipio de Zitácuaro.

* Volumen Anual Proyectado: 10 Hectáreas × 12.13 Ton/Ha = 121.3 Toneladas brutas.
* Unidades de Comercialización: 121,300 kg / 9 kg = 13,477 cajas estándar.

Gracias al bajo nivel de error del modelo (RMSE = 0.29), este cálculo cuenta con una desviación de apenas $$ $\pm$ $$ 2.9 toneladas para toda la parcela. Logísticamente, la dirección operativa de la PyME puede asegurar la contratación de transporte de carga y almacenamiento en frío para un volumen que oscilará de manera segura entre 118.4 y 124.2 toneladas.

Es importante destacar que este cálculo representa la _capacidad instalada histórica_ de un ciclo anual exitoso. Aunque reportes intermedios (como las cifras semestrales del SIAP a junio de 2024) pueden mostrar caídas temporales por condiciones climáticas, la meta estratégica de "Aguacates Monarca" es apalancar prácticas de agricultura intensiva para asegurar que sus 10 hectáreas alcancen el umbral de las 12.13 Ton/Ha dictado por la máxima eficiencia del modelo estadístico.
