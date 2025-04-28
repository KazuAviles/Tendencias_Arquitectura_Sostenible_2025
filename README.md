# Predicción tendencias arquitectónicas:

Este es el desarrollo de un proyecto de practica personal, utilizando datos sintéticos.

Descripción del Proyecto:
Este proyecto consiste en la visualización de un dashboard interactivo en Power BI, basado en datos de Google Trends, que permite identificar y analizar las principales búsquedas relacionadas con arquitectura durante los años 2023, 2024 y proyecciones para 2025. El objetivo es ayudar a profesionales, emprendedores y empresas del sector a comprender mejor las necesidades y preferencias del público, detectando oportunidades de negocio emergentes y comportamientos estacionales.

Proyecto: Predicción tendencias arquitectónicas:

🎯Objetivo del Proyecto: Desarrollar un modelo de Machine Learning que permita predecir el interés futuro en ciertas tendencias arquitectónicas usando datos históricos de búsquedas (como los de Google Trends). Esto permitirá anticipar comportamientos y apoyar decisiones estratégicas en contenido, marketing o desarrollo de servicios arquitectónicos.

🧠 Preguntas de Hipotesis: ¿Qué tipo de servicios están más interesados en contratar un los clientes? Quienes son? Que tendencias estan vigentes? Que servicios contratan? Que tipo de servicios buscan?

##  Descripción de los datos

#### Columnas clave
fecha (formato string) → Variable temporal.

13 columnas temáticas → Variables numéricas con volúmenes de interés (búsquedas) para cada tendencia:

Los datos son obtenidos de Google Trends estan representados por porcentaje de interés. 
- `arquitectura sostenible` - Volúmen de interes;
- `urbanismo`
- `diseño paramétrico` - 
- `ciudades inteligentes` 
- `casas pequeñas` 
- `tiny house`- 
- `diseño de interiores`- 
- `render 3D`- 
- `arquitectura moderna`- 
- `remodelación casa`- 
- `domótica`- 
- `planos de casas`- 
- `arquitectura minimalista`- 

### Condiciones:
#Convertir la columna objetivo "Fecha" en formato string:

Contratado → 1
No Contratado → 0

Característica objetivo: la columna 'Fecha'

Métrica principal: AUC-ROC.

Métrica adicional: exactitud.

Criterios de evaluación:

- AUC-ROC < 0.75 — 0 SP
- 0.75 ≤ AUC-ROC < 0.81 — 4 SP
- 0.81 ≤ AUC-ROC < 0.85 — 4.5 SP
- 0.85 ≤ AUC-ROC < 0.87 — 5 SP
- 0.87 ≤ AUC-ROC < 0.88 — 5.5 SP
- AUC-ROC ≥ 0.88 — 6 SP