# PhawAI: Predicción de Enfermedades Coronarias

[![Kaggle Competition](https://img.shields.io/badge/Kaggle-Competition-blue)](https://www.kaggle.com/competitions/phawai-prediccion-enfermedades-coronarias)

Este repositorio contiene los archivos, códigos y documentación del proyecto **PhawAI**, enfocado en desarrollar un modelo de Machine Learning para predecir enfermedades coronarias usando el dataset proporcionado por el Behavioral Risk Factor Surveillance System (BRFSS) 2022. 

---

## 📜 Tabla de Contenidos
- [Introducción](#introducción)
- [Objetivos del Proyecto](#objetivos-del-proyecto)
- [Estructura del Repositorio](#estructura-del-repositorio)
- [Requisitos Previos](#requisitos-previos)
- [Instrucciones de Uso](#instrucciones-de-uso)
- [Métricas de Evaluación](#métricas-de-evaluación)
- [Enfoque del Proyecto](#enfoque-del-proyecto)
- [Referencias](#referencias)

---

## 📖 Introducción

Las enfermedades coronarias son una de las principales causas de muerte a nivel mundial. Este proyecto tiene como objetivo aprovechar el dataset **BRFSS 2022**, que incluye información demográfica, hábitos de salud y condiciones previas, para construir modelos predictivos que puedan identificar individuos con riesgo de padecer enfermedades coronarias. 

### Desafíos del Proyecto:
- Dataset desbalanceado con pocos casos positivos.
- Manejo de valores nulos y características no relevantes.
- Uso de métricas como F1-score para evaluación en lugar de precisión estándar.

---

## 🎯 Objetivos del Proyecto

1. **Predicción precisa**: Desarrollar un modelo de Machine Learning para predecir enfermedades coronarias usando variables relevantes.
2. **Balanceo de datos**: Implementar técnicas como sobremuestreo o submuestreo para mitigar el desbalance de clases.
3. **Optimización**: Usar técnicas avanzadas de preprocesamiento, selección de características y ajuste de hiperparámetros para maximizar el F1-score.
4. **Escalabilidad**: Crear un pipeline reproducible y eficiente para su potencial uso en implementaciones reales.

---

## 📂 Estructura del Repositorio

```plaintext
PhawAI/
│
├── data/                    # Archivos de datos
│   ├── train.csv            # Dataset de entrenamiento
│   ├── test_public.csv      # Dataset de prueba pública
│   └── test_private.csv     # Dataset de prueba privada
│
├── notebooks/               # Notebooks de Jupyter
│   ├── EDA.ipynb            # Exploración de datos (EDA)
│   ├── Preprocessing.ipynb  # Limpieza y preprocesamiento
│   ├── Modeling.ipynb       # Entrenamiento y evaluación de modelos
│   └── Submission.ipynb     # Generación de archivo de predicción
│
├── scripts/                 # Scripts de Python
│   ├── preprocess.py        # Funciones de preprocesamiento
│   ├── model.py             # Entrenamiento y evaluación de modelos
│   └── utils.py             # Utilidades generales
│
├── results/                 # Resultados y archivos de salida
│   └── resultados.csv       # Archivo de predicciones para Kaggle
│
├── README.md                # Este archivo
└── requirements.txt         # Dependencias del proyecto
