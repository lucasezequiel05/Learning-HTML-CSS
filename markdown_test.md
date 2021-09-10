# Título1  
## Título2  
### Subtítulo 

Encabezado1
==

Encabezado2
--

Este es un ejemplo de texto que da entrada a una lista genérica de elementos:

- Elemento 1
+ Elemento 2
* Elemento 3
    - Elemento 4 en una lista anidada.
- Elemento 5

Este es un ejemplo de texto que da entrada a una lista numerada. Para crearla se utiliza el estilo *"numero. "*:  

1. Elemento 1
2. Elemento 2
3. Elemento 3

Al texto en Markdown puedes añadirle formato como **negrita** o *cursiva* de una manera muy sencilla.  
Para utilizar ambas combinadas ***cursiva y negrita.***  

Este es un nuevo párrafo.  
Auto.  
Casa.

> "Esto es una cita.  
De dos renglones."  
  
> Este es otra cita.
>
>> Esta es una cita anidada.  
>
> Acá termina


Las Reglas / Lineas de separación horizontales se crean en un renglón en blanco con 3 símbolos sean asteriscos, guión o guión bajo, juntos o separados por un espacio cada uno.

***
---
___
* * *
- - -

## MOSTRAR LOS SIMBOLOS OMITIENDO MARKDOWN:

Antepongo la barra invertida antes del símbolo `\. , \* , \#`

## CREAR LINKS:  

`[Descripción del Link entre corchetes](URL entre paréntesis)`  

`[Enlace a tutorial](https://markdown.es/sintaxis-markdown/)`  

[https://github.com/](https://github.com/)

Enlace a GitHub [Aquí](https://github.com/) .  


## CREAR ENLACE DE REFERENCIA:
Consiste en utilizar una referencia que guarda nuestro enlace y de esta forma evitamos declarar la sintaxis de enlace en el texto cada vez que sea requerido.

[link]: https://www.youtube.com/

Este es un texto de ejemplo [Enlace23][link].

Para mostrar la URL completa y no dentro de un enlace enmascarado: 

<https://www.youtube.com//>

***
## INDICAR CÓDIGO:

Para introducir código dentro de una oración se escribe dentro de dos comillas simples `LÍNEA DE CÓDIGO como etiqueta de html <code>`.

Para declarar un código de bloque como la etiqueta de texto preformateado < pre >:  

    Línea de código declarada con 4 espacios en blanco al inicio.

~~~
Este es un bloque de código.  
La virgulilla en este taclado es: AltGr + 4
~~~  

Declarando el lenguaje al que se hace referencia en el bloque de código:

\~\~\~python  
print("Hello world!")  
\~\~\~

***
## INSERTAR UNA IMAGEN

Se compone de 4 parámetros:
+ ! signo de exclamación al inicio
+ [] Texto a mostrar en caso de error de carga
+ () Ruta de acceso a la imagen
+ "" Título en caso de detener el cursor sobre la imagen

~~~
Sintaxis:

![msj error][ruta/hacia/la/ubicación/de/la/imágen "Título"]  
~~~

Ejemplo:

![Visual studio code logo](https://regmedia.co.uk/2015/11/27/visual_studio_code_logo.jpg?x=198&y=131&crop=1 "VSC logo")

También se puede referenciar el enlace a la imagen como en el caso de los links.  
A continuación un caso de una imagen no encontrada y su mensaje para este caso:

~~~
[img1]: /ruta/inexistente/nodisponible.jpg "titulo de imágen"

![Imágen no disponible](img1)
~~~

[img1]: /ruta/inexistente/null.jpg "Título de Imágen"

![Imágen no disponible](img1)  

***

## TABLAS

Se utiliza las filas de línea punteada para separar e indicar los títulos de columna del contenido de cada fila:

~~~
| Columna1 | Columna2 |
| -------- | -------- |
| Fila_1 | Descripción |
| Fila_2 | Descripción |
~~~

| Columna1 | Columna2 |
| -------- | -------- |
| Fila_1 | Descripción |
| Fila_2 | Descripción |

La alineación del texto depende de la posición de los "dos puntos :" 
+ :-- a la izquierda
+ --: a la derecha
+ :--: centrado

| Columna1 | Columna2 |
| ------: | :------: |
| Fila_1 | Descripción |
| Fila_2 | Descripción |


***
## CREAR COMENTARIOS

~~~html
<!-- Un comentario-->
~~~
***

## RECURSOS PARA GITHUB


#### **REALIZAR MENCIONES DE USUARIOS**

`@username`

#### **INSERTAR EMOJIS**

Colocar nombre del emoji entre dos símbolos " : "  
`:octocat:`

Fuente: <https://emojipedia.org/github/>

#### **CREAR CASILLA DE TAREAS**

~~~
- [ ] Casilla1
- [ ] Casilla2
- [x] Casilla3
~~~
- [ ] Casilla1
- [ ] Casilla2
- [x] Casilla3

***
## VINCULAR ENLACE A UN EMAIL:

Dentro de la sección de enlace anteponemos la palabra `mailto:`  

    Este es un link a [adress@gmail.com](mailto:adress@gmail.com)

***
Comando para convertir archivo markdown a html. Utilizando pandoc a través de la consola: `pandoc -f markdown Hello.md > Hello.html `.  

Activar el previsualizador de markdown de VSC:
1. view
2. command palette
3. Markdown: open preview

***
