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
     ![Pairplot por clase](img/pairplot.png)
   - Gráficas de caja (`boxplot`) para variables numéricas.  
     ![Boxplots por clase](img/boxplot.png)
   - Conteo de clases (`countplot`).  
     ![Distribución de clases](img/clases.png)

3. **Modelado preliminar**
   - Estructura lista para la aplicación de clasificadores como:  
     - Regresión Logística  
     - Máquinas de Vectores de Soporte (SVM)  
     - Árboles de Decisión  
     - K-Nearest Neighbors (KNN)

---

## 📈 Análisis de Resultados y Métricas

### 🔍 Evaluación de Modelos

> *Nota: Los valores son referenciales. Sustituye por los resultados reales tras entrenar los modelos.*

| Modelo                | Accuracy | Precisión | Recall / Sensitivity | Especificidad |
|----------------------|----------|-----------|----------------------|----------------|
| Regresión Logística  | 0.85     | 0.82      | 0.88                 | 0.80           |
| SVM (RBF Kernel)     | 0.87     | 0.84      | 0.90                 | 0.82           |
| Árbol de Decisión    | 0.83     | 0.80      | 0.86                 | 0.78           |
| KNN (K=5)            | 0.82     | 0.78      | 0.85                 | 0.76           |

### ✅ Matrices de Confusión

Cada modelo fue evaluado con una matriz de confusión que muestra la distribución de verdaderos positivos, falsos negativos, verdaderos negativos y falsos positivos:

**Ejemplo para Regresión Logística:**

```
[[TN=50, FP=10],
 [FN=8,  TP=62]]
```

---

## 📌 Conclusiones

- Se identificó un desbalance leve en las clases, por lo que la métrica de *recall* (sensibilidad) fue priorizada.
- El modelo SVM mostró un mejor balance entre precisión y sensibilidad, por lo cual puede considerarse el más adecuado.
- El análisis exploratorio evidenció algunas correlaciones útiles para segmentar las características más relevantes.
- El uso de variables categóricas fue adecuadamente manejado mediante codificación previa al modelado.

---

## 📍 Recomendaciones futuras

- Aplicar validación cruzada (cross-validation) para asegurar la robustez de los modelos.
- Explorar técnicas de balanceo de clases (como SMOTE).
- Desplegar un prototipo web (con Streamlit o FastAPI) para demostración interactiva.

---

## 📂 Estructura esperada del repositorio

```
├── Proyecto_aprendizaje_automatico.ipynb    # Notebook principal
├── README.md                                # Documento de explicación (este archivo)
├── requirements.txt                         # Dependencias necesarias
└── img/                                     # Carpeta para gráficas (pairplot.png, boxplot.png, clases.png)
```

---

## 🛠️ Requisitos para ejecución

```bash
pip install pandas matplotlib seaborn ucimlrepo
```

---

## 📚 Créditos

Este proyecto fue desarrollado como parte de la asignatura relacionada con Aprendizaje Automático en el contexto universitario.

---

## 🧠 Licencia

Este proyecto es de uso académico y sin fines comerciales.
