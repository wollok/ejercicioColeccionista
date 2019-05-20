# Ejercicio: Coleccionista
 
[![Build Status](https://travis-ci.org/wollok/ejercicioColeccionista.svg?branch=master)](https://travis-ci.org/wollok/ejercicioColeccionista)


Se trata de una aplicación que sirve para que una persona, dueña de una galería de elementos coleccionables
los administre. 
  
De un elemento coleccionable interesa saber:
	- su valor 
 	- si es frágil o no 
 	- su categoría.

Para iniciar, ya vienen programados algunos objetos: 
	- Hay dos categorías: juguete y música. Por supuesto, podrían aparecer más categorías (debe ser sencillo agregar nuevas), 
	- Elementos coleccionables iniciales:
        	- Soldado de plomo: Es frágil, vale 500 y es un juguete
         	- Casssette de Cantaniño: No es frágil, vale 900 y es musical
         	- Muñeco de He-man: No es frágil, vale 800 y es un juguete
         	- Disco de vinilo de La Balsa:  Es frágil, vale 1500 y es musical
Por supuesto, podría haber más elementos coleccionables (debe ser sencillo incorporar nuevos elementos).
      
También viene la definición de un objeto 'coleccionista' que modela al dueño de la galería. La implementación de dicho
    objeto está vacía y completarla es lo que se exige en el punto 1.
  
Finalmente, existe la definición de un objeto guitarra eléctrica, que modela un objeto coleccionable distinto de los ya preprogramados
Este objeto también tiene su implementación vacía y completarlo es lo que se exige en el punto 2. Para esto podría necesitar de 
objetos nuevos no predefinidos en el examen.
  
El código inicial incluye una serie de test programados (no deberían ser modificados) que deben ejecutarse con éxito. 
  
Puede acceder a cualquier material "no humano" de consulta. En especial, la guía de colecciones y closures accesible en el sitio
web de la materia.
  
## Punto 1) COLECCIONES
Hacer que el objeto coleccionista entienda los siguientes mensajes:  
  - agregarElemento(unElemento) -> agrega un elemento a la galería de elementos.
  - quitarElemento(unElemento) -> elimina un elemento de la galería de elementos.
  - objetosFragiles() -> devuelve todos los elementos de la galeria que son frágiles.
  - objetoFragilMasCaro() -> devuelve el objeto frágil de mayor valor.
  - valorEnObjetosFragiles() -> devuelve la suma de los valores de todos los objetos frágiles de la galería.
  - valorEnCategoria(unaCategoria) -> devuelve la suma de los valores de todos los objetos de la galería que pertenecen a la categoría dada.
  - existeElementoDe(unaCategoria) -> indica si en la galería existe algún elemento que pertenezca a la categoría dada.
  - categorías() -> devuelve todas las categorías en las cuales el coleccionista posea al menos un elemento.
  - todosValiosos() -> indica si la colección sólo posee elementos valiosos. Un elemento es considerado valioso para el coleccionista 
     si el valor supera $600
  
En el archivo 'coleccionista.wtest' están programados todos los test necesarios para probar los mensajes anteriores. 
Por supuesto, los test fallan actualmente. Debés agregar el código necesario para que los test den resultados positivos.
Se puede agregar nuevos test de considerarse necesario, pero para este examen alcanza con los provistos por los docentes.
  
#  Punto 2) POLIMORFIMSO
El dueño de la galería posee una guitarra eléctrica que quiere incorporar a su galería.
Como es un luthier experto, suele jugar a cambiar los micrófonos. También la guitarra se puede guardar en distintos estuches. 
  - El valor de la guitarra electrica es de 10000 más el valor de los micrófonos. En principio el coleccionista tiene dos micrófonos distintos, 
    los gibson (que valen 1000) y los Di Marzio (que valen 800). El dueño planea comprar nuevos micrófonos, por lo que la solución debe 
    permitir hacer esto sencillamente
  - La fragilidad de la guitarra depende del estuche donde se guarda: El estuche flexible hace que la guitarra sea frágil, mientras que el rígido no
    Podrían aparecer nuevos estuches en el futuro.
  - La categoría de la guitarra eléctrica es música.
  
Para este punto no se proveen objetos preprogramados (salvo la definición del objeto guitarra eléctrica con una implementación vacía). 
Se provee además un archivo 'coleccionistaConGuitarra.wtest' que prueba que un coleccionista que tiene sólo una guitarra en su galería 
funcione bien. 
IMPORTANTE: La solución de este punto puede implicar la aparición de nuevos objetos! 
Nota: A efectos de este examen no es necesario agregar nuevos test. Pero es importante aclarar que, en un sistema real, las buenas prácticas exigirían que todos los objetos estén testeados individualmente, y no solo a través de los test del coleccionista. 
  
  


