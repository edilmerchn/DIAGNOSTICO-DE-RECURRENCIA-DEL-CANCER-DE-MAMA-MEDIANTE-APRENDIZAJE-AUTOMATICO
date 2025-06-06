# Diagnóstico de Recurrencia del Cáncer de Mama mediante Aprendizaje Automático

Este proyecto aplica algoritmos de aprendizaje automático para predecir la recurrencia del cáncer de mama, utilizando el conjunto de datos del repositorio UCI. Se comparan tres modelos supervisados: Regresión Logística, Árbol de Decisión y SVM con kernel RBF.

---

## Resultados

A continuación se presenta una tabla comparativa con las métricas más relevantes para la clase de recurrencia:

| Modelo              | Exactitud | Precisión (Recurrencia) | Sensibilidad (Recall) | F1-score (Recurrencia) |
|---------------------|-----------|--------------------------|------------------------|-------------------------|
| Regresión Logística | 0.70      | 0.50                     | 0.32                   | 0.39                    |
| Árbol de Decisión   | 0.69      | 0.48                     | 0.40                   | 0.44                    |
| SVM (Kernel RBF)    | 0.73      | 0.60                     | 0.24                   | 0.34                    |

---

## Matrices de Confusión

Las siguientes figuras muestran el desempeño de cada modelo al clasificar correctamente (o no) los casos de recurrencia y no recurrencia:

### Regresión Logística
![Matriz de Confusión - Regresión Logística](ruta/a/la/imagen1.jpg)

- 51 verdaderos negativos
- 8 falsos positivos
- 17 falsos negativos
- 8 verdaderos positivos

### Árbol de Decisión
![Matriz de Confusión - Árbol de Decisión](ruta/a/la/imagen2.jpg)

- 48 verdaderos negativos
- 11 falsos positivos
- 15 falsos negativos
- 10 verdaderos positivos

### SVM con Kernel RBF
![Matriz de Confusión - SVM con Kernel RBF](ruta/a/la/imagen3.jpg)

- 55 verdaderos negativos
- 4 falsos positivos
- 19 falsos negativos
- 6 verdaderos positivos

---

## Estructura del Proyecto
