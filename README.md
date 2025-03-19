# **Team Challenge: Construcción de Pipelines con Scikit-learn**

## **Descripción**
Este proyecto forma parte del *Team Challenge* dedicado a la construcción de *Pipelines* en Scikit-learn. El objetivo es aplicar técnicas de preprocesamiento, modelado y evaluación de datos en un flujo automatizado y reproducible.

El dataset utilizado es **Airline Passenger Satisfaction**, permitiendo desarrollar modelos de clasificación para predecir la satisfacción de los pasajeros en función de diversas características del vuelo.

---

## **Equipo**
- Mario G.
- Mar P.
- Deiene A.
- Antonio E.
- Angela R.
- Marta T.

---

## **Estructura del Repositorio**

```
├── README.md                   # Descripción del proyecto
├── src
│   ├── data
│   │   ├── train.csv           # Datos de entrenamiento
│   │   ├── test.csv            # Datos de prueba
│   ├── models                  # Modelos entrenados
│   ├── result_notebooks
│   │   ├── Team_Ithaca_Pipelines_I.ipynb  # Implementación del Pipeline
│   │   ├── Team_Ithaca_Pipelines_II.ipynb # Evaluación del modelo
│   ├── notebooks               # Notebooks de pruebas
│   ├── utils                   # Funciones auxiliares
```

---

## **Objetivo**
El propósito principal del proyecto es diseñar *Pipelines* en Scikit-learn que permitan realizar un flujo completo de preprocesamiento y modelado. 

### **Pipelines Implementados**

- **Pipeline 1: Limpieza de Nulos y Duplicados**
  - Se eliminan columnas con más del 15% de valores nulos.
  - Se eliminan filas con valores nulos restantes y duplicadas.
  - **Resultado:** Dataset limpio sin valores nulos ni duplicados.

- **Pipeline 2: Identificación de Tipos de Columnas**
  - Identificación de columnas numéricas, binarias y categóricas.
  - Definición de columnas para *One-Hot Encoding* y escalado.
  - **Resultado:** Estructura clara de las transformaciones necesarias.

- **Pipeline 3: Aplicar Logaritmo a Variables Numéricas**
  - Transformación logarítmica a variables con alta variabilidad.
  - Uso de `np.log1p()` para evitar problemas con valores cero.
  - **Resultado:** Distribución más normalizada de variables numéricas.

- **Pipeline 4: Codificación y Escalado**
  - Conversión de variables binarias en valores numéricos (0 y 1).
  - Codificación de variables categóricas con *One-Hot Encoding* y reducción de dimensiones con *SVD*.
  - Escalado de variables numéricas con *StandardScaler()*.
  - **Resultado:** Datos listos para el modelado.

- **Pipeline 5: Entrenamiento y Selección del Mejor Modelo**
  - Prueba de varios modelos (*Random Forest, Gradient Boosting, Regresión Logística, LightGBM*).
  - Evaluación con *Balanced Accuracy*.
  - Selección del mejor modelo para optimización con *GridSearchCV*.
  - Entrenamiento de un *Pipeline* completo con preprocesamiento y el mejor modelo.
  - **Resultado:** Modelo optimizado y listo para predicciones.

---

## **Evaluación**
El rendimiento del modelo se evaluará utilizando **Balanced Accuracy** debido al posible desbalanceo de clases en el dataset.

---

