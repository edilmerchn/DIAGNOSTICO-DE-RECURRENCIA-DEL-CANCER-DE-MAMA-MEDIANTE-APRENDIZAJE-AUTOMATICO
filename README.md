# DIAGNOSTICO TEMPRANO DEL CANCER DE MAMA MEDIANTE APRENDIZAJE AUTOMATICO

Este proyecto utiliza técnicas de aprendizaje automático para predecir de manera temprana la presencia de cáncer de mama, empleando datos públicos de características clínicas de pacientes. El objetivo es desarrollar modelos que asistan a profesionales de la salud en el diagnóstico predictivo, mejorando así la velocidad y precisión del proceso.

## Descripción del Proyecto
## Conjunto de datos
</head>
<body>

<img src="img/1.png" width="400" align="right"/>

El conjunto de datos utilizado en este proyecto es el conjunto de datos de https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic, que consta de características calculadas a partir de una imagen digitalizada de una aspiración con aguja fina (PAAF) de una masa mamaria. La variable objetivo indica si la masa es benigna (0) o maligna (1).

<br><br><br><br><br><br><br><br><br><br>

El cuaderno "DIAGNOSTICO_TEMPRANO_DEL_CANCER_DE_MAMA_MEDIANTE_APRENDIZAJE_AUTOMATICO", contiene el flujo completo de un proyecto de *machine learning* aplicado a datos médicos, incluyendo:

- Importación y exploración del conjunto de datos de cáncer de mama desde el repositorio UCI.
- Limpieza y preprocesamiento de datos.
- Visualización exploratoria de las variables.
- Comparación de múltiples algoritmos de clasificación:
  - Regresión Logística
  - Árboles de Decisión
  - XGBoost
- Evaluación de modelos mediante métricas como precisión, recall, f1-score y matriz de confusión.

Este flujo permite identificar el modelo más eficiente para la tarea de clasificación binaria entre tumores benignos y malignos.

## Tecnologías Utilizadas

- **Python 3**
- **Pandas**: manipulación de datos
- **NumPy**: operaciones matemáticas
- **Matplotlib y Seaborn**: visualización
- **Scikit-learn**: modelado, métricas, preprocesamiento
- **XGBoost**: modelo de boosting avanzado
- **ucimlrepo**: descarga del dataset desde la UCI Machine Learning Repository

## Estructura del Proyecto

```
diagnostico-cancer-mama/
│
├── notebooks/
│   └── diagnostico_cancer_mama.ipynb     # Cuaderno principal del análisis
│
├── requirements.txt                      # Dependencias del proyecto
├── README.md                             # Documentación del proyecto
├── LICENSE                               # Licencia MIT
└── .gitignore                            # Archivos a ignorar por Git
```

## Cómo Empezar

1. **Clona el repositorio**
```bash
   git clone https://github.com/edilmerchn/DIAGNOSTICO_TEMPRANO_DEL_CANCER_DE_MAMA_MEDIANTE_APRENDIZAJE_AUTOMATICO
   cd DIAGNOSTICO_TEMPRANO_DEL_CANCER_DE_MAMA_MEDIANTE_APRENDIZAJE_AUTOMATICO
```

2. **Instala las dependencias**
```bash
pip install -r requirements.txt
```

3. **Ejecuta el notebook**
```bash
jupyter notebook notebooks/DIAGNOSTICO_TEMPRANO_DEL_CANCER_DE_MAMA_MEDIANTE_APRENDIZAJE_AUTOMATICO
.ipynb
```

## Evaluación de Modelos

Se evaluaron diferentes clasificadores y se midió su desempeño con las siguientes métricas:

- **Precisión (Accuracy)**
- **Sensibilidad (Recall)**
- **Puntaje F1**
- **Matriz de Confusión**

Esto permitió seleccionar el modelo con mayor potencial diagnóstico en función del dataset disponible.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT, lo que permite su uso, modificación y distribución con atribución adecuada.
