# 🧮 Estimación de Puntuaciones de Examen con Regresión Lineal

## 📘 Informe de Investigación 3
**Materia:** Inteligencia de Negocios
**Tema:** Estimación usando Regresión Lineal

**Autores:**
- Randy Alexander Germosén Ureña *(1013-4707)*
- Fernando Almonte Delgado *(1015-7628)*

---

## 🎯 Objetivo del Proyecto
El propósito de este trabajo es aplicar la **Regresión Lineal** como técnica de estimación para predecir la **puntuación en un examen** de un estudiante en función de dos variables predictoras:
- Horas de estudio
- Horas de sueño

A través de este modelo, se busca analizar cómo estos factores influyen en el desempeño académico y evaluar la precisión del modelo predictivo mediante métricas de desempeño.

---

## 📂 Dataset Utilizado
**Archivo:** `student_exam_regression.csv`

---

## 🧠 Metodología
**El proceso metodológico se desarrolló en las siguientes etapas:**

1. **Obtención de los datos:** se utilizó el archivo ```student_exam_regression.csv```, que contiene los registros de horas de estudio, horas de sueño y la calificación final de los estudiantes.

2. **Preparación de los datos:** se verificó la estructura del conjunto de datos, se identificaron valores faltantes y se realizaron resúmenes estadísticos para explorar la distribución de las variables.

3. **División del conjunto de datos:** el dataset fue dividido en subconjuntos de entrenamiento y prueba, con el fin de ajustar y validar el modelo de regresión.

4. **Construcción del modelo:** se aplicó la función lm() de R para estimar el modelo de regresión lineal múltiple con la fórmula: 
$$\text{Calificación} = -0.87189 + 6.55909(\text{horas de estudio}) + 3.24630(\text{horas de sueño})$$

5. **Evaluación del modelo:** se analizaron los coeficientes estimados, su significancia estadística (valores p), y el coeficiente de determinación ajustado $R^2$ ajustado para valorar el ajuste global del modelo. También se calcularon métricas de error como el RMSE y MAE para evaluar su precisión.

6. **Visualización de resultados:** se elaboraron gráficos de dispersión y de comparación entre valores observados y predichos, con el fin de verificar el comportamiento del modelo y la coherencia de las predicciones.

---

## 📊 Resultados
El modelo de regresión lineal múltiple demuestra que las horas de estudio y de sueño influyen significativamente en el rendimiento académico, explicando cerca del 80 % de la variabilidad en las calificaciones. Cada hora adicional de estudio aumenta en promedio 6.56 puntos la nota, y cada hora extra de sueño, 3.25 puntos. Estos resultados indican que tanto el esfuerzo académico como el descanso adecuado contribuyen de manera positiva al desempeño de los estudiantes.

---

## 🧩 Herramientas Utilizadas
- **R** (en un entorno de Notebook de Jupyter o RStudio)
- **Librerías principales (R):**
  - `readr` y `dplyr` (parte de `tidyverse`) – Manejo y análisis de datos
  - `ggplot2` (parte de `tidyverse`) – Visualización de datos
  - `GGally` – Matriz de gráficos de correlación (EDA)
  - `caTools` – División de datos (train/test split)
