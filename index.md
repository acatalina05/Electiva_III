# Análisis y predicción de series de tiempo: Predicción del consumo energético

La predicción de la demanda eléctrica es un elemento clave para el funcionamiento eficiente de los sistemas energéticos, ya que permite anticipar el consumo y coordinar de manera óptima la generación y distribución de energía. En un contexto donde se explora la implementación de diversas fuentes de energía, contar con estimaciones precisas resulta fundamental para integrar de manera eficiente estas alternativas, reducir la incertidumbre, mejorar la estabilidad del sistema y contribuir a una formación más adecuada de precios. Este trabajo explora el modelado de la demanda energética considerando distintos horizontes temporales y el papel fundamental de factores como la temperatura, con el fin de comprender mejor los patrones de consumo y fortalecer la toma de decisiones en el sector energético.

## Análisis explotatorio de datos

El análisis exploratorio de datos (EDA) se orienta en identificar patrones temporales relevantes, como tendencias, estacionalidad y posibles ciclos en el consumo energético, los cuales son fundamentales para la correcta especificación de modelos de series de tiempo. Asimismo, el EDA facilita la detección de anomalías, valores atípicos o inconsistencias en los datos, que podrían sesgar los resultados si no son tratados adecuadamente.
Adicionalmente, dado que el estudio incorpora una dimensión comparativa entre países, el análisis exploratorio resulta clave para evidenciar posibles diferencias estructurales en los patrones de consumo, particularmente aquellas asociadas a factores climáticos. Esto permite evaluar preliminarmente la existencia de heterogeneidad entre países con climas fríos y cálidos, lo cual constituye un elemento central en la estrategia empírica del trabajo.
[Ir al análisis](prediccion_consumo_energia.ipynb)


## Descripción del conjunto de datos

Los datos utilizados en este estudio provienen de la Red Europea de Gestores de Redes de Transporte de Electricidad (ENTSO-E), e incluyen información sobre la carga de consumo energético para un conjunto de países europeos. La base de datos contiene observaciones con frecuencia horaria, agregadas mensualmente, y la variable de interés se mide en teravatios-hora (TWh). La serie abarca el periodo comprendido entre enero de 2023 y diciembre de 2025.
Para efectos del análisis, los países se clasifican según su condición climática en dos grupos. Por un lado, los países de clima cálido incluyen España, Grecia, Croacia y Portugal. Por otro lado, los países de clima frío comprenden Estonia, Finlandia, Lituania, Letonia, Noruega y Suecia. Esta clasificación permite capturar posibles diferencias estructurales en los patrones de consumo energético asociadas a condiciones climáticas, en línea con la estrategia empírica del estudio.
