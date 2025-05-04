# Clasificación de Lecturas de Sensores de Agua y Aceite

## Tabla de contenido
1. [Introducción](#1-introducción)  
2. [Resumen](#2-resumen)  
3. [Metodologías](#3-metodologías)  
   - [Procesamiento de Datos](#procesamiento-de-datos)  
   - [Modelos de Clasificación](#modelos-de-clasificación)  
   - [Evaluación](#evaluación)  
4. [Resultados y Análisis](#4-resultados-y-análisis)  
   - [Matriz de Confusión - Árbol de Decisión](#matriz-de-confusión---árbol-de-decisión)  
   - [Frontera de Decisión - Árbol de Decisión](#frontera-de-decisión---árbol-de-decisión)  
   - [Matriz de Confusión - SVM](#matriz-de-confusión---svm)  
   - [Frontera de Decisión - SVM](#frontera-de-decisión---svm)  
   - [Matriz de Confusión - Regresión Logística](#matriz-de-confusión---regresión-logística)  
   - [Frontera de Decisión - Regresión Logística](#frontera-de-decisión---regresión-logística)  
   - [Comparación del F1-score por modelo](#comparación-del-f1-score-por-modelo)  
   - [Curva ROC - Regresión Logística](#curva-roc---regresión-logística)  
   - [Métricas de los Modelos](#métricas-de-los-modelos)  
5. [Conclusiones](#5-conclusiones)  

---

## 1. Introducción
El objetivo de este proyecto es desarrollar y evaluar modelos de clasificación para predecir si un sensor de agua y aceite puede detectar con precisión las condiciones del entorno a partir de sus lecturas. Se emplearon tres modelos de clasificación: Árbol de Decisión, SVM (Máquinas de Vectores de Soporte) y Regresión Logística. Las métricas clave utilizadas fueron Precisión, Recall, F1-score y Curvas ROC.

## 2. Resumen
En este informe se presentan los resultados obtenidos de la implementación y evaluación de tres modelos de clasificación. Los datos provienen del archivo `dataset.csv`. El modelo SVM se destacó en rendimiento, aunque los otros también fueron competitivos.

## 3. Metodologías

### Procesamiento de Datos
- Carga de datos desde `dataset.csv`, delimitado por `;`.
- Normalización de características.
- División en 80% entrenamiento, 20% prueba.

### Modelos de Clasificación
- **Árbol de Decisión**: Estructura de árbol binario.
- **SVM**: Maximiza el margen de separación entre clases.
- **Regresión Logística**: Estima probabilidades con función logística.

### Evaluación
- Métricas: Precisión, Recall, F1-score, AUC.
- Gráficas: Matriz de confusión, frontera de decisión, curva ROC.

## 4. Resultados y Análisis

### Matriz de Confusión - Árbol de Decisión  
Análisis: Excelente clasificación, con solo 3 falsos positivos y ningún falso negativo.  
![Ilustración 1](Imagenes/Matriz%20de%20confusion-Arbol%20de%20decision.png)

### Frontera de Decisión - Árbol de Decisión  
Análisis: Separación clara, aunque con algunas zonas de solapamiento.  
![Ilustración 2](Imagenes/Frontera%20de%20decision-Arbol%20de%20decision.png)

### Matriz de Confusión - SVM  
Análisis: Buen rendimiento, con 12 falsos negativos y 15 falsos positivos.  
![Ilustración 3](Imagenes/Matriz%20de%20confusion-SVM.png)

### Frontera de Decisión - SVM  
Análisis: Frontera no lineal que mejora la separación entre clases.  
![Ilustración 4](Imagenes/Frontera%20de%20decision-SVM.png)

### Matriz de Confusión - Regresión Logística  
Análisis: 16 falsos negativos y 11 falsos positivos. Rendimiento aceptable.  
![Ilustración 5](Imagenes/Matriz%20de%20confusion-Regresion%20Logistica.png)

### Frontera de Decisión - Regresión Logística  
Análisis: Frontera lineal. Clasificación menos precisa en zonas solapadas.  
![Ilustración 6](Imagenes/Frontera%20de%20decision-Regresion%20Logistica.png)

### Comparación del F1-score por modelo  
Análisis: Árbol de Decisión tiene el F1-score más alto.  
![Ilustración 7](Imagenes/Comparacion%20de%20F1-score%20por%20modelo.png)

### Curva ROC - Regresión Logística  
Análisis: AUC muy cercano a 1. Excelente capacidad de discriminación.  
![Ilustración 8](Imagenes/Curva%20ROC%20-%20Regresion%20Logistica.png)

### Métricas de los Modelos  
Análisis: Todos los modelos tienen métricas altas. Árbol de Decisión ligeramente superior.  
![Ilustración 9](Imagenes/DATAFRAMEcon%20todas%20las%20metricas.png)

## 5. Conclusiones
Todos los modelos evaluados resultaron adecuados. SVM se destaca por su rendimiento y manejo de clases no lineales. El Árbol de Decisión también ofrece alta precisión y facilidad de interpretación. La Regresión Logística, aunque algo más limitada, sigue siendo una buena opción cuando las clases son linealmente separables.





