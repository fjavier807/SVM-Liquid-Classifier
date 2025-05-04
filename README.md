
# 🔍 Clasificación de Líquidos con SVM usando Datos de Sensores

Este proyecto implementa un modelo de clasificación binaria utilizando **Máquinas de Vectores de Soporte (SVM)** para diferenciar entre agua y aceite a partir de datos obtenidos por sensores. Se incluyen pasos de preprocesamiento, reducción de dimensionalidad, entrenamiento, evaluación y visualización del modelo.



## ✅ Resumen

Este proyecto tiene como objetivo desarrollar un sistema de clasificación automática para identificar líquidos (agua o aceite) utilizando datos obtenidos por sensores. A partir de un conjunto de características medidas, se entrenó un modelo de aprendizaje automático basado en Máquinas de Vectores de Soporte (SVM) que permite clasificar con alta precisión el tipo de líquido. El proceso incluye preprocesamiento de datos, reducción de dimensiones con PCA para visualización y validación del rendimiento mediante métricas de clasificación y análisis visual.



## ⚙️ Metodología

1. **Adquisición de Datos**: Se utilizó un archivo CSV con múltiples características medidas por sensores y una columna `target` que indica la clase del líquido (`+1` para agua, `-1` para aceite).

2. **Preprocesamiento**:
   - Se normalizaron las variables con `StandardScaler` para igualar escalas y mejorar el rendimiento del modelo.
   - Se aplicó reducción de dimensionalidad con `PCA` para visualizar los datos en 2D sin perder la estructura esencial.

3. **Entrenamiento**:
   - Se utilizó un modelo SVM (`SVC` de scikit-learn) por su capacidad de generalización en problemas de clasificación binaria con márgenes óptimos.
   - No se usó validación cruzada por simplicidad, pero se pueden agregar técnicas adicionales para robustez.

4. **Evaluación**:
   - Se generaron reportes con métricas como precisión, recall, F1-score y matriz de confusión.
   - Se graficó la frontera de decisión del modelo en el plano PCA para validar visualmente la separación entre clases.

---

## 📌 Conclusiones

- El modelo SVM entrenado logró clasificar correctamente los líquidos con una alta tasa de precisión.
- La separación entre clases es clara cuando se proyectan los datos a través de PCA, lo que valida tanto la calidad de los datos como la elección del modelo.
- La metodología utilizada es eficiente y puede aplicarse a otros sistemas de sensores para clasificación binaria.
- Para futuras mejoras se recomienda:
  - Evaluar con validación cruzada
  - Probar otros modelos como Random Forest o Redes Neuronales
  - Implementar el sistema en tiempo real con entrada de sensores físicos

---

## 📁 Archivos Incluidos

- `SVM_AD_sensores_agua_aceite.ipynb` — Notebook con todo el desarrollo del proyecto.
- `dataset.csv` — Conjunto de datos que contiene mediciones de sensores y la clase objetivo (`+1` = agua, `-1` = aceite).

---

## 🧪 Tecnologías Utilizadas

- Python
- pandas, numpy — procesamiento y análisis de datos
- scikit-learn — escalado, PCA, SVM, métricas de evaluación
- matplotlib, seaborn — visualización de datos y resultados

---

## 🔄 Flujo del Proyecto

1. **Carga del Dataset**
   - Lectura de `dataset.csv` usando separador `;`
   - Exploración inicial de las clases (`+1`, `-1`)

2. **Preprocesamiento**
   - Separación de características (`X`) y etiqueta (`y`)
   - Normalización con `StandardScaler`

3. **Reducción de Dimensionalidad**
   - Aplicación de PCA (Análisis de Componentes Principales) para reducir las dimensiones a 2 y facilitar la visualización

4. **Entrenamiento del Modelo**
   - Se entrena un clasificador `SVC` (Support Vector Classifier)

5. **Evaluación del Modelo**
   - Cálculo de métricas como:
     - Accuracy
     - Precision, Recall, F1-score
     - Matriz de confusión

6. **Visualización**
   - Análisis visual de la distribución de clases y separación por PCA
   - Frontera de decisión del modelo
   - Matriz de confusión en forma de imagen

---

## 📊 Visualizaciones Incluidas

- 📈 **Distribución de clases** (`target`) con `seaborn`
- 🌐 **Gráfica 2D de PCA** mostrando la separación entre agua y aceite
- ✳️ **Frontera de decisión del SVM** sobre los datos reducidos a 2 dimensiones
- 🧩 **Matriz de confusión** visual con `matplotlib`
- 📋 **Reporte de métricas** en consola (`classification_report` de scikit-learn)

---

## 🚀 Cómo Ejecutar el Proyecto

1. Instala las dependencias necesarias:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
