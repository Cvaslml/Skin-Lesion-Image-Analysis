# 🎥 Video del Proyecto

**YouTube:** [https://youtu.be/k7liobt4jhM?si=BZsb3U0w1VhqRhSy](https://youtu.be/k7liobt4jhM?si=BZsb3U0w1VhqRhSy)

> *Video del Proyecto: presentación visual del flujo de trabajo y resultados principales.*

# 🩺 DermaMNIST-ML-Project

### Análisis y modelado de imágenes dermatológicas con técnicas de Machine Learning

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![NumPy](https://img.shields.io/badge/NumPy-Arrays-orange?logo=numpy)
![Sklearn](https://img.shields.io/badge/Scikit--Learn-ML-green?logo=scikitlearn)
![PCA](https://img.shields.io/badge/PCA-Dimensionality%20Reduction-orange)
![KMeans](https://img.shields.io/badge/K--Means-Clustering-yellow)
![DBSCAN](https://img.shields.io/badge/DBSCAN-Density%20Clustering-red)
![tSNE](https://img.shields.io/badge/t--SNE-Visualization-purple)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)

---

## 📌 Descripción del proyecto

Este repositorio contiene un proyecto completo de **Machine Learning aplicado a imágenes dermatológicas**, utilizando el dataset **DermaMNIST**.
El objetivo es analizar la estructura de los datos, reducir su dimensionalidad, visualizar patrones internos y aplicar distintos modelos de análisis explorarorio.

El proyecto incluye:

* Preprocesamiento y normalización del dataset
* Reducción de dimensionalidad con **PCA**
* Análisis de agrupamiento con **K-Means** y **DBSCAN**
* Visualización avanzada con **t-SNE**
* Comparación gráfica y técnica entre métodos
* Organización clara y reproducible para facilitar su estudio

Todo el flujo de trabajo está implementado en notebooks y puede ser ejecutado directamente.

---

## 📚 Tabla de contenidos

* [Dataset](#-dataset)
* [Tecnologías utilizadas](#-tecnologías-utilizadas)
* [Pipeline del proyecto](#-pipeline-del-proyecto)
* [Visualizaciones generadas](#-visualizaciones-generadas)

---

## 🗂 Dataset

El dataset utilizado es **DermaMNIST**, parte de la colección *MedMNIST*.
Contiene imágenes clínicas clasificadas en 7 tipos de lesiones dermatológicas, ya preprocesadas a tamaño 28×28×3.

Clases incluidas:

* akiec – queratosis actínica
* bcc – carcinoma basocelular
* bkl – queratosis benigna
* df – dermatofibroma
* nv – nevus
* mel – melanoma
* vasc – lesiones vasculares

Las imágenes permiten explorar patrones visuales entre las diferentes lesiones.

---

## 🧰 Tecnologías utilizadas

* **Python 3**
* **NumPy**
* **Pandas**
* **Matplotlib / Seaborn**
* **Scikit-Learn** (PCA, KMeans, DBSCAN, t-SNE)
* **Joblib**
* **Jupyter Notebook**

---

## 🔄 Pipeline del proyecto

### **1. Carga y preprocesamiento**

* Lectura del dataset `.npz`
* Normalización de píxeles
* Flatten de imágenes para modelos que lo requieren
* Escalado con `StandardScaler`

### **2. Reducción de dimensionalidad**

* Aplicación de **PCA** reteniendo el 95% de la varianza
* Obtención del número óptimo de componentes
* Gráfica de varianza explicada
* Proyección a PCA(2) para visualización

### **3. Análisis de estructura interna**

* Exploración de la forma del dataset en 2D
* Interpretación de densidad y distribución de puntos

### **4. Métodos de agrupamiento**

#### 🔵 K-Means

* Selección de *K* mediante:

  * Inertia (Elbow Method)
  * Distortion curve
  * Silhouette Score
* Entrenamiento con el *K* óptimo
* Visualización de clusters en PCA(2)
* Inspección de ejemplos por cluster

#### 🔴 DBSCAN

* Estimación del `eps` con **k-distance plot**
* Prueba de diferentes configuraciones
* Visualización en PCA(2)
* Extracción de ejemplos por cluster y análisis de ruido

### **5. Visualización avanzada**

* Proyección de un subconjunto del dataset usando **t-SNE**
* Comparaciones visuales entre técnicas
* Mapa de colores por cluster

### **6. Conclusiones generales**

* Interpretación de los patrones observados
* Observaciones sobre la estructura del dataset
* Observaciones sobre el desempeño relativo de los métodos

---

## 🎨 Visualizaciones generadas

El proyecto produce diversas figuras, incluyendo:

* Gráfico de varianza explicada por PCA
* Elbow Method, Distortion y Silhouette Score
* Proyecciones PCA(2) del dataset
* Visualización de K-Means
* Visualización de DBSCAN
* Comparación directa K-Means vs DBSCAN
* Proyección t-SNE coloreada por cluster

---
El objetivo es analizar la estructura de los datos, reducir su dimensionalidad, visualizar patrones internos y aplicar distintos modelos de análisis explorarorio.

El proyecto incluye:
- Preprocesamiento y normalización del dataset  
- Reducción de dimensionalidad con **PCA**  
- Análisis de agrupamiento con **K-Means** y **DBSCAN**  
- Visualización avanzada con **t-SNE**  
- Comparación gráfica y técnica entre métodos  
- Organización clara y reproducible para facilitar su estudio

Todo el flujo de trabajo está implementado en notebooks y puede ser ejecutado directamente.

---

## 📚 Tabla de contenidos
- [Dataset](#-dataset)
- [Tecnologías utilizadas](#-tecnologías-utilizadas)
- [Pipeline del proyecto](#-pipeline-del-proyecto)
- [Visualizaciones generadas](#-visualizaciones-generadas)

---

## 🗂 Dataset
El dataset utilizado es **DermaMNIST**, parte de la colección *MedMNIST*.  
Contiene imágenes clínicas clasificadas en 7 tipos de lesiones dermatológicas, ya preprocesadas a tamaño 28×28×3.

Clases incluidas:
- akiec – queratosis actínica  
- bcc – carcinoma basocelular  
- bkl – queratosis benigna  
- df – dermatofibroma  
- nv – nevus  
- mel – melanoma  
- vasc – lesiones vasculares  

Las imágenes permiten explorar patrones visuales entre las diferentes lesiones.

---

## 🧰 Tecnologías utilizadas
- **Python 3**  
- **NumPy**  
- **Pandas**  
- **Matplotlib / Seaborn**  
- **Scikit-Learn** (PCA, KMeans, DBSCAN, t-SNE)  
- **Joblib**  
- **Jupyter Notebook**

---

## 🔄 Pipeline del proyecto

### **1. Carga y preprocesamiento**
- Lectura del dataset `.npz`  
- Normalización de píxeles  
- Flatten de imágenes para modelos que lo requieren  
- Escalado con `StandardScaler`  

### **2. Reducción de dimensionalidad**
- Aplicación de **PCA** reteniendo el 95% de la varianza  
- Obtención del número óptimo de componentes
- Gráfica de varianza explicada
- Proyección a PCA(2) para visualización

### **3. Análisis de estructura interna**
- Exploración de la forma del dataset en 2D  
- Interpretación de densidad y distribución de puntos  

### **4. Métodos de agrupamiento**
#### 🔵 K-Means
- Selección de *K* mediante:
  - Inertia (Elbow Method)
  - Distortion curve
  - Silhouette Score  
- Entrenamiento con el *K* óptimo  
- Visualización de clusters en PCA(2)  
- Inspección de ejemplos por cluster  

#### 🔴 DBSCAN
- Estimación del `eps` con **k-distance plot**  
- Prueba de diferentes configuraciones  
- Visualización en PCA(2)  
- Extracción de ejemplos por cluster y análisis de ruido  

### **5. Visualización avanzada**
- Proyección de un subconjunto del dataset usando **t-SNE**  
- Comparaciones visuales entre técnicas  
- Mapa de colores por cluster  

### **6. Conclusiones generales**
- Interpretación de los patrones observados  
- Observaciones sobre la estructura del dataset  
- Observaciones sobre el desempeño relativo de los métodos  

---

## 🎨 Visualizaciones generadas
El proyecto produce diversas figuras, incluyendo:

- Gráfico de varianza explicada por PCA  
- Elbow Method, Distortion y Silhouette Score  
- Proyecciones PCA(2) del dataset  
- Visualización de K-Means  
- Visualización de DBSCAN  
- Comparación directa K-Means vs DBSCAN  
- Proyección t-SNE coloreada por cluster  

---

