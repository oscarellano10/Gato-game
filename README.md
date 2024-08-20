# Gato-game

El juego que he seleccionado para este proyecto es el juego de gato. Se me hace un juego interesante que se ve simple pero ya tomando un paso atras se vuelve un poco más complejo. Como ya tengo previos conocimientos escribiendo código con Python me gustaría usar esos conocimientos e involucrar un aspecto gráfico al juego usando la librería de Turtle.

Antes de empezar con el algoritmo, voy a explicar la estructura del código. Usando 2 listas voy a basarme en todo el código. La primera lista sería una donde se establece el estado de cada cuadro del gato. Sería algo asi, ["-","-","-"]. Esto representa la fila de arriba del gato. La segunda lista que estructura el código es uno con coordenadas. Usando el ejemplo de la primera fila del gato, la lista quedaría como, [(-200, 200),(0, 200),(200, 200)]. Usando tupels puedo hacer una lista coon coordenadas facilmente. Ahora que ya tenemos la estructura del código definido, podemos empezar con el algoritmo.

1. Usando los gráficos de Turtle, dibujaré los cuadritos del gato, y en cada cuadro tendrá un numero que le corresponde.
2. El user luego tendrá que picarle un numero de uno de los cuadros para poner su X. Este es la primera y unica entrada. Esto se usará usando el listen_on_key function de Turtle.
3. El código checará si el espacio está disponible usando la lista del grid. Si está disponible, se dibujará la X del jugador en las coordenadas de la lista de las coordenadas.
4. La computadora luego pondrá una respuesta para hacer un counter contra el jugador. Es decir, buscará un espacio disponible random para poner su pieza.
5. Las piezas se dibujarán usando Turtle.
6. Cuando ambas piezas son puestas, el código checará si se han usado 3 cuadritos seguidos por el jugador y luego la computadora. Si se cumple esta función, el juego acabará y se declarará el ganador.
7. Existirá una variable global que simboliza los turnos. Si no hay ningun ganador despues de 9 rondas, se acabará el juego.
8. Los últimos 6 pasos se repetirarán en un Loop hasta que un jugador gane o turnos lleguen a 9.
9. En un archivo .csv se escribirá el ganador y en cuantas rondas.
