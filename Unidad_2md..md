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
