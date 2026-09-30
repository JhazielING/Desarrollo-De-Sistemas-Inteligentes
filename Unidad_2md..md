Actividad 1: Ejemplos machine learning:
**1. Detectar correos spam**

- **T:** Clasificar un correo como spam o no spam.
- **P:** Porcentaje de correos clasificados correctamente.
- **E:** Correos anteriores marcados como spam y no spam.

**2. Recomendar películas**

- **T:** Recomendar películas que le puedan gustar al usuario.
- **P:** Porcentaje de recomendaciones que el usuario califica positivamente.
- **E:** Historial de películas vistas y calificadas.


# ACT 2.1

## Ejemplos de aplicaciones donde se muestran T, E y P

### Spotify

**Tarea (T):** Identificar qué canciones podrían ser del agrado de una persona y sugerírselas.

**Experiencia (E):** El sistema utiliza información como las canciones que escucha, las que omite, las que guarda y las listas que reproduce.

**Medición (P):** Se puede evaluar el funcionamiento observando cuántas canciones recomendadas son reproducidas, guardadas o escuchadas durante cierto tiempo.

### Google Maps

**Tarea (T):** Calcular rutas para ayudar al usuario a llegar de un lugar a otro.

**Experiencia (E):** Utiliza información de recorridos anteriores, tráfico, velocidades de los vehículos y datos de ubicación para aprender sobre las condiciones de las rutas.

**Medición (P):** Se puede medir qué tan acertadas son las estimaciones del tiempo de llegada y qué tan bien las rutas evitan zonas con tráfico.

## Planteamiento y solución de problemas mediante Machine Learning

### ¿Qué es Machine Learning?

El Machine Learning es una forma de inteligencia artificial en la que una computadora puede aprender a realizar una actividad utilizando datos y ejemplos, en lugar de depender únicamente de instrucciones escritas específicamente para cada situación.

Para plantear un problema de Machine Learning se pueden identificar tres elementos principales:

- **Tarea (T):** Es la actividad que queremos que el sistema realice.
    
- **Experiencia (E):** Son los datos o ejemplos que utiliza el sistema para aprender.
    
- **Medición (P):** Es la forma en la que comprobamos qué tan bien está funcionando.
    

### Proceso para resolver un problema con Machine Learning

1. **Establecer el objetivo:** Primero se determina qué actividad queremos que realice el sistema.
    
2. **Obtener datos:** Se recopila información relacionada con el problema para que pueda ser utilizada durante el aprendizaje.
    
3. **Definir una métrica:** Se decide cómo se determinará si el sistema está dando buenos resultados.
    
4. **Entrenar el modelo:** El algoritmo analiza los datos disponibles y encuentra patrones que le permitan realizar la tarea.
    
5. **Comprobar los resultados:** Se prueba el modelo con información que no utilizó durante el entrenamiento.
    
6. **Realizar mejoras:** Si los resultados no son suficientemente buenos, se pueden modificar los datos, el modelo o el proceso de entrenamiento y volver a probarlo.
    

## Tipos principales de Machine Learning

### Aprendizaje supervisado

En este tipo de aprendizaje, el sistema recibe ejemplos en los que ya conocemos cuál debería ser el resultado. A partir de esos ejemplos, busca aprender la relación entre los datos de entrada y la respuesta correcta.

### Aprendizaje no supervisado

Aquí el sistema recibe información sin que se le indiquen previamente las respuestas correctas. Su función es encontrar características, grupos o patrones que existan dentro de los datos.

### Aprendizaje por refuerzo

El sistema aprende mediante la interacción con un entorno. Realiza diferentes acciones y recibe recompensas o penalizaciones dependiendo de los resultados obtenidos, por lo que poco a poco aprende qué decisiones le convienen más.

# ACT 2.2

## Clasificaciones de Machine Learning explicadas con mis propias palabras

### Aprendizaje supervisado

Es cuando una computadora aprende utilizando ejemplos que ya tienen una respuesta conocida. El sistema compara lo que calcula con la respuesta correcta y, con base en esa información, va mejorando sus resultados.

**Ejemplo:** Enseñarle a identificar si una fotografía contiene un perro o un gato utilizando imágenes que previamente ya fueron identificadas.

### Aprendizaje no supervisado

En este caso, la computadora recibe los datos pero no tiene las respuestas indicadas. Por sí misma analiza la información y trata de encontrar semejanzas, diferencias o grupos dentro de los datos.

**Ejemplo:** Una tienda puede utilizar este método para encontrar grupos de clientes que tienen hábitos de compra parecidos sin decirle previamente cuáles son esos grupos.

### Aprendizaje por refuerzo

Es una forma de aprendizaje en la que el sistema va tomando decisiones y aprende de las consecuencias de cada una. Cuando realiza una acción adecuada obtiene una recompensa y cuando toma una mala decisión recibe una penalización o una recompensa menor.

**Ejemplo:** Un programa que aprende a jugar un videojuego probando diferentes movimientos y descubriendo cuáles le permiten obtener más puntos.





**Caja Blanca:** Podemos entender l proceso interno.
**Caja Negra:** Vemos entrada y salida, pero el proceso interno es difícil de explicar.

### 1. Árbol de decisión

**Definición:**  
Es un algoritmo de aprendizaje automático que toma decisiones siguiendo una estructura parecida a un árbol, donde cada pregunta o condición divide los datos hasta llegar a una decisión final.

**Cómo funciona:**  
Comienza con todos los datos y va haciendo preguntas sobre sus características. Cada respuesta divide los datos en grupos más pequeños hasta llegar a una clasificación o resultado. Las ramas representan las diferentes decisiones y las hojas representan el resultado final.

**Caso de uso:**  
Un banco puede utilizar un árbol de decisión para determinar si una persona puede recibir un préstamo tomando en cuenta factores como sus ingresos, edad, historial crediticio y deudas.

Quinlan, J. R. (1986). Induction of decision trees. _Machine Learning, 1_, 81–106. https://doi.org/10.1007/BF00116251

### 2. Regresión logística

**Definición:**  
Es un algoritmo utilizado principalmente para problemas de clasificación, especialmente cuando se quiere determinar entre dos posibles resultados.

**Cómo funciona:**  
Analiza diferentes características de los datos y calcula una probabilidad de que pertenezcan a una determinada categoría. Después, utilizando un límite de decisión, convierte esa probabilidad en una clasificación.

**Caso de uso:**  
Se puede utilizar para determinar si un correo electrónico es **spam o no spam**, analizando características como las palabras utilizadas, el remitente y la frecuencia de ciertos términos.

Hosmer, D. W., Lemeshow, S., & Sturdivant, R. X. (2013). _Applied logistic regression_ (3rd ed.). Wiley. [https://doi.org/10.1002/9781118548387](https://doi.org/10.1002/9781118548387)

### 3. K vecinos (K-NN)

**Definición:**  
K-NN es un algoritmo que clasifica un dato nuevo basándose en los datos que se encuentran más cerca de él.

**Cómo funciona:**  
Primero se elige un número de vecinos, representado por **K**. Cuando llega un dato nuevo, el algoritmo busca los K datos más cercanos y determina su categoría según la mayoría de ellos.

**Caso de uso:**  
Puede utilizarse para clasificar una fruta como manzana, naranja o plátano comparando características como su peso, tamaño y color con frutas que ya están clasificadas.

Cover, T., & Hart, P. (1967). Nearest neighbor pattern classification. _IEEE Transactions on Information Theory, 13_(1), 21–27. [https://doi.org/10.1109/TIT.1967.1053964](https://doi.org/10.1109/TIT.1967.1053964)

### 4. Naive Bayes

**Definición:**  
Es un algoritmo de clasificación basado en probabilidades y en el teorema de Bayes. Calcula qué tan probable es que un dato pertenezca a una determinada categoría considerando sus características.

**Cómo funciona:**  
Analiza la probabilidad de cada categoría y la combina con la evidencia que proporcionan las características del dato. Después selecciona la categoría que tenga la mayor probabilidad.

**Caso de uso:**  
Se puede utilizar para clasificar mensajes como **spam o no spam**, calculando la probabilidad de que un mensaje sea spam según las palabras que contiene.

Rish, I. (2001). An empirical study of the naive Bayes classifier. _IJCAI 2001 Workshop on Empirical Methods in Artificial Intelligence_, 41–46.
### 5. SVM (Support Vector Machine)

**Definición:**  
Es un algoritmo de aprendizaje automático que busca separar diferentes categorías de datos mediante una frontera o límite de decisión.

**Cómo funciona:**  
Busca la línea o plano que permita separar las diferentes clases dejando la mayor distancia posible entre ellas. Los datos que quedan más cerca de esa frontera son llamados vectores de soporte.

**Caso de uso:**  
Puede utilizarse para clasificar imágenes, por ejemplo, para determinar si una imagen contiene un perro o un gato.

Cortes, C., & Vapnik, V. (1995). Support-vector networks. _Machine Learning, 20_, 273–297. [https://doi.org/10.1007/BF00994018](https://doi.org/10.1007/BF00994018)

### 6. Bosque aleatorio (Random Forest)

**Definición:**  
Es un algoritmo que combina varios árboles de decisión para obtener una predicción más confiable.

**Cómo funciona:**  
Construye muchos árboles de decisión utilizando diferentes partes de los datos y características. Cada árbol realiza su propia predicción y posteriormente se combinan todas las respuestas para obtener el resultado final.

**Caso de uso:**  
Una empresa puede utilizarlo para predecir si un cliente tiene probabilidades de cancelar un servicio utilizando información como antigüedad, pagos, uso del servicio y tipo de contrato.

Breiman, L. (2001). Random forests. _Machine Learning, 45_, 5–32. https://doi.org/10.1023/A:1010933404324

### 7. Red neuronal

**Definición:**  
Es un modelo de aprendizaje automático inspirado en la forma en que funcionan las conexiones entre neuronas. Está formada por diferentes capas de nodos que procesan información.

**Cómo funciona:**  
Los datos entran por una capa de entrada y pasan por una o varias capas ocultas donde se realizan diferentes cálculos. Finalmente, una capa de salida genera la predicción. Durante el entrenamiento, la red modifica sus parámetros para reducir los errores de sus predicciones.

**Caso de uso:**  
Las redes neuronales se utilizan en sistemas de reconocimiento de imágenes, por ejemplo, para identificar objetos, personas o animales dentro de una fotografía.

Breiman, L. (2001). Random forests. _Machine Learning, 45_, 5–32. https://doi.org/10.1023/A:1010933404324
