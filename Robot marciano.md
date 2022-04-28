# Robot marciano

## Consigna

Desarrolla una API que permita mover un robot en la superficie de marte.

* Inicialmente se da un punto de inicio del robot (x, y), la dirección a la que apunta y el tamaño de la grilla.
* Las direcciónes puede ser
  * Norte (N)
  * Sur (S)
  * Este (E)
  * Oeste (O)
* El robot puede ejecutar una cadena de comandos
* Los comandos que puede entender el robot son:
  * Moverse adelante (f)
  * Moverse hacia atras (b)
  * Girar a la izquierda (l)
  * Girar a la derecha (r)
* Los bordes de la grilla se unen (dado que la superficie del planeta es una esfera)

## Hint

El constructor, por ejemplo, puede ser así `new MarsRover(location, direction, grid)`.
Si instanciamos el robot con estos parámetros `const rover = new MarsRover([0, 0], 'e', [50, 50])` y ejecuta el comando `fflff`,
entonces el robot debería encontrarse en las coordenadas `(2, 2)`.


## Nivel 2

Dar al robot la capacidad de detectar obstaculos. Si una secuencia de comandos encuentra un obstáculo,
entonces el robot deberia quedarse en la última posición posible y reportar el obstáculo.
El API debe poder recibir los obstáculos que existen en el mapa del planeta.
