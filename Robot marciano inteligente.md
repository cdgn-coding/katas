# Robot Marciano Inteligente

## Consigna

Los científicos de la Comisión Nacional de Actividades Espaciales (CONAE) lograron mapear la superficie de marte mediante fotografías tomadas 
con telescopios y estimaciones de los relieves. Se te solicita retomar el [robot marciano](https://github.com/cdgn-coding/katas/blob/main/Robot%20marciano.md) 
desarrollado previamente y brindarle la inteligencia de descubrir el camino entre dos puntos de marte.

* El robot se encuentra en alguna posición (x<sub>0</sub>, y<sub>0</sub>)
* Se le da al robot la posición de destino (x<sub>f</sub>, y<sub>f</sub>) y debe indicar si encontró algún camino.
* Si encuentra algún camino, indicar la secuencia de comandos que llevan desde (x<sub>0</sub>, y<sub>0</sub>) a (x<sub>f</sub>, y<sub>f</sub>)
* Si no encuentra camino, el robot debe quedarse en la última posición posible.

## Hint

Se puede mantener la interface de construcción `const rover = new MarsRover(location, direction, grid)`. Implementar al nueva interface que le da inteligencia 
al dispositivo, por ejemplo `const [reached, path] = rover.reach([x, y]`, donde `reached` indica si encontró el camino y `path` es la secuencia de comandos
desde el inicio al destino.

## Nivel 3

Por los resultados que están obteniendo en las estimaciones del relieve marciano, los científicos de la CONAE están interesados 
en hacer una base de datos de caminos óptimos en marte para poder ahorrar combustible en futuras exploraciones.
Se te pide que el robot sea capaz de encontrar el camino más corto entre (x<sub>0</sub>, y<sub>0</sub>) y (x<sub>f</sub>, y<sub>f</sub>).

## Nivel 4

Los científicos de la CONAE encontraron la posibilidad de existencia de minerales valiosos en marte. Se debe agregar al robot
la capacidad de explorar la superficie del planeta para encontrar la posición del mineral especificado,
este debe indicar si encontró algún camino y si es así, dar el camino mas corto como secuencia de comandos.
La interface puede ser parecida a la anterior, por ejemplo `const [reached, path] = rover.find(mineral)`.
La API debe recibir los minerales valiosos en el mapa del planeta.
