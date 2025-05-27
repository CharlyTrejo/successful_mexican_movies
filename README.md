# 🎬 Predicción del Éxito de Películas Mexicanas con Machine Learning
## Proyecto para Netflix-LATAM

Este proyecto utiliza datos de The Movie Database (TMDB) para construir un modelo predictivo que clasifique si una película mexicana será exitosa o no, a partir de información pública como su elenco, género, idioma, año de lanzamiento, presupuesto y más.

Reporte ejecutivo disponible en: 
[https://drive.google.com/drive/folders/1_EfBAIjvlHfV-rE1kBz6X4aCQTE-h0V6?usp=sharing](https://drive.google.com/drive/folders/1_EfBAIjvlHfV-rE1kBz6X4aCQTE-h0V6?usp=sharing)

## 🧠 Modelo de Machine Learning

- Tipo de modelo: Clasificación binaria
- Algoritmo principal: Random Forest Classifier
- Técnicas aplicadas:
  - Recolección dinámica de datos vía TMDB API
  - Ingeniería de características (género, director, actores principales)
  - Tratamiento de desbalanceo con SMOTE
  - Optimización con GridSearchCV
  - One-hot encoding para variables categóricas

## 📊 Principales features predictivas
- `budget`,`vote_count`, `popularity`, `release_month`, `runtime`
- Géneros: `horror`, `thriller`, `drama`, `action`, `romance`
- Idiomas: `original_language_es`, `original_language_en`
- Actores: `Cantinflas`, `Pedro Infante`
- Directores: `Miguel M. Delgado`, `Pedro Pablo Ibarra`

## 🧪 Resultados del modelo

- Accuracy: 92%
- Precision: 0.90 (clase 0) / 0.93 (clase 1)
- Recall: 0.93 (clase 0) / 0.90 (clase 1)

## 📁 Estructura del proyecto
* /data_api_tmdb.py/  *Código para recolección desde TMDB*


* /features_modeling.ipynb/ *Ingeniería de datos, transformación, entrenamiento, tuning y evaluación*


## 📌 Requisitos

- Python 3.8+
- scikit-learn, pandas, requests, imbalanced-learn, matplotlib, seaborn

## 🤖 Futuras mejoras

- Incorporar sinopsis (overview) usando NLP
- Reentrenamiento automático con nuevos lanzamientos
- Clasificación multinivel (bajo, medio, alto éxito)

