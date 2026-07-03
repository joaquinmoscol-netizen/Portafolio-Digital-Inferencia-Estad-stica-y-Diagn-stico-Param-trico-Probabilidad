# Resultados estadísticos principales

- Dataset original: 8765 registros y 57 columnas.
- Provincia filtrada: Loja, código territorial 11.
- Registros analizados de Loja: 302 hogares.
- Variable cuantitativa principal: `vi141`.
- Media muestral: 142.80 dólares.
- Mediana: 120.00 dólares.
- Desviación estándar: 94.08 dólares.
- Intervalo de confianza 95%: [132.14, 153.45].
- Asimetría: 1.8357.
- Curtosis: 6.1235.
- Shapiro-Wilk valor-p: 5.2607e-16.
- Prueba T contra 200 dólares: t = -10.5659, valor-p = 2.1064e-22.
- A/B urbano vs rural: t = 9.6256, valor-p = 6.6426e-19.
- ANOVA por grupos de cuartos: F = 33.5994, valor-p = 6.8731e-14.

## Resumen por área

| area_etiqueta   |   count |   mean |    std |   median |
|:----------------|--------:|-------:|-------:|---------:|
| Rural           |     136 |  94.63 |  52.01 |      100 |
| Urbana          |     166 | 182.26 | 102.25 |      160 |

## Resumen por grupos de cuartos

| grupo_cuartos   |   count |   mean |    std |   median |
|:----------------|--------:|-------:|-------:|---------:|
| 1-2 cuartos     |      71 |  81.48 |  53.27 |       70 |
| 3-4 cuartos     |     193 | 150.73 |  79.83 |      150 |
| 5 o más cuartos |      38 | 217.11 | 142.68 |      190 |

## Tukey

```text
       Multiple Comparison of Means - Tukey HSD, FWER=0.05        
==================================================================
   group1        group2     meandiff p-adj  lower   upper   reject
------------------------------------------------------------------
1-2 cuartos     3-4 cuartos  69.2465   0.0 41.3596  97.1335   True
1-2 cuartos 5 o más cuartos 135.6264   0.0 95.2433 176.0095   True
3-4 cuartos 5 o más cuartos  66.3799   0.0 30.7231 102.0367   True
------------------------------------------------------------------
```