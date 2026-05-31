---
description: >-
  Ajuste de curvas para entender el crecimiento no lineal del cultivo en
  Michoacán.
---

# Tendencias de Producción (Regresión Polinomial)

El crecimiento del sector agroalimentario rara vez obedece a un comportamiento perfectamente lineal, ya que se ve influenciado por periodos de auge económico, límites físicos territoriales y la adopción de nuevas tecnologías. Para comprender la trayectoria evolutiva específica del estado de Michoacán, se implementó un modelo de regresión polinomial sobre los datos históricos de superficie sembrada y volumen de producción.

Para garantizar la estabilidad numérica del algoritmo y evitar el desbordamiento de varianza, se realizó un escalado de la variable independiente temporal, tomando el año 2000 como punto de origen ($$X = \text{Año} - 2000$$). El modelo ajustado responde a la ecuación general polinomial:

$$
Y = \beta_0 + \beta_1 X + \beta_2 X^2 + \dots + \beta_n X^n + \epsilon
$$

Los resultados del entrenamiento revelaron un ajuste matemático excepcional para un polinomio de Grado 3, obteniendo un Coeficiente de Determinación ($$ $R^2$ $$) de 0.9890 para la expansión territorial y de 0.9755 para el volumen cosechado. Esto demuestra que el crecimiento histórico de la industria aguacatera en la región obedece a un patrón estadísticamente predecible.

<figure><img src="../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

> _Figura 4: Tendencia de Crecimiento del Volumen en Michoacán. Ajuste polinomial de la curva de producción._ Elaboración propia.

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

> _Figura 5: Tendencia de Crecimiento de la Superficie en Michoacán. Ajuste polinomial de la expansión territorial._ Elaboración propia.

**Proyecciones a Corto Plazo (2024-2025) y Realidad del Mercado**

Para dotar a la planificación estratégica de "Aguacates Monarca" con inteligencia anticipatoria, se extrapoló el algoritmo para proyectar el comportamiento del mercado michoacano en el bienio siguiente. Las estimaciones matemáticas del modelo proyectaron una superficie sembrada de 186.64 miles de hectáreas y un volumen de 2,106.42 miles de toneladas para el cierre de 2024. Para 2025, el modelo previó una expansión hacia las 193.46 miles de hectáreas y 2,216.74 miles de toneladas.

Sin embargo, al contrastar este escenario matemático con el avance real reportado por el SIAP a junio de 2024, se hace evidente una fuerte fricción en el mercado. A mitad del año, Michoacán reportó una superficie sembrada de 175,012 hectáreas, lo que representa la disminución más significativa del país con 4,902 hectáreas menos (2.7%) respecto al mismo periodo de 2023. En términos de volumen, la región líder produjo 917,329 toneladas en el primer semestre , evidenciando también una caída impulsada no solo por la pérdida de hectáreas, sino por una baja generalizada en los rendimientos nacionales, los cuales pasaron de 5.7 toneladas por hectárea en 2023 a 5.5 toneladas por hectárea a junio de 2024.

La discrepancia entre la inercia de crecimiento histórico (dictada por el modelo polinomial) y la contracción real del mercado en 2024 (dictada por el reporte del SIAP) advierte que la disponibilidad de tierra cultivable en Michoacán ha enfrentado un tope físico y operativo. Para "Aguacates Monarca", esta métrica subraya un imperativo estratégico vital: en los próximos años, la rentabilidad no dependerá de la agricultura extensiva (adquirir o sembrar más hectáreas), sino de la agricultura intensiva. La optimización del rendimiento por hectárea es el único vector de crecimiento viable frente a la saturación del suelo agrícola.
