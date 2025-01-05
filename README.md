# PhawAI: Predicción de Enfermedades Coronarias

[![Kaggle Competition](https://img.shields.io/badge/Kaggle-Competition-blue)](https://www.kaggle.com/competitions/prediccion-de-sufrir-enfermedades-coronarias)

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
- [Visualización de Resultados](#visualización-de-resultados)
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
│   └── phawai-challenge-rody-uzuriaga.ipynb
│       ├── 1. Preparación del Notebook
│       ├── 2. Análisis Exploratorio de Datos (EDA)
│       ├── 3. Preprocesamiento
│       ├── 4. Balanceo de Clases
│       ├── 5. Entrenamiento del Modelo
│       ├── 6. Ensamblaje de Modelos
│       ├── 7. Generación de Predicciones
│       └── 8. Visualización de Resultados
│
├── results/                 # Resultados y archivos de salida
│   └── resultados.csv       # Archivo de predicciones para Kaggle
│
├── README.md                # Este archivo
└── requirements.txt         # Dependencias del proyecto
```

---

## 💻 Requisitos Previos

Antes de comenzar, asegúrate de tener instalados los siguientes programas:
- **Python** (versión 3.8 o superior)
- **Jupyter Notebook**
- Bibliotecas listadas en `requirements.txt`

Instala las dependencias usando:
```bash
pip install -r requirements.txt
```

---

## 🛠 Instrucciones de Uso

1. Clona el repositorio:
   ```bash
   git clone https://github.com/rodyuzuriaga/phawai-challenge.git
   cd phawai-challenge
   ```

2. Abre el notebook principal:
   ```bash
   jupyter notebook notebooks/phawai-challenge-rody-uzuriaga.ipynb
   ```

3. Sigue los pasos del notebook, que incluyen:
   - **Exploración de datos**
   - **Preprocesamiento**
   - **Entrenamiento de modelos**
   - **Generación de predicciones**

4. Genera el archivo `resultados.csv` en la carpeta `results/`.

5. Sube el archivo generado a Kaggle para la evaluación final.

---

## 📊 Métricas de Evaluación

El desempeño del modelo se evalúa usando el **F1-score**, ideal para datasets desbalanceados como este. También se utilizan las siguientes métricas:
- **ROC-AUC:** Mide la capacidad del modelo para diferenciar entre clases.
- **Matriz de confusión:** Proporciona una vista detallada de verdaderos positivos, negativos y errores.

---

## 📈 Visualización de Resultados

1. **Matriz de Confusión**:
   - Representa la clasificación correcta y errónea de las predicciones.
     
     ![image](https://github.com/user-attachments/assets/28b05be6-dd71-41e1-a8f8-4f4bde88548d)

   
2. **Curva Precision-Recall**:
   - Evalúa la relación entre precisión y recall en diferentes umbrales.
  
     ![image](https://github.com/user-attachments/assets/437d7f44-f625-486d-9dce-7bf4ca7b7fe5)


3. **Curva ROC y AUC**:
   - Muestra la capacidad del modelo para diferenciar entre clases.
  
     ![image](https://github.com/user-attachments/assets/65a8ba5f-42a6-4379-b9a2-4ff78370ae8a)


4. **Heatmap del F1 Score por Clase**:
   - Indica un buen equilibrio entre precisión y recall, con un alto F1-score para ambas clases.
  
     ![image](https://github.com/user-attachments/assets/746897ec-2833-473c-918c-0b9d510db0eb)


4. **Importancia de Características**:
   - Identifica las variables más relevantes para la predicción.
  
     ![image](https://github.com/user-attachments/assets/7087b289-0488-45a7-9f92-21b9c4cf2393)
     

---

## 📚 Referencias

1. [Dataset BRFSS 2022](https://www.cdc.gov/brfss/annual_data/annual_2022.html)
2. [Kaggle Competition](https://www.kaggle.com/competitions/prediccion-de-sufrir-enfermedades-coronarias)
3. Breiman, L. (2001). Random Forests. *Machine Learning, 45(1), 5-32*.
4. Chen, T., & Guestrin, C. (2016). XGBoost: A Scalable Tree Boosting System. *Proceedings of the 22nd ACM SIGKDD*.

---

### **requirements.txt**
```
pandas
numpy
matplotlib
seaborn
scikit-learn
imbalanced-learn
xgboost
lightgbm
```
---

### Tabla de Contenidos del Notebook
```
1. Preparación del Notebook  
2. Análisis Exploratorio de Datos (EDA)  
3. Preprocesamiento  
4. Balanceo de Clases  
5. Entrenamiento del Modelo  
6. Ensamblaje de Modelos  
7. Generación de Predicciones  
8. Visualización de Resultados
```
