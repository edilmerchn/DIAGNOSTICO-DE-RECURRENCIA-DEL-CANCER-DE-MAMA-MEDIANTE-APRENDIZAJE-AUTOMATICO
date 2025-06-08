# Diagnóstico de Recurrencia del Cáncer de Mama mediante Aprendizaje Automático

Este proyecto emplea técnicas de aprendizaje automático para predecir la recurrencia del cáncer de mama utilizando el conjunto de datos **Breast Cancer** proveniente del repositorio UCI. A través de diferentes etapas de limpieza, exploración y modelado, se construyen modelos predictivos para estimar si un evento de recurrencia ha ocurrido o no.

---

## 👨‍💻 Integrantes del equipo

- Juan Fernando Aldana – 2201173  
- Marco Antonio Acosta – 2190289  
- Juan Camilo León – 2190612  
- Santiago Cortés Murcia – 2190365  
- Julian David Velasquez Patiño - 2205142  
- Edilmer Chachinoy Narváez - 22501262

---

## 📊 Dataset

El conjunto de datos fue cargado directamente desde el repositorio UCI Machine Learning. Este contiene variables categóricas como edad, estado de menopausia, tamaño del tumor, nodos invadidos, entre otras. La variable objetivo es `Class`, que indica si hubo o no recurrencia de eventos cancerígenos.

- Fuente: [UCI Breast Cancer Dataset](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer)

---

## ⚙️ Flujo de trabajo

1. **Carga y preprocesamiento de los datos**
   - Extracción desde el repositorio UCI mediante la librería `ucimlrepo`.
   - Unificación de `features` y `target` en un único `DataFrame`.
   - Análisis exploratorio básico (`describe`, `info`, conteos).
   - Visualización de la distribución de clases y boxplots por clase.

2. **Visualización de datos**
   - `Pairplot` por clase.
   - Gráficas de caja (`boxplot`) para las variables numéricas.
   - Conteo de clases (`countplot`).

3. **Modelado preliminar (pendiente de integración)**
   - Se deja estructurado para la inclusión de modelos de clasificación como Regresión Logística, SVM, Árboles de Decisión, etc.

---

## 📂 Estructura esperada del repositorio

```
├── Proyecto_aprendizaje_automatico.ipynb    # Notebook principal
├── README.md                                # Documento de explicación (este archivo)
├── requirements.txt                         # (Opcional) Dependencias necesarias
└── img/                                     # Carpeta sugerida para gráficas
```

---

## 🛠️ Requisitos (sugerido en entorno local o Colab)

```bash
pip install pandas matplotlib seaborn ucimlrepo
```

---

## 📌 Consideraciones

- El análisis aún puede ser extendido con modelos predictivos supervisados.
- La estructura del proyecto permite escalar hacia una aplicación web o API en FastAPI, en futuras etapas.
- El enfoque educativo refuerza el aprendizaje de análisis exploratorio, visualización y uso de datos categóricos.

---

## 📚 Créditos

Este proyecto fue desarrollado como parte de la asignatura relacionada con Aprendizaje Automático en el contexto universitario.

---

## 🧠 Licencia

Este proyecto es de uso académico y sin fines comerciales.
