# Predicción del número de productos comprados

## Descripción del Problema

Imagina que eres parte del equipo de ciencia de datos de una empresa de comercio electrónico. Tu tarea es predecir cuántos productos un cliente comprará basado en sus características (edad, ingresos, productos, tiempo de navegación, etc.). Para esto, utilizarás tres tipos de modelos de regresión:

* Regresión Lineal
* Árboles de Decisión
* Modelos de Ensamble (Random Forest, Gradient Boosting)

**Nota Importante:** Aunque el número de productos comprados puede ser discreto, el objetivo del reto se enfoca en utilizar modelos de regresión para realizar la predicción.

El objetivo del reto es predecir el número de productos comprados utilizando las variables predictoras del dataset, ajustando los hiperparámetros de cada modelo y comparando los resultados. Para ello sigue los pasos que se encuentran a continuación:

## Pasos a Seguir

### 1. Carga de Datos y Preprocesamiento

**Descripción:** Carga el archivo de datos y explora las variables. Asegúrate de preprocesar las variables correctamente, incluyendo:

* Tratamiento de valores nulos.
* Codificación de variables categóricas (si las hay).
* Estandarización o normalización de las variables numéricas.

### 2. Entrenamiento de Modelos de Regresión

**Descripción:** Entrena tres modelos de regresión para predecir el número de productos comprados:

* **Regresión Lineal:**
    * Utiliza `LinearRegression()` de Scikit-learn.
* **Árbol de Decisión:**
    * Utiliza `DecisionTreeRegressor()` de Scikit-learn.
    * **Hiperparámetros a sintonizar:**
        * `max_depth`: profundidad máxima del árbol.
        * `min_samples_split`: número mínimo de muestras para dividir un nodo.
        * `min_samples_leaf`: número mínimo de muestras en un nodo hoja.
* **Modelos de Ensamble (Random Forest o Gradient Boosting):**
    * Utiliza `RandomForestRegressor` o `GradientBoostingRegressor` de Scikit-learn.
    * **Hiperparámetros a sintonizar:**
        * `n_estimators`: número de árboles (para Random Forest y Gradient Boosting).
        * `max_depth`: profundidad máxima de los árboles.
        * `learning_rate`: tasa de aprendizaje (solo para Gradient Boosting).
        * `min_samples_split`, `min_samples_leaf`: para mejorar el sobreajuste.
    * **Función:** `RandomForestRegressor()` o `GradientBoostingRegressor()`

### 3. Evaluación y Comparación de Modelos

**Descripción:** Evalúa el rendimiento de los tres modelos utilizando las métricas:

* Error Cuadrático Medio (MSE).
* R² (R-cuadrado) para evaluar qué tan bien los modelos se ajustan a los datos de prueba.

**Tareas:**

* Calcular MSE y R² para cada modelo en el conjunto de prueba.
* Comparar los modelos y discutir los resultados obtenidos. ¿Cuál tiene el mejor rendimiento? ¿Por qué?

### 4. Sintonización de Hiperparámetros

**Descripción:** Realiza la sintonización de hiperparámetros para cada modelo utilizando `GridSearchCV` o `RandomizedSearchCV`.

### 5. Visualización de Resultados

**Descripción:** Compara las predicciones de los modelos con los valores reales.
