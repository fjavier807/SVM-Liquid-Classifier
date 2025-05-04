# 🔬 Clasificación Binaria con Sensores de Agua y Aceite

Este proyecto aplica técnicas de aprendizaje automático para clasificar señales de sensores industriales con el objetivo de diferenciar entre muestras de **agua** y **aceite**. Se entrenaron y compararon tres modelos de clasificación: Árbol de Decisión, Regresión Logística y SVM.

---

## 📁 Índice

- 📂 Descripción y Estructura del Proyecto  
- 🔍 Análisis Exploratorio de Datos (EDA)  
- 📝 Descripción de Variables y Clases  
- 📊 Matriz de Correlación  
- ❌ Eliminación de Variables Irrelevantes  
- ⚙️ Preprocesamiento  
  - Tratamiento de valores nulos  
  - Codificación de variables  
  - Escalado de variables numéricas  
  - División del dataset  
- 🤖 Implementación de Clasificadores  
  - Árbol de Decisión  
  - SVM  
  - Regresión Logística  
- ✅ Comparación de Resultados  
- 🧑‍💻 Autores  

---

## 📊 Metodología

- Se utilizó un dataset de sensores (`dataset.csv`) separado por punto y coma.
- Se aplicó normalización de variables.
- División del conjunto de datos: 80% entrenamiento / 20% prueba.
- Evaluación mediante métricas estándar y visualización de fronteras de decisión.

---

## 🧠 Modelos de Clasificación

### Árbol de Decisión

- **Matriz de Confusión**  
  ![Matriz Árbol](Imagenes/Matriz%20de%20confusion-Arbol%20de%20decision.png)

- **Frontera de Decisión**  
  ![Frontera Árbol](Imagenes/Frontera%20de%20decision-Arbol%20de%20decision.png)

---

### SVM

- **Matriz de Confusión**  
  ![Matriz SVM](Imagenes/Matriz%20de%20confusion-SVM.png)

- **Frontera de Decisión**  
  ![Frontera SVM](Imagenes/Frontera%20de%20decision-SVM.png)

---

### Regresión Logística

- **Matriz de Confusión**  
  ![Matriz Regresión](Imagenes/Matriz%20de%20confusion-Regresion%20Logistica.png)

- **Frontera de Decisión**  
  ![Frontera Regresión](Imagenes/Frontera%20de%20decision-Regresion%20Logistica.png)

- **Curva ROC**  
  ![Curva ROC](Imagenes/Curva%20ROC%20-%20Regresion%20Logistica.png)

---

## 📈 Comparación de Resultados

- **Comparación de F1-Score por Modelo**  
  ![F1-Score](Imagenes/Comparacion%20de%20F1-score%20por%20modelo.png)

- **Métricas por Modelo (DataFrame)**  
  ![Métricas](Imagenes/DATAFRAME%20Resultados%20de%20metricas.png)

- **Resumen de Todas las Métricas**  
  ![Todas las Métricas](Imagenes/DATAFRAMEcon%20todas%20las%20metricas.png)

---

## ✅ Conclusiones

- **SVM** obtuvo el mejor desempeño general, destacando en F1-score y área bajo la curva ROC.
- **Árbol de Decisión** es más interpretable y aún competitivo.
- **Regresión Logística** tuvo rendimiento razonable, pero fue superado por SVM.

---

## 👨‍💻 Autores

- María Fernanda Bolaños Escandón  
- Francisco Javier Estupiñán Andrade  
- Fernando Xavier Montaño Cárdenas  

---

## 📁 Estructura del Repositorio



