]# Análisis Causal del Plan 401(k): Una Perspectiva Evolutiva

Este repositorio contiene el código y los resultados para el análisis empírico del impacto de la participación en el plan de ahorro 401(k) sobre la riqueza neta de los hogares.

## 🏛️ Objetivo de Investigación
El proyecto aborda la pregunta de investigación transitando por tres épocas de la inferencia causal:
1. **Enfoque Clásico:** Variables Instrumentales (2SLS) / Estimador de Wald.
2. **Revolución Moderna:** Double Machine Learning (DML) con Random Forest y XGBoost.
3. **Descubrimiento de Heterogeneidad:** Árboles Causales (Causal Forests) para identificar desigualdades estructurales automatizadas (CATE).

## 🚀 Resultados Clave
- **Impacto Promedio:** El modelo clásico subestima el efecto ($7,219), mientras que el método doblemente robusto (DML) identifica un impacto de ~$12,085.
- **Hallazgo Principal (Plot Twist):** Al usar *Causal Forests*, el algoritmo ignoró los cortes clásicos de ingreso y edad, revelando que la variable determinante para maximizar el beneficio del plan es la **tenencia de vivienda propia**.

## 📊 Visualización del Descubrimiento Causal
![Árbol Causal 401k](graficos_png/arbol_causal_401k.png)

## 📁 Estructura del Repositorio
- `analisis_401k.ipynb`: Cuaderno principal con el pipeline de datos completo.
- `graficos_png/`: Visualizaciones de LATE y Árbol Causal.
- `regresiones_txt/`: Salidas estadísticas detalladas de los modelos (formato estándar).
- `datos_csv/`: Tablas de estadísticas descriptivas.

---
*Desarrollado para fines académicos para la hackathon del curso Aplicaciones de Machine Learning Para Economia*
