# ⚽ Inteligencia Artificial Aplicada al Scouting: SOM & Algoritmos Genéticos (Moneyball)

Este repositorio documenta el desarrollo de un motor de *Scouting* Táctico basado en Inteligencia Artificial No Supervisada. El objetivo principal es identificar y agrupar jugadores de fútbol en "Macro-Arquetipos" tácticos, utilizando métricas de rendimiento y algoritmos de aprendizaje automático para descubrir talento oculto bajo la filosofía *Moneyball*.

## 📂 Estructura y Evolución del Proyecto

Este proyecto está dividido en dos grandes fases para demostrar el proceso de iteración, mejora continua y refactorización del código base:

### 📁 `v1_proyecto_academico/` (Fase Inicial)
Contiene la versión original desarrollada como entrega universitaria. 
* Implementación base de Mapas Autoorganizados (SOM).
* Generación inicial de clústeres y análisis táctico exploratorio.
* *Nota: Esta versión se mantiene por fines históricos e institucionales.*

### 📁 `v2_pipeline_avanzado/` (Fase Profesional - Recomendada ⭐)
Esta carpeta contiene la iteración profesional del proyecto, donde el modelo original fue rediseñado bajo estándares de la industria, separando el ecosistema en 5 scripts modulares para facilitar el MLOps y la experimentación:

* **`Script 1 - EDA y Preprocesamiento:`** Limpieza de datos cualitativos, filtrado de minutos jugados y normalización base.
* **`Script 2 - Geometría y PCA:`** Corrección de asimetrías extremas (distribuciones de cola larga) mediante transformación de **Yeo-Johnson** y reducción de dimensionalidad con **PCA** (reteniendo el 87.3% de la varianza táctica en 4 componentes).
* **`Script 3 - Algoritmo Genético:`** Búsqueda de hiperparámetros de la red neuronal mediante un motor evolutivo con mutaciones (micro/macro) y sistema de cataclismos para evitar estancamientos en mínimos locales.
* **`Script 4 - Entrenamiento SOM y Clustering:`** Despliegue de la red neuronal óptima, cálculo de los Errores (Topológico y de Cuantización), y agrupación en Arquetipos usando **K-Means** (validado por Método del Codo y Silueta).
* **`Script 5 - Panel de Scouting (Moneyball):`** Cruce dinámico de la topología matemática con las métricas reales. Conversión de Z-Scores a Percentiles para identificar a los jugadores élite de cada arquetipo en 4 dimensiones del juego (Ataque, Creación, Defensa, Movilidad).

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python
* **Procesamiento y Matemáticas:** Pandas, NumPy, SciPy
* **Machine Learning:** Scikit-Learn, MiniSom
* **Visualización:** Matplotlib, Seaborn
