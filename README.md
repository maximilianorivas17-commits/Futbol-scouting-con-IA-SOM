# ⚽ Disecando el ADN Táctico: Scouting Automatizado con IA

Este repositorio contiene la **Versión 1.0 (Baseline)** de un sistema de inteligencia deportiva diseñado para agrupar y descubrir perfiles de futbolistas basándose estrictamente en su rendimiento estadístico. 

## 🎯 Objetivo del Proyecto
El objetivo principal es implementar un enfoque "Moneyball" en el fútbol internacional, identificando talentos infravalorados que replican los patrones de comportamiento táctico de la élite mundial, independientemente de su posición nominal.

## 🛠️ Herramientas y Metodología
* **Extracción de Datos:** API de StatsBomb (Open Data).
* **Preprocesamiento:** Pandas, Numpy, Estandarización P90 y Min-Max.
* **Optimización (Algoritmos Genéticos):** Búsqueda heurística para definir los hiperparámetros óptimos de la red neuronal.
* **Clustering (SOM):** Mapas Autoorganizados para proyectar la huella táctica en un plano topográfico 2D.

## 📂 Estructura del Repositorio
* `/notebooks`: Scripts en Python con la extracción, ingeniería de variables, motor evolutivo (AG) y entrenamiento SOM.
* `/docs`: Informes técnicos y presentación ejecutiva de los hallazgos (Versión 1.0).

## 🚀 Próximos Pasos (Hoja de Ruta Versión 2.0)
Este proyecto está en evolución continua. Las próximas actualizaciones incluirán:
1. **Refinamiento de Variables:** Ajuste de métricas defensivas por el porcentaje de posesión del equipo e inclusión de variables de *Expected Threat (xT)*.
2. **Control de Sesgo de Competición:** Estandarización Intra-Torneo (Z-Score) para comparar equitativamente torneos de distintas confederaciones.
3. **Expansión Muestral:** Integración de datos a nivel de clubes de ligas emergentes para la detección real de "diamantes ocultos".
