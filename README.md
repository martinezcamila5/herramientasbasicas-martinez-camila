# Trabajo Final Integrador – Análisis de factores de riesgo cardiovascular

**Autora:** Camila Martínez  
**Curso:** Herramientas Básicas para el Análisis de Datos – UTN  
**Cohorte:** Septiembre 2026

## Objetivo

Analizar la relación entre factores clínicos, características físicas, hábitos de vida y la presencia de enfermedades cardiovasculares. El proyecto integra Python, Power BI y GitHub para desarrollar un análisis reproducible y comunicar sus resultados mediante visualizaciones e indicadores interactivos.

## Dataset

Se utilizó el *Cardiovascular Disease Dataset*, publicado por Svetlana Ulianova en Kaggle, compuesto originalmente por 70.000 registros. Incluye edad, sexo, peso, altura, presión arterial, colesterol, glucosa, tabaquismo, consumo de alcohol, actividad física y diagnóstico cardiovascular.

**Fuente:** [Cardiovascular Disease Dataset – Kaggle](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset).

## Metodología

El procesamiento se realizó en Google Colab utilizando Python y las bibliotecas Pandas, Matplotlib y Seaborn.

Primero se auditaron los tipos de datos, valores faltantes, duplicados y valores atípicos. Luego se aplicaron criterios de consistencia a las mediciones de presión arterial, altura y peso. Se conservaron 68.544 registros, equivalentes al 97,92 % del conjunto original.

También se transformó la edad de días a años aproximados, se convirtió la altura a metros y se calculó el índice de masa corporal (IMC). Se realizaron estadísticas descriptivas, análisis de valores extremos mediante IQR y percentiles, y visualizaciones exploratorias.

## Resultados principales

La prevalencia cardiovascular general fue del **49,44 %**. El **26,85 %** de los registros presentó presión sistólica elevada (140 mmHg o más), mientras que la prevalencia cardiovascular entre personas inactivas fue del **53,26 %**.

Se observaron mayores porcentajes de diagnósticos positivos en los niveles elevados de colesterol y glucosa, así como un incremento de la prevalencia en los grupos de mayor edad. Estos resultados describen asociaciones y no permiten establecer relaciones causales.

## Dashboard y archivos

Se desarrolló un dashboard interactivo en Power BI con tres indicadores, cuatro gráficos y filtros por sexo y grupo de edad.

- [Notebook de Python](notebooks/TP_final_Martinez_Camila.ipynb)
- [Dataset original](data/raw/cardio_train.csv)
- [Dataset procesado](data/processed/cardio_limpio.csv)
- [Dashboard de Power BI](dashboard/TP%20final%20Martinez%20Camila%20-%20Cardiovascular.pbix)

El repositorio permite consultar los datos, reproducir el análisis y explorar los resultados mediante el archivo de Power BI.
