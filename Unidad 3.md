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