
El siguiente trabajo analiza un hilo de tweets de Elon Musk

Link de acceso: https://colab.research.google.com/drive/1fKoZ_c1HGMJxdqY53Rg4Ir0U1bHNgp4E?usp=sharing

El trabajo se compone por 2 grandes bloques, el primero es sobre PNL y el segundo contiene Deep learning y Red neuronal.

En la primer etapa vemos como esta compuesto el data set, que columnas tiene:
row ID	Tweet	Time	Retweet from	User 

Luego limpiamos los datos y asignamos sentimientos a cada tweet. Sobre eso se agrego un grafico para ver cuantos tweets se hicieron con cada sentimiento (positivo-neutral-negativo) y como fue la evolucion de los sentimientos en el tiempo.

Ademas de eso, creamos una WordlCloud, para eso aplicamos Lematización.Para ellos se creo un grafico por sentimiento con las palabras mas repetidas. Vale aclarar que hay palabras que se repiten en los 3 sentimientos como "Tesla" donde hace referencia a su marca, no quiere decir que la usa para hacer referencia a algun sentido como tal.

Para la segunda etapa de Deep Learning y redes neuronales se probaron ambos metodos, CNN y RNN.

Concluciones para cada método:

CNN: 

El dataset MNIST contiene 60,000 imágenes de entrenamiento y 10,000 de test, balanceado entre 10 clases.

- Las imágenes son en escala de grises, tamaño 28x28 pixeles, con valores normalizados para el entrenamiento.

- Un modelo sencillo CNN con una sola capa convolucional logró buena precisión (~96%).

- Al agregar capas convolucionales adicionales, una capa densa más grande y Dropout, la precisión mejoró (~98%).

- El aumento de capas permite capturar características más complejas, mejorando el rendimiento del modelo.

RNN:

-Se entrenó una red neuronal recurrente (RNN) con LSTM para clasificar sentimientos en tweets de Elon Musk. El modelo alcanzó una precisión final del 67.24% sobre el conjunto de validación.

-Durante el entrenamiento se observó un comportamiento típico de sobreajuste:

-La precisión de entrenamiento (train accuracy) fue alta, pero la precisión de validación (val accuracy) se mantuvo más baja.

-La pérdida en validación (val loss) fue mayor que la de entrenamiento y aumentó con las épocas.

-Esto indica que el modelo aprendió muy bien los datos de entrenamiento, pero no logra generalizar correctamente a datos nuevos. Se recomienda aplicar estrategias para reducir el sobreajuste, como usar más datos, ajustar hiperparámetros o incorporar regularización adicional.
