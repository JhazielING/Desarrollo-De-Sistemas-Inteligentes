1. **Problemas de búsqueda:** Son problemas en los que se necesita encontrar una solución entre diferentes posibilidades, explorando caminos o acciones hasta alcanzar un objetivo determinado.

2. **Espacios de estados:** Es el conjunto de todos los estados o situaciones posibles por los que puede pasar un problema desde el inicio hasta llegar a una solución.

3. **Estado inicial:** Es la situación o condición en la que comienza un problema y desde la cual el agente inicia la búsqueda de una solución.

4. **Acciones:** Son las operaciones o movimientos que se pueden realizar para pasar de un estado a otro y acercarse al objetivo deseado.

5. **Modelo de transición:** Es la descripción de cómo cambia un estado cuando se realiza una acción determinada. Permite conocer cuál será el siguiente estado.

6. **Prueba de meta:** Es el procedimiento que permite comprobar si el estado actual cumple con las condiciones necesarias para considerar que se ha alcanzado el objetivo.

7. **Costo del camino:** Es la suma de los costos de todas las acciones realizadas desde el estado inicial hasta llegar a un estado determinado. Permite comparar diferentes caminos.

8. **Solución:** Es una secuencia de acciones que permite pasar del estado inicial a un estado que cumple con el objetivo del problema.

9. **Frontera:** Es el conjunto de nodos que ya fueron descubiertos, pero que todavía están pendientes de exploración. Su organización depende del algoritmo de búsqueda utilizado.

10. **Nodo:** Es una estructura que representa un estado dentro del árbol de búsqueda y puede contener información sobre las acciones realizadas, el nodo padre y el costo acumulado.

11. **Agente de resolución de problemas:** Es un sistema inteligente que identifica un objetivo, analiza las posibles acciones y busca una secuencia de pasos para alcanzar una solución.

**Sistemas de búsqueda:** 
1. **Búsqueda no informada:** Es un método que explora los estados posibles sin utilizar información adicional que indique qué camino es más conveniente para alcanzar el objetivo. Se basa en las reglas del problema.

2. **Búsqueda en amplitud:** Es un algoritmo que explora primero todos los nodos de un mismo nivel antes de avanzar al siguiente. Cuando cada acción tiene el mismo costo, encuentra la solución con menos pasos.

3. **Búsqueda en profundidad:** Es un algoritmo que sigue un camino hasta donde puede llegar antes de regresar y explorar otras opciones. Utiliza menos memoria en algunos casos, pero puede tardar en encontrar la solución.

4. **Búsqueda de costo uniforme:** Es un algoritmo que siempre explora primero el camino con el menor costo acumulado. Puede encontrar la solución óptima si los costos de las acciones son positivos.

5. **Cola:** Es una estructura de datos que organiza los elementos según el orden en que llegan. El primero en entrar es el primero en salir (FIFO), y se utiliza en la búsqueda en amplitud.

6. **Pila:** Es una estructura de datos en la que el último elemento en entrar es el primero en salir (LIFO). Se utiliza para implementar la búsqueda en profundidad.

7. **Completitud:** Es la propiedad de un algoritmo que garantiza encontrar una solución si existe, siempre que se cumplan ciertas condiciones del problema y del algoritmo.

8. **Optimalidad:** Es la capacidad de un algoritmo para encontrar la mejor solución posible, generalmente aquella que tiene el menor costo total entre todas las soluciones disponibles.

9. **Complejidad en tiempo:** Es una medida de la cantidad de operaciones o del tiempo de ejecución que necesita un algoritmo para resolver un problema, según el tamaño de la búsqueda.

10. **Complejidad en espacio:** Es la cantidad de memoria que necesita un algoritmo para almacenar los nodos, estados y demás información durante el proceso de búsqueda.



**1: Breadth First Search (BFS): Explora los caminos por niveles, revisando primero los puntos más cercanos al inicio hasta encontrar el destino.**

![[Captura de pantalla 2026-10-08 181523.png]]


**2: Best First Search: Selecciona el siguiente punto según una estimación de qué tan cerca se encuentra del destino, buscando llegar a él de manera más directa.**
![[Captura de pantalla 2026-10-08 181608.png]]


**3: Dijkstra: Encuentra el camino de menor costo desde el punto A hasta el punto B, considerando la distancia o el peso de cada conexión.**
![[Captura de pantalla 2026-10-08 181706.png]]





**Actividad 3.2:**

## (Manhattan, sin diagonal)

***1: ¿Qué longitud tiene el camino?*** 
Tiene una longitud de **29**.

**2: ¿Cuánto tiempo tardó?****  
Tardó **0.2000 ms**, con 301 operaciones. Fue el más rápido de los tres.

**3: ¿Qué diferencia observas?****  
Explora solo una zona pequeña del mapa, concentrada entre el inicio y la meta. Esto pasa porque la heurística Manhattan lo guía hacia el nodo rojo. Con eso llega al mismo largo de camino que BFS sin diagonal (29), pero con unas 8 veces menos operaciones (301 contra 2331).
![[Captura de pantalla 2026-10-14 155307.png]]

## Breadth-First-Search (con Allow Diagonal)

**1: ¿Qué longitud tiene el camino?**
Tiene una longitud de **23.14**.

**2: ¿Cuánto tiempo tardó?**
Tardó **1.5000 ms**, con 1985 operaciones. Fue el más lento de los tres.

**3: ¿Qué diferencia observas?**  
Es el único con camino **más corto** (23.14) y con **líneas inclinadas**, porque puede cortar en diagonal. Cada diagonal cuesta aprox. 1.41 en vez de 2 movimientos rectos. A cambio tardó más, porque cada nodo revisa hasta 8 vecinos. Además, el área explorada es muy grande, ya que BFS no sabe dónde está la meta.
![[Captura de pantalla 2026-10-14 155356 1.png]]

## Breadth-First-Search (sin diagonal)

**1: ¿Qué longitud tiene el camino?**  
Tiene una longitud de **29**.

**2: ¿Cuánto tiempo tardó?**
Tardó **0.4000 ms**, con 2331 operaciones.

**3: ¿Qué diferencia observas?**  
Es el que **más nodos exploró** (2331), con un área celeste enorme en forma de círculo o rombo que se expande en todas direcciones. El camino va en forma de escalera, solo con movimientos rectos. Tiene la misma longitud que A* (29), pero A* llegó ahí explorando mucho menos.
![[Captura de pantalla 2026-10-14 155424.png]]




















**Actividad 3.4:**

**1:¿Que relación las gpus con las redes neuronales y las neuronas? Como se beneficiaron un de otra?**
Las GPU se relacionan con las redes neuronales porque permiten realizar muchos cálculos al mismo tiempo, lo que ayuda a entrenarlas de manera más rápida. Las redes neuronales están inspiradas en las neuronas del cerebro humano, ya que procesan información y aprenden a reconocer patrones. Las GPU se beneficiaron de las redes neuronales porque aumentó su uso y desarrollo, mientras que las redes neuronales aprovecharon la potencia de las GPU para mejorar su aprendizaje y rendimiento.

**Actividad 3.5:** Diagrama redes neuronales
![[Captura de pantalla 2026-10-21 163038.png|700]]