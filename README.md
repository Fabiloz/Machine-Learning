## Ejercicio Práctico - Bootcamp de Análisis de Datos 
## 🚢 Predicción de Supervivencia de Pasajeros del Titanic: Un Análisis Comparativo con Machine Learning.
Este proyecto es un caso de estudio clásico de análisis exploratorio de datos, preprocesamiento y modelado de machine learning para problemas de clasificación binaria.
## 🎯 Objetivo: Desarrollar y evaluar modelos predictivos para determinar si un pasajero a bordo del Titanic sobrevivió o no, en base a un conjunto de datos históricos.

## 🔗 Notebook del proyecto https://github.com/Fabiloz/Machine-Learning/blob/main/TITANIC_Regresi%C3%B3n%20Log%C3%ADstica%20y%20Random%20Forest.ipynb

## 💡Metodología y Técnicas Aplicadas:
Análisis Exploratorio de Datos (EDA):
Visualización de datos de las variables clave (edad, genero, clase, etc.) y su relación con la supervivencia.
Eliminación y renombre de columnas. 
Conversión de datos categóricos a binarios.
Identificación de patrones y correlaciones relevantes para la predicción.

## ⚙️ Modelado de Machine Learning:
1.	Modelo de Regresión Logistica - LogisticRegression
2.	Random Forest - RandomForestClassifier

## 📊Evaluación del Modelo:
División del dataset en conjuntos de Entrenamiento (70%) y Prueba (30%).
Uso de métricas de clasificación binaria:
Accuracy (Exactitud): Métrica principal para evaluar el rendimiento general.
Precisión, Recall y F1-Score: Para entender el balance entre falsos positivos y falsos negativos, especialmente relevante en problemas donde una clase es más crítica que otra.
Matriz de Confusión: Para visualizar el rendimiento del clasificador.
Curva ROC y AUC para evaluar la capacidad discriminatoria del modelo.

Optimización con Grid Search o Random Search para optimización de hiperparámetros  para Random Forest.

## 📊 Principales Hallazgos

-	El género se relaciona en un 54% con la sobrevivencia, esto quiere decir que probablemente se dio la prioridad de salvar a mujeres y niños.
-	La clase en la cual viajaban los pasajeros también se relaciona con la sobrevivencia en un 32%, viéndose en gran desventaja aquellos pasajeros que viajaron en las clases más económicas.
-	Implementando la regresión logística se obtuvo una exactitud del 76% siendo un modelo útil y sencillo para entender la relación de características como genero y la clase de pasajero.
-	Al utilizar Random Forest, inicialmente se observa que su exactitud para predecir es del 75%, sin embargo, al aplicar una búsqueda de hiperparámetros (GridSearchCV), la exactitud de este modelo mejoró significativamente, alcanzando un 82%. La técnica de combinar múltiples árboles (con max_depth limitado y max_features aleatorias) ayuda a reducir el sobreajuste, resultando en un modelo más robusto. Entonces para este caso, el mejor modelo es el Random Forest.


## 🛠️ Tecnologías y Herramientas
Python: Lenguaje de programación principal.
Librerías: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn.

## 📂 Estructura del repositorio
Machine Learning/
TITANIC_Regresión Logística y Random Forest.ipynb -Notebook principal 
titanic.csv - Dataset inicial 
README.md - Este mismo archivo

## 👤 Autora
Fabiola Isabel Lozano Molina Estudiante / Estudiante de Análisis de Datos 📧 [flozano0515@gmail.com] 🔗 [https://github.com/Fabiloz] 
