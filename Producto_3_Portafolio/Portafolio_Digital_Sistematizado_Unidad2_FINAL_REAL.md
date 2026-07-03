# Portafolio Digital Sistematizado - Unidad 2

**Asignatura:** Análisis de Teoría de la Distribución y Probabilidad  
**Unidad:** 02 - Inferencia Estadística y Diagnóstico Paramétrico  
**Estudiante:** Joaquín Emilio Moscol Castillo  
**Carrera:** Computación  
**Paralelo:** 2.º “A”  
**Dataset:** ENEMDU Vivienda y Hogar 2026-02  
**Región:** Provincia de Loja

## 1. Presentación del portafolio

Este portafolio reúne las evidencias desarrolladas durante la Unidad 2 y las integra en una evaluación sumativa basada en datos reales. La organización se ajusta a la plataforma EVA, donde aparecen los APE del **06 al 10**.

El objetivo general fue aplicar herramientas de teoría de la distribución, estimación, prueba de hipótesis y comparación multigrupo sobre el dataset regional de Loja.

## 2. Estructura real de evidencias

| APE | Tema | Archivo/evidencia | Integración en el producto final |
|---|---|---|---|
| APE06 | Distribuciones Continuas Notables | Normalidad del dataset regional | Se diagnosticó la distribución de `vi141` mediante histograma, Q-Q Plot, asimetría, curtosis y Shapiro-Wilk. |
| APE07 | Distribuciones Muestrales y TLC | Cuaderno TLC | Se justificó el uso de inferencia paramétrica sobre la media por tamaño muestral mayor a 30. |
| APE08 | Estimación de parámetros e intervalos | Manuscrito de inferencia e intervalos; notebook de intervalos | Se construyó un intervalo de confianza del 95% para la media de `vi141`. |
| APE09 | Pruebas de hipótesis y valor-p | Cuaderno de hipótesis | Se aplicó una prueba T unimuestral para contrastar la media contra 200 dólares. |
| APE10 | ANOVA y Tukey | Cuaderno ANOVA | Se compararon tres grupos de viviendas según el número de cuartos y se aplicó Tukey. |

## 3. Archivo complementario

Se incluye además el documento **Ajuste_Discreto_GrupoE**, que trabaja el número de dormitorios `vi05a` con una distribución de Poisson. Aunque en la captura de la plataforma no aparece como APE específico de entrega final, sirve como evidencia de práctica adicional sobre distribuciones discretas.

## 4. Producción final realizada

### Producto 1: Documento técnico en Jupyter Notebook

Archivo: `Evaluacion_Sumativa_Unidad2_Inferencia_Loja_FINAL_REAL.ipynb`

Incluye:

- Carga del dataset ENEMDU.
- Filtro de la provincia de Loja.
- Limpieza de `vi141`.
- Estadística descriptiva.
- Diagnóstico de normalidad.
- Intervalo de confianza del 95%.
- Prueba T unimuestral.
- Comparación A/B urbana-rural.
- ANOVA de un factor.
- Prueba Post-Hoc de Tukey.
- Interpretación del valor-p.
- Conclusiones.

### Producto 2: Video de defensa

Archivo de apoyo: `Guion_Video_Defensa_Unidad2_FINAL_REAL.md`

El guion explica el criterio estadístico, la elección de pruebas, el uso de Python, la interpretación del valor-p y la decisión sobre hipótesis.

### Producto 3: Portafolio digital

Este documento organiza las evidencias y explica cómo cada APE se conecta con el producto final.

## 5. Resultados principales del análisis

- Registros originales del dataset: **8765**.
- Registros analizados de Loja: **302**.
- Media muestral de `vi141`: **142.80 dólares**.
- Intervalo de confianza del 95%: **[132.14, 153.45]**.
- Prueba T unimuestral contra 200 dólares: valor-p = **2.1064e-22**.
- Comparación A/B urbano-rural: valor-p = **6.6426e-19**.
- ANOVA por grupos de cuartos: valor-p = **6.8731e-14**.

## 6. Autoevaluación breve

Durante la Unidad 2 se fortaleció la capacidad de transformar datos reales en evidencia estadística. La principal dificultad fue decidir qué prueba aplicar debido a la falta de normalidad perfecta en la variable `vi141`; sin embargo, el tamaño muestral y el Teorema del Límite Central permitieron justificar el uso de pruebas paramétricas sobre la media. También se comprendió que el valor-p no es simplemente un número, sino un criterio de decisión que permite rechazar o no rechazar una hipótesis bajo un nivel de significancia.

## 7. Reflexión final

La unidad permitió comprobar que la estadística no debe aplicarse de forma mecánica. Antes de ejecutar una prueba, es necesario revisar la naturaleza de la variable, el tamaño de la muestra, la distribución de los datos y la estructura de los grupos. En este caso, el análisis de Loja permitió evidenciar que los valores de vivienda presentan variabilidad territorial y diferencias según características físicas del hogar. Por ello, Python no actúa como una caja negra, sino como una herramienta que debe ser interpretada con criterio matemático.

## 8. Referencias

- Devore, J. L. (2016). *Probabilidad y estadística para ingeniería y ciencias* (9.ª ed.). Cengage Learning.
- Walpole, R. E., Myers, R. H., Myers, S. L., & Ye, K. (2012). *Probabilidad y estadística para ingeniería y ciencias* (9.ª ed.). Pearson Educación.
- Conover, W. J. (1999). *Practical nonparametric statistics* (3.ª ed.). John Wiley & Sons.
- Instituto Nacional de Estadística y Censos. Base ENEMDU Vivienda y Hogar 2026-02.