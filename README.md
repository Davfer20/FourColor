# FourColor
David Fernandez Salas 2022045079
Este trabajo constra en un algoritmo que resuelve el teorema de four color. Este teoema se basa que en un mapa se puede colorear con 4 colores
sin que los lados adyacentes tengan el mismo color. Osea que los mismos colores no se toquen en lados diferentes. Este trabajo mio consta en varias partes

Primero se crea el mapa manualmente como se desea gracias al void regiones

Una de las funciones mas importantes se llama determinarRegiones. La idea de esta funcion era buscar una region tomando el valor que estaba dentro
de ella para ir buscando todas las iguales. Su proposito era tener todos los lados adyacentes que tuviera esta region. Por ejemplo la fila1 y columna1
tiene el valor de region '1' entonces busca todas las regiones 1 y anota en una lista los valores que tiene adyacentes, se intenta que la lista no se
repitan valores para finalmente tener una lista con las regiones vecinas. 

Otra funcion importante es funcionDefinirColor la cual se va a mano con unas funciones complementarias la primera es un struct el cual define ciertas
caracteristicas que tiene una region como el tipo, color y sus adyacencias. Para las adyacencias el reto es que se guarda como un struct el cual es 
dificil de manipular y tomar datos. Tambien se utilizo una funcion llamada repeticion que tiene un entero como parametro de entrada el cual devuelve 
un numero mas alto del ingresado dentro de rango 4. Por ejemplo como son 4 colores y si el color 4 esta ocupado pasa al color 1 entonces siempre devuelve
un color distinto para todos los casos.

La funcion definir color se encarga de recorrer todas las regiones y asignarles un color distinto. Se enfoca que las regiones del lado no tengan los mismos
colores y si eso sucede esta tiene un while hasta que la bandera cambie significando que tiene color diferente. Finalmente se comprara los colores
con las regiones ordenadas asi que por ejemplo si la region 1 y la proxima que es region2 tienen el mismo color devuelve una bandera de error.
