# Clasificación con Red Neuronal Perceptrón Multicapa (MLP)

## Descripción del Proyecto
Este proyecto aborda el diseño, entrenamiento y optimización de un modelo de red neuronal tipo **Perceptrón Multicapa (MLP)** para la clasificación de imágenes del dataset Fashion-MNIST. Se realizaron pruebas de hiperparámetros (tamaño de batch, tasa de aprendizaje, funciones de activación, pérdidas y regularización con Dropout) para encontrar la arquitectura óptima y evaluar su rendimiento global.

---

## Integrantes
* Javier Loaiza
* Fabian Romero

---

## Dataset
* **Nombre:** Fashion-MNIST
* **Descripción:** Conjunto de datos compuesto por 70.000 imágenes en escala de grises de 28x28 píxeles repartidas en 10 categorías de prendas de vestir (60.000 para entrenamiento/validación y 10.000 para evaluación final de test).

---

## Trabajo Realizado
1. **Análisis Exploratorio y Preprocesamiento:** Carga de datos, normalización de píxeles al rango [0, 1] y división estratificada (80% entrenamiento, 20% validación).
2. **Modelo Base:** Implementación e hiperparámetros iniciales.
3. **Experimentación:** 
   * Evaluación de *Batch Size* (32 vs 64).
   * Evaluación de *Learning Rate* (0.001 vs 0.0001).
   * Comparación de funciones de activación (**ReLU** vs **Tanh**).
   * Comparación de funciones de pérdida (*Sparse Categorical Crossentropy* vs *Categorical Crossentropy*).
4. **Regularización y Optimización:** Incorporación de **Dropout (0.3)** y **Early Stopping** para mitigar el sobreajuste.
5. **Evaluación Final:** Medición de Accuracy, Precision, Recall, F1-Score y análisis mediante Matriz de Confusión.

---

## Instrucciones para Abrir y Visualizar en Google Colab

> ⚠️ **IMPORTANTE:** El cuaderno ya cuenta con todos los experimentos entrenados y los resultados/gráficos guardados. **NO ejecutes nuevamente las celdas de entrenamiento (`model.fit`)**.

1. Navega hasta el archivo `Deep_Learning_Ev1.ipynb` en la raíz del repositorio.
2. Haz clic en el botón **Open in Colab** ubicado en la parte superior del cuaderno.
3. Conéctate a un entorno de ejecución en Colab si deseas revisar los bloques interactivos.
4. Recorre las secciones, tablas resumen y gráficos precalculados para visualizar las métricas obtenidas.
