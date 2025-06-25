
Este proyecto aplica técnicas de Natural Language Processing (NLP) y Deep Learning para analizar y clasificar el sentimiento expresado en tweets. El objetivo principal fue construir una red neuronal recurrente capaz de identificar si un tweet tiene un tono positivo, negativo o neutral.

Se partió de un dataset real de tweets relacionados con Elon Musk, el cual fue limpiado, preprocesado y utilizado como base para entrenar modelos secuenciales.

Link de acceso: https://colab.research.google.com/drive/1fCjYPmd-MG5aHTRiu890QIjw7E2oIadz?usp=sharing

-Objetivo del Proyecto
Aplicar técnicas fundamentales de preprocesamiento de texto.

Implementar una red neuronal recurrente (RNN) con arquitectura LSTM para clasificación de sentimiento.

Comparar una arquitectura básica vs. una versión mejorada con más capas.

Evaluar si esta arquitectura es adecuada para el problema.

-Pasos del Desarrollo
Carga y exploración del dataset
Se analizaron patrones de sentimiento y frecuencia de palabras.

Preprocesamiento NLP
Incluyó limpieza de texto, tokenización, stopwords y padding.

Codificación de etiquetas
Las clases de sentimiento fueron convertidas a variables categóricas.

Modelo RNN básico
Se implementó un modelo LSTM sencillo con embedding + una capa LSTM.

Modelo RNN mejorado
Se construyó una red más profunda con Bidirectional LSTM, Dropout y capas densas.

Evaluación de resultados
Se compararon métricas de precisión y pérdida en entrenamiento y validación.

-Resultados
El modelo simple alcanzó una precisión moderada.

El modelo mejorado superó el 67% de accuracy en validación.

Se detectó cierto sobreajuste, abriendo el camino para mejorar regularización o usar más datos.

-Conclusión Técnica
La red construida pertenece a la familia de redes recurrentes, y aunque los resultados son aceptables, el rendimiento podría beneficiarse de ajustes adicionales. Este tipo de arquitectura es válida para el problema abordado, pero su efectividad depende del volumen de datos y del ajuste del modelo.
