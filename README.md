
# Clasificación Binaria con Sensores de Agua y Aceite

## 📄 Resumen del Proyecto

Este proyecto tiene como objetivo aplicar y comparar modelos de clasificación para detectar condiciones ambientales a partir de sensores de agua y aceite. Se evaluaron tres enfoques:

- Árbol de Decisión
- Máquinas de Vectores de Soporte (SVM)
- Regresión Logística

Las métricas empleadas fueron Precisión, Recall, F1-score y Curva ROC.

---

## 👨‍🏫 Información General

- **Materia:** Aprendizaje Automático  
- **Profesora:** Gladys María Villegas Rugel  
- **Fecha de entrega:** 03/05/2025  
- **Integrantes:**
  - María Fernanda Bolaños Escandón
  - Francisco Javier Estupiñán Andrade
  - Fernando Xavier Montaño Cárdenas

---

## 📊 Metodología

### 🔹 Procesamiento de Datos

- Carga del archivo `dataset.csv` (separador: punto y coma).
- Normalización de las variables.
- División 80/20 para entrenamiento y prueba.

### 🔹 Modelos Utilizados

- **Árbol de Decisión:** estructura jerárquica para clasificación.
- **SVM:** busca la mejor frontera de separación no lineal.
- **Regresión Logística:** frontera de decisión lineal basada en probabilidad.

### 🔹 Evaluación

- **Métricas:** Precisión, Recall, F1-score, AUC.
- **Visualizaciones:** Matriz de Confusión, Frontera de Decisión, Curva ROC.

---

## 📈 Resultados

### Árbol de Decisión

- **Matriz de Confusión**  
  ![Matriz Árbol](proyecto_clasificacion_binaria/matriz_arbol.png)

- **Frontera de Decisión**  
  ![Frontera Árbol](proyecto_clasificacion_binaria/frontera_arbol.png)

---

### SVM

- **Matriz de Confusión**  
  ![Matriz SVM](proyecto_clasificacion_binaria/matriz_svm.png)

- **Frontera de Decisión**  
  ![Frontera SVM](proyecto_clasificacion_binaria/frontera_svm.png)

---

### Regresión Logística

- **Matriz de Confusión**  
  ![Matriz Regresión](proyecto_clasificacion_binaria/matriz_regresion.png)

- **Frontera de Decisión**  
  ![Frontera Regresión](proyecto_clasificacion_binaria/frontera_regresion.png)

---

### Comparación de Modelos

- **F1-Score por Modelo**  
  ![F1-score](proyecto_clasificacion_binaria/f1score.png)

- **Curva ROC - Regresión Logística**  
  ![ROC](proyecto_clasificacion_binaria/roc_regresion.png)

- **Métricas Generales**  
  ![Métricas](proyecto_clasificacion_binaria/metricas_modelos.png)

---

## ✅ Conclusiones

- **SVM** mostró el mejor rendimiento general, especialmente con datos no linealmente separables.
- **Árbol de Decisión** ofreció alto F1-score y es más interpretable.
- **Regresión Logística** fue adecuada, pero menos eficaz con solapamientos.

> En resumen, se recomienda el modelo **SVM** como el más robusto para este caso de clasificación binaria.

---

## 📂 Estructura del Repositorio



