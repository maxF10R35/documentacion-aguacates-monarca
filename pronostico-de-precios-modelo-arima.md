---
description: >-
  Predicción estadística del valor de la caja de 9 kg para los próximos meses de
  2026 para anticipar compras.
---

# Pronóstico de Precios (Modelo ARIMA)

### Prueba de Estacionariedad (Dickey-Fuller Aumentada)

La extrema volatilidad detectada en la Central de Abasto de Iztapalapa hace imperativo el uso de un modelo econométrico robusto para proyectar los costos de adquisición futuros. Antes de configurar el algoritmo predictivo, la serie temporal de precios frecuentes para la caja de 9 kg (2018-2025) fue sometida a la prueba estadística de Dickey-Fuller Aumentada (ADF) para evaluar la presencia de raíces unitarias.

El test diagnóstico arrojó un _p-value_ de 0.00000880, un valor con una significancia estadística superior al 99.99%. Este resultado rechaza contundentemente la hipótesis nula, confirmando matemáticamente que la serie de costos es fuertemente estacionaria. A nivel de mercado, esto indica que, a pesar de las severas fluctuaciones, el precio mayorista en la CDMX tiende a una rápida reversión a su media histórica; los choques de sobrecosto son escenarios temporales y no permanentes. A nivel econométrico, este diagnóstico dicta la parametrización inicial del modelo, estableciendo un orden de diferenciación nulo ($$d=0$$). Con la serie estabilizada, el entorno de datos es óptimo para proceder con el entrenamiento del modelo predictivo.

### Calibración de Parámetros y Entrenamiento (Modelo ARIMA)

Con la estacionariedad de la serie confirmada, el siguiente paso metodológico consistió en identificar los parámetros óptimos de autorregresión ($$p$$) y de media móvil ($$q$$). Tras un proceso de iteración econométrica y evaluación de los correlogramas (ACF y PACF), se probaron múltiples arquitecturas para la serie temporal.

La evaluación del Criterio de Información de Akaike (AIC) y la prueba de significancia de los coeficientes determinaron que la arquitectura óptima para evitar el sobreajuste es un modelo ARIMA(1, 0, 2). Este modelo demostró una excelencia estadística absoluta: todos sus parámetros ($$p=1$$, $$q=2$$) arrojaron un _p-value_ inferior a 0.01, confirmando un alto poder predictivo. Adicionalmente, la prueba de Ljung-Box sobre los residuos (Prob = 0.72) validó que el algoritmo logró extraer toda la información sistemática del mercado, dejando únicamente ruido blanco aleatorio.

Sin embargo, al proyectar este modelo tradicional hacia el futuro, se detectó que el intervalo de confianza (margen de riesgo) resultaba logísticamente inoperable, con un rango de fluctuación superior a los 500 MXN. Este nivel de incertidumbre evidenció que el modelo estándar carece de "memoria estacional", ignorando los ciclos naturales de escasez y abundancia del aguacate a lo largo del año.

<figure><img src=".gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>



### Ajuste Estacional y Pronóstico Final (Modelo SARIMAX)

Para solucionar esta limitante y generar un presupuesto de compras de emergencia altamente preciso para "Aguacates Monarca", el algoritmo fue escalado a un modelo SARIMA (Seasonal AutoRegressive Integrated Moving Average) con arquitectura $$(1, 0, 2) \times (1, 0, 1)_{12}$$. Al incorporar el ciclo de 12 meses ($$m=12$$), se forzó al algoritmo a recuperar su memoria estacional, proyectando un escenario de costos que replica fielmente los picos de escasez de verano y los valles de sobreproducción de invierno. Esta inyección de inteligencia estacional redujo drásticamente la incertidumbre del modelo, contrayendo la zona de riesgo.

Para validar la agudeza del pronóstico mediante _backtesting_, se superpuso el costo real de adquisición reportado para mayo de 2026 (350 MXN/Caja) sobre la proyección del algoritmo. El cruce de datos reveló una anomalía de mercado altamente capitalizable: el costo actual se ubica en el límite inferior del intervalo de confianza, significativamente por debajo de la apreciación histórica esperada para esta época del año, donde la tendencia natural dicta una escalada agresiva de precios.

<figure><img src=".gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>

El modelo SARIMA demuestra que el mercado mayorista en Iztapalapa se encuentra en una ventana de subvaluación temporal. La recomendación financiera inmediata para "Aguacates Monarca" es ejecutar compras estratégicas de inventario de respaldo durante esta anomalía bajista, bloqueando los costos de adquisición a 350 MXN antes de que la inercia estacional corrija el mercado y empuje los precios hacia el pico inflacionario proyectado inminentemente para el tercer trimestre del año.

