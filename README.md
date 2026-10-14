# Predicción de riesgo crediticio con Machine Learning

## Descripción
Proyecto de aprendizaje supervisado que busca clasificar solicitudes de crédito según su nivel de riesgo, utilizando técnicas de análisis de datos y aprendizaje automático.

## Objetivo
Construir y comparar modelos de clasificación para identificar créditos de mayor riesgo y evaluar su desempeño.

## Datos
Se trabajó con un conjunto de datos de riesgo crediticio de 1.000 observaciones y 20 variables predictoras originales, incluyendo características financieras y personales.

La variable objetivo se codificó así:
- **0:** crédito de bajo riesgo.
- **1:** crédito de alto riesgo.

## Metodología
- Exploración y preparación de los datos.
- Codificación de variables categóricas.
- Estandarización de variables numéricas.
- Entrenamiento y comparación de modelos.
- Evaluación mediante validación cruzada y métricas de clasificación.
- Análisis de coeficientes, probabilidades y calibración.

## Modelos evaluados
- Regresión logística.
- Árbol de decisión.
- Random Forest.

## Resultados
La regresión logística obtuvo el mejor F1-score para la clase de alto riesgo entre los tres modelos evaluados.

| Modelo | Accuracy | AUC | F1-score |
|---|---:|---:|---:|
| Regresión logística | 0.780 | 0.804 | 0.593 |
| Random Forest | 0.765 | 0.802 | 0.472 |
| Árbol de decisión | 0.640 | 0.590 | 0.438 |

La validación cruzada de la regresión logística obtuvo un AUC promedio de 0.785, con desviación estándar de 0.019.

## Tecnologías
Python, pandas, NumPy, Matplotlib y scikit-learn.

## Conclusión
La regresión logística presentó el mejor desempeño general en esta comparación. Sin embargo, la identificación de créditos de alto riesgo todavía puede mejorarse. Los resultados corresponden a un ejercicio educativo y no constituyen una herramienta validada para tomar decisiones crediticias reales.
