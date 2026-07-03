# Guion para video de defensa - Unidad 2

**Duración sugerida:** 6 a 8 minutos  
**Tema:** Inferencia estadística paramétrica aplicada al dataset ENEMDU de vivienda y hogar en Loja  
**Archivo base:** `Evaluacion_Sumativa_Unidad2_Inferencia_Loja_FINAL_REAL.ipynb`

## 0:00 - 0:40 | Presentación

Buenas tardes, mi nombre es Joaquín Emilio Moscol Castillo. En este video voy a defender la Evaluación Sumativa de la Unidad 2 de Análisis de Teoría de la Distribución y Probabilidad. El trabajo se realizó con el dataset ENEMDU de vivienda y hogar 2026-02, filtrando únicamente los registros correspondientes a la provincia de Loja.

La variable principal analizada fue `vi141`, que representa el valor mensual de arriendo o gasto de vivienda. Con esta variable se aplicaron los contenidos reales de la plataforma: APE06, APE07, APE08, APE09 y APE10.

## 0:40 - 1:40 | Criterio estadístico inicial

Primero cargué el dataset en Python usando pandas y filtré la provincia de Loja mediante los dos primeros dígitos de la variable `ciudad`, donde el código 11 corresponde a Loja. Después limpié la variable `vi141`, eliminando datos faltantes o códigos de no información.

El dataset final de Loja quedó con **302 hogares**. La media muestral del valor mensual fue de **142.80 dólares**, con una desviación estándar de **94.08 dólares**.

## 1:40 - 2:40 | APE06 y APE07: normalidad y TLC

Como parte del APE06, revisé la forma de la distribución mediante histograma, gráfico Q-Q, asimetría, curtosis y Shapiro-Wilk. Los resultados mostraron que la variable no sigue una normalidad perfecta, porque presenta sesgo positivo y valores extremos.

Sin embargo, aquí se conecta el APE07 sobre el Teorema del Límite Central. Como la muestra tiene más de 30 observaciones, se puede trabajar con inferencia sobre la media, considerando que la distribución de las medias muestrales tiende a estabilizarse.

## 2:40 - 3:35 | APE08: intervalo de confianza

Luego, en el APE08 apliqué estimación de parámetros. Como no conocemos la desviación estándar poblacional, utilicé la distribución T de Student para construir un intervalo de confianza del 95%.

El intervalo obtenido fue aproximadamente de **132.14 a 153.45 dólares**. Esto significa que, con 95% de confianza, el promedio poblacional del valor mensual de arriendo en Loja se encuentra dentro de ese rango.

## 3:35 - 4:45 | APE09: prueba de hipótesis y valor-p

Para el APE09 planteé una prueba de hipótesis unimuestral. La hipótesis nula fue que la media poblacional del valor mensual de arriendo es igual a 200 dólares:

H0: mu = 200

La hipótesis alternativa fue que la media es diferente de 200 dólares:

H1: mu ≠ 200

Apliqué una prueba T de Student para una muestra. El valor-p obtenido fue **2.1064e-22**, menor que 0,05. Por eso, rechazo la hipótesis nula. Esto significa que existe evidencia estadística suficiente para afirmar que el promedio mensual de arriendo en Loja es diferente de 200 dólares.

## 4:45 - 5:45 | Comparación A/B urbano-rural

Como comparación de dos grupos, dividí los datos entre área urbana y área rural. Para esto apliqué una prueba T de Welch, porque no se asume igualdad de varianzas.

El valor-p fue **6.6426e-19**, por lo que se rechaza la hipótesis de igualdad de medias. En otras palabras, el valor mensual de vivienda cambia significativamente entre el área urbana y el área rural.

## 5:45 - 6:50 | APE10: ANOVA y Tukey

Finalmente, para el APE10 apliqué un ANOVA de un factor. El factor fue el número de cuartos de la vivienda, agrupado en 1-2 cuartos, 3-4 cuartos y 5 o más cuartos. La variable dependiente fue nuevamente `vi141`.

El ANOVA obtuvo un valor-p de **6.8731e-14**, menor que 0,05. Por tanto, rechazo la hipótesis nula de igualdad de medias entre todos los grupos. Luego apliqué la prueba Post-Hoc de Tukey, que permite identificar entre qué pares de grupos existen diferencias significativas.

## 6:50 - 7:40 | Cierre e interpretación final

En conclusión, este análisis demuestra que el software estadístico no debe usarse como una caja negra. Primero se debe revisar la distribución de los datos, luego estimar parámetros, después formular hipótesis y finalmente interpretar el valor-p.

Los resultados muestran que el valor mensual de vivienda en Loja difiere significativamente de 200 dólares, cambia entre zonas urbanas y rurales, y también se relaciona con el número de cuartos de la vivienda. Por ello, la inferencia estadística permitió transformar datos regionales reales en evidencia matemática para la toma de decisiones.