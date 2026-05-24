# 📧 Clasificador de Correos Spam con Machine Learning

## 📌 Descripción del proyecto

Este proyecto consiste en la construcción de un modelo básico de Machine Learning para detectar correos electrónicos Spam utilizando Python y Scikit-learn.

El notebook implementa un flujo completo de procesamiento de texto y clasificación utilizando el algoritmo **Naive Bayes Multinomial**, una técnica ampliamente utilizada en tareas de clasificación de texto.

El objetivo principal es aprender cómo transformar texto en variables numéricas y entrenar un modelo capaz de diferenciar entre:

- Correos Spam
- Correos legítimos (Ham)

---

# 🎯 Objetivos del proyecto

- Comprender el flujo básico de un proyecto de NLP (Natural Language Processing)
- Aprender a vectorizar texto utilizando `CountVectorizer`
- Entrenar un modelo de clasificación con `MultinomialNB`
- Evaluar el rendimiento del modelo
- Realizar predicciones sobre nuevos correos electrónicos

---

# 🧰 Tecnologías utilizadas

- Python 3
- Jupyter Notebook
- Pandas
- Scikit-learn

---

# 📚 Librerías principales

```python
import pandas as pd
from sklearn.feature_extraction.text import CountVectorizer
from sklearn.model_selection import train_test_split
from sklearn.naive_bayes import MultinomialNB
from sklearn.metrics import accuracy_score, confusion_matrix, classification_report
```

---

# 🧠 Algoritmo utilizado

## Naive Bayes Multinomial

El modelo utilizado es:

```python
MultinomialNB()
```

Este algoritmo es especialmente eficiente para:

- Clasificación de texto
- Filtrado de spam
- Análisis de sentimientos
- NLP básico

El modelo trabaja calculando probabilidades sobre la frecuencia de palabras presentes en cada correo.

---

# 🗂️ Estructura del notebook

## 1. Creación del dataset

Se crea un conjunto de datos de ejemplo con correos etiquetados como:

- `spam`
- `ham`

Ejemplos:

- “Gana dinero rápido trabajando desde casa” → Spam
- “Hola Juan, te adjunto el reporte de ventas” → Ham

---

## 2. Vectorización del texto

Se utiliza `CountVectorizer` para convertir texto en datos numéricos.

```python
vectorizer = CountVectorizer()
```

Además, se eliminan algunas palabras comunes (`stop words`) para mejorar el análisis.

---

## 3. División de datos

El dataset se divide en:

- 70% entrenamiento
- 30% validación

```python
train_test_split()
```

---

## 4. Entrenamiento del modelo

El modelo se entrena utilizando:

```python
modelo.fit(X_train, y_train)
```

---

## 5. Evaluación

Se evalúa el rendimiento del modelo utilizando:

- Accuracy
- Matriz de confusión
- Classification report

---

## 6. Predicción de nuevos correos

El notebook incluye ejemplos de correos nuevos ingresados manualmente para verificar si son clasificados como Spam o Ham.

Ejemplos:

```text
"Urgente, haz clic aquí para reclamar tu premio exclusivo"
```

```text
"Hola profe, le envío la tarea de inteligencia artificial"
```

---

# 📈 Flujo general del proyecto

```text
Texto → Vectorización → Entrenamiento → Predicción
```

---

# 🧪 Ejercicios propuestos

El notebook incluye actividades adicionales para reforzar el aprendizaje:

- Utilizar `predict_proba()` para obtener probabilidades
- Modificar stop words
- Agregar nuevos correos de entrenamiento
- Analizar cómo cambia el modelo

---

# ▶️ Cómo ejecutar el proyecto

## 1. Clonar el repositorio

```bash
git clone <url-del-repositorio>
```

---

## 2. Instalar dependencias

```bash
pip install pandas scikit-learn jupyter
```

---

## 3. Ejecutar Jupyter Notebook

```bash
jupyter notebook
```

Abrir el archivo:

```bash
spam_email_ml.ipynb
```

---

# 🚀 Posibles mejoras futuras

- Utilizar un dataset real de correos
- Implementar TF-IDF
- Probar otros algoritmos de clasificación
- Crear una interfaz web
- Implementar Deep Learning para NLP
- Añadir limpieza avanzada de texto
- Soporte para múltiples idiomas

---

# 📊 Conceptos aprendidos

Este proyecto permite practicar:

- NLP básico
- Bag of Words
- Clasificación supervisada
- Entrenamiento y validación
- Predicción de texto
- Machine Learning aplicado

---

# 👨‍💻 Autor

Proyecto educativo desarrollado para practicar Machine Learning y procesamiento de lenguaje natural utilizando Python y Scikit-learn.
