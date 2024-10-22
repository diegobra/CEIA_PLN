
<div align="center">
  <img src="https://www.fi.uba.ar/images/logo-fiuba.png" alt="Logo FIUBA" width="200" style="margin-bottom: 20px;">
  
  # Procesamiento del Lenguaje Natural - Desafíos Resueltos
  
  **Facultad de Ingeniería, Universidad de Buenos Aires (FIUBA)**  
  **Laboratorio de Sistemas Embebidos (LSE)**
  
  ![Python](https://img.shields.io/badge/Python-3.10.12-blue) ![TensorFlow](https://img.shields.io/badge/TensorFlow-2.17.0-orange) ![PyTorch](https://img.shields.io/badge/PyTorch-2.4.1-red)
</div>

Este repositorio contiene la resolución de diferentes desafíos del curso **Procesamiento del Lenguaje Natural** del Laboratorio de Sistemas Embebidos (LSE) de la **Facultad de Ingeniería de la Universidad de Buenos Aires (FIUBA)**. Cada desafío aborda un problema específico de PLN, con el uso de distintas técnicas y modelos.

### Profesor Responsable: Rodrigo Cárdenas

## Tabla de Contenidos

- [Desafío 1: Vectorización de Texto y Clasificación con Naïve Bayes](#desafío-1-vectorización-de-texto-y-clasificación-con-naïve-bayes)
- [Desafío 2: Custom Embeddings con Gensim](#desafío-2-custom-embeddings-con-gensim)
- [Desafío 3: Modelos de Lenguaje con Tokenización](#desafío-3-modelos-de-lenguaje-con-tokenización)
- [Desafío 4: Construcción de un Bot QA](#desafío-4-construcción-de-un-bot-qa)
- [Desafío 5: Análisis de Sentimiento con BERT](#desafío-5-análisis-de-sentimiento-con-bert)

---

## Desafío 1: Vectorización de Texto y Clasificación con Naïve Bayes

En este desafío se trabajó con el dataset **20 newsgroups** para:
1. **Vectorizar documentos**: Se midió la similaridad entre documentos para analizar coherencia en el contenido.
2. **Entrenar modelos de clasificación**: Se implementaron modelos de Naïve Bayes para maximizar el desempeño en el conjunto de test, probando distintas configuraciones de vectorización y variantes como Multinomial y ComplementNB.
3. **Estudiar la similaridad entre palabras**: Utilizando una matriz término-documento, se analizaron términos manualmente seleccionados para estudiar sus similitudes.

**Archivo**: [Desafío 1](Desafio1/Desafio_1.ipynb)

---

## Desafío 2: Custom Embeddings con Gensim

Se utilizó Gensim para crear embeddings personalizados a partir de un corpus distinto al presentado en clase. Los objetivos fueron:
- Generar embeddings y evaluar similitudes entre palabras.
- **Visualizar** los resultados mediante gráficos para entender la relación entre términos en el espacio de embeddings.
- **Obtener conclusiones** sobre las similitudes y diferencias encontradas.

**Archivo**: [Desafío 2](Desafio2/Desafio_2.ipynb)

---

## Desafío 3: Modelos de Lenguaje con Tokenización

En este desafío se desarrollaron modelos de lenguaje utilizando técnicas de tokenización a nivel de palabra y letra. Las tareas incluyeron:
- **Preprocesamiento** del corpus y creación de conjuntos de entrenamiento y validación.
- **Implementación de modelos** con arquitecturas recurrentes (RNN, LSTM, GRU).
- **Generación de secuencias** utilizando estrategias de búsqueda greedy y beam search, explorando los efectos de la temperatura.

**Archivo (tokenización por palabras)**: [Desafío 3 (palabras)](Desafio3/Desafio_3_word.ipynb)\
**Archivo (tokenización por letras)**: [Desafío 3 (letras)](Desafio3/Desafio_3_char.ipynb)

---

## Desafío 4: Construcción de un Bot QA

El objetivo fue construir un bot de preguntas y respuestas utilizando datos del **ConvAI2**. Los pasos fueron:
1. **Preprocesamiento**: Generar secuencias para entrenar un modelo encoder-decoder.
2. **Preparación de embeddings**: Utilización de Glove o FastText para vectorizar entradas.
3. **Entrenamiento del modelo**: Implementación del esquema encoder-decoder.
4. **Inferencia**: Separar la inferencia de encoder y decoder para evaluar el desempeño del bot.

**Archivo**: [Desafío 4](Desafio4/Desafio_4.ipynb)

---

## Desafío 5: Análisis de Sentimiento con BERT

El último desafío consiste en implementar un modelo de **análisis de sentimiento** utilizando **BERT**. Se trabajó con un dataset de reseñas de aplicaciones para comprender el contexto y el significado de las palabras, aprovechando las capacidades avanzadas de BERT para análisis semántico.

**Archivo 1**: [Desafío 5 (modelo original)](Desafio5/Desafio_5_original.ipynb)\
**Archivo 2**: [Desafío 5 (modelo con 5 categorías)](Desafio5/Desafio_5_cinco_categorias.ipynb)\
**Archivo 3**: [Desafío 5 (modelo con 5 categorías y otros experimentos)](Desafio5/Desafio_5_cinco_categorias_plus.ipynb)

---

## Requisitos

- Python 3.8+
- Librerías: `scikit-learn`, `gensim`, `tensorflow`, `torch`, `transformers`, `matplotlib`, `seaborn`, `numpy`, `pandas`
- Todas las notebooks fueron ejecutadas en el entorno Colab (Google) entre agosto y octubre del año 2024.