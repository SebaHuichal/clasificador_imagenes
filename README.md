# 🧥 Clasificador Inteligente de Imágenes de Ropa — StyleNet

> Proyecto de evaluación del módulo 8: **Fundamentos de Deep Learning**

Modelo de Deep Learning capaz de clasificar automáticamente imágenes de prendas de vestir, desarrollado para el Área de Ciencia de Datos de la tienda virtual **StyleNet**.

---

## 📋 Descripción

El proyecto entrena y evalúa distintas arquitecturas de redes neuronales sobre el dataset **Fashion-MNIST** (70.000 imágenes, 28×28 píxeles, 10 categorías de ropa), pasando de una red densa básica hasta una CNN avanzada con normalización por lotes.

---

## 🗂️ Estructura del proyecto

```
proyecto8/
├── proyecto8_leccion1.ipynb   # La Red Neuronal Artificial
├── proyecto8_leccion2.ipynb   # Deep Learning y elección de arquitectura
├── proyecto8_leccion3.ipynb   # Implementación en Python
└── proyecto8_leccion4.ipynb   # Redes Neuronales Convolucionales
```

---

## 🔬 Contenido por lección

### Lección 1 — La Red Neuronal Artificial
- Definición de una arquitectura densa (MLP) con capas `Flatten` → `Dense(128, relu)` → `Dense(64, relu)` → `Dense(10, softmax)`
- Implementación de una red para clasificación binaria con función de pérdida `binary_crossentropy`
- Inspección de capas, pesos, sesgos, funciones de activación y optimizador

### Lección 2 — Deep Learning
- Arquitectura CNN clásica: bloques `Conv2D` + `MaxPooling2D` + capas densas finales
- Comparativa MLP vs CNN: la CNN requiere hasta 7.5× menos parámetros para imágenes equivalentes
- Justificación del framework elegido: **Keras / TensorFlow** por su rapidez de prototipado y ecosistema de producción

### Lección 3 — Implementación en Python
- Entrenamiento y validación del modelo CNN sobre Fashion-MNIST con normalización de píxeles (0–255 → 0–1)
- Comparación de hiperparámetros: optimizador `Adam` vs `SGD`, distintos `batch_size`
- Aplicación de **Dropout** y **Early Stopping** para prevenir sobreajuste

### Lección 4 — Redes Neuronales Convolucionales
- Rediseño de la CNN con 3 bloques convolucionales, **Batch Normalization** y `padding='same'`
- Evaluación avanzada con métricas de Precision, Recall y F1-Score por categoría
- Predicción sobre imagen externa preprocesada al formato Fashion-MNIST

---

## ⚙️ Tecnologías

| Herramienta | Uso |
|---|---|
| Python 3.11 | Lenguaje base |
| TensorFlow 2.12 / Keras | Construcción y entrenamiento de modelos |
| NumPy | Manipulación de arrays |
| scikit-learn | Métricas de evaluación (F1, Precision, Recall) |
| Matplotlib | Visualización de curvas de entrenamiento |

---


## 📝 Autor

Proyecto desarrollado como evaluación del módulo 8 — Fundamentos de Deep Learning.
por Sebastian Huichal
