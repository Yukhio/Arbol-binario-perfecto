¡Oh, no! El último experimento del Comandante Sigma para mejorar la eficiencia de su dispositivo del fin del mundo ha fracasado espectacularmente.
Había estado mejorando la estructura del árbol convertidor de flujo de iones, pero algo salió terriblemente mal y las cadenas de flujo explotaron.
Algunos de los convertidores de flujo de iones sobrevivieron intactos a la explosión, pero a otros se les borraron las etiquetas con la explosión.
El está haciendo que sus secuaces reconstruyan el árbol del convertidor de flujo de iones a mano, pero usted cree que puede hacerlo mucho más rápido, ¡quizás lo suficientemente rápido como para lograr subir de rango!



Las cadenas de flujo requieren árboles binarios perfectos, por lo que el diseño de Sigma acomodó los convertidores de flujo de iones para formar uno.
Para etiquetarlos, realizó un recorrido post-orden del árbol de convertidores y etiquetó cada convertidor con el orden de ese convertidor en el recorrido, comenzando en 1.
Por ejemplo, un árbol de 7 convertidores tendría el siguiente aspecto:

   7
 3   6
1 2 4 5



Escriba una función respuesta (h, q) - donde h es la altura del árbol perfecto de convertidores y q es una lista de enteros positivos
que representan diferentes convertidores de flujo - que devuelve una lista de enteros p donde cada elemento en p es la etiqueta de el
convertidor que se encuentra encima del convertidor respectivo en q, o -1 si no existe tal convertidor. Por ejemplo, respuesta(3, [1, 4, 7])
devolvería los convertidores por encima de los convertidores en los índices 1, 4 y 7 en un árbol binario perfecto de altura 3, que es [3, 6, -1].



El dominio del entero h es 1 <= h <= 30, donde h = 1 representa un árbol binario perfecto que contiene solo la raíz,
h = 2 representa un árbol binario perfecto con la raíz y dos nodos de hoja, h = 3 representa un árbol binario perfecto con la raíz,
dos nodos internos y cuatro nodos de hoja (como el ejemplo anterior), y así sucesivamente.
Las listas q y p contienen al menos uno pero no más de 10000 números enteros distintos, todos los cuales estarán entre 1 y 2^h-1, inclusivo.

Ejemplos

==========



Entrada:

    (entero) h = 3
	(lista de enteros) q = [7, 3, 5, 1]

Salida:

    (lista de enteros) [-1, 7, 6, 3]



Entrada:

    (entero) h = 5
	(lista de enteros) q = [19, 14, 28]

Salida:

    (lista de enteros) [21, 15, 29]
