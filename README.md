# xml-python
*Durante el curso 2023-2024, he adquirido una serie de conocimientos para el desarrollo informático en mi ámbito profesional como administrador de sistemas. Me gustaría realizar un análisis específico de los temarios que he aplicado en las asignaturas de Lenguajes de Marcas y Programación.*

## PYTHON ##

**Que es Python?**

Python es un lenguaje de programación de alto nivel, interpretado y versátil, conocido por su sintaxis clara y su amplia gama de aplicaciones, desde desarrollo web hasta inteligencia artificial. Es fácil de aprender, multiplataforma y cuenta con una gran comunidad de desarrolladores y bibliotecas.

**Variables**

Es un espacio de almacenamiento donde se guardará un valor que puede ser modificable y que puede ir variando
a lo largo de la ejecución del programa. Se declara con un nombre para poder referenciar durante el programa a
esa variable

**Reglas de Variables**

1. El nombre de la variable sea lo más descriptivo posible del contenido que va a tener esa variable.
2. El nombre de la variable siempre comenzará por una letra en minúscula o un guion bajo:    , alumno1, _alumno, _alumno1
3. No puede haber separación en el nombre de la variable si el nombre tuviera más de una palabra. Podemos utilizar un guion bajo para separar los nombres.
4. En el caso que el nombre de la variable tenga más de una palabra se puede indicar las dos palabras juntas y la primera letra de la segunda palabra en mayúscula.
5. No pueden contener caracteres especiales excepto el guion bajo para separación de dos palabras en el nombre de la variable. No se puede poner en el nombre de una variable: ‘,’ ‘.’ ‘?’, ‘¿’, ‘!’, ‘$’, ‘%’,‘&amp;’,etc.
6. El nombre de la variable no puede ser una palabra reservada del lenguaje

**Tipos de Variables**

El tipo de variable no se declara, en Python se calcula automáticamente a partir del valor inicial que se le asigna
al nombre de la variable, Python reconoce a partir de ese valor que tipo de variable se trata.

Se crea la variable asignándole mediante el operador = el valor que tiene de inicio. Este proceso recibe el nombre
de inicializar una variable. Este proceso de inicializar una variable es obligatorio en Python, ya que reconoce que
tipo de variable se trata a partir del valor inicial.

* edad = 23  Entero int: Números negativo o positivos sin decimales: -5, -9, 0, 256, 65852 
* nota_media = 6.5  Decimal float: Números positivos o negativos con decimales: -5.25, 6.256, 89.25698514
* letra = ‘a’ nombre = ‘Antonio’  Cadenas de caracteres (string): Es un solo carácter o un conjunto de caracteres. Se representa mediante comillas simples o dobles, es decir “Antonio” o ‘Antonio”, o también “a” o ‘a’
* mayorEdad = False  Booleanos o lógicos. Únicamente pueden tomar dos posibles valores True (Verdadero) o False (Falso)

**Entrada de datos estándard.**

La entrada de datos estándar se realiza mediante teclado y se solicita al usuario mediante un mensaje indicando
que debe realizar, para este proceso se utiliza la sentencia input, indicando entre comillas (simples o dobles) el
‘mensaje’) y el valor que el usuario introduce por teclado, que recoge la función input, se asigna a una variable.

numero = input(‘Introduce numero entero’)

Cualquier dato introducido desde teclado, la función input lo lee siempre como cadena de caracteres, por tanto,
tendremos que convertir esa cadena de texto en otro tipo de dato si fuera necesario.

* int(valor): Convierte el texto introducido a número entero. En caso que no se pueda convertir, es decir,
el formato del valor introducido no es equivalente a un entero, muestra un error y no continúa
ejecutando el resto del programa.
* float(variable): Convierte el texto introducido a número con decimales. En caso que no se pueda
convertir, es decir, el formato del número introducido no es equivalente a un número con decimales,
muestra un error y no continúa ejecutando el resto del programa.

**Salida de datos estándard**

* Únicamente un mensaje: Este mensaje puede ser de un posible error, aviso o información en la aplicación,
se indica con la función print entre paréntesis y comillas (simples o dobles) el mensaje que queremos
mostrar.

1. print(“Error: El número no es válido”)
2. print(“El número debe ser mayor que cero”);
3. print(“Se ha dado de alta correctamente al usuario”)

* Únicamente el valor de una variable: Se indica el print entre paréntesis el nombre de la variable.
  
1. print(suma)
2. print(numero)

* Un mensaje junto con el valor de una variable: Se indica en el print entre paréntesis y de forma concatenada
con el operador + el mensaje y el nombre de la variable. Teniendo en cuenta que lo que debe imprimir es
una cadena de texto (string), si el valor de la variable es numérico (entero o float), tenemos que convertirlo
a string con la función str(nombre_variable). En caso de no realizar la conversión, el programa finaliza con el
error: TypeError: can only concatenate str (not &quot;int&quot;) to str

* print(&quot;La suma es: &quot; + str(suma))
* a = &quot;Hola&quot; (string)
* b = 23 (int)
* print(&quot;El mensaje es &quot; + a)  El mensaje es Hola
* print(&quot;El mensaje es &quot; + a + &quot;, bienvenido a Python&quot;)  El mensaje es Hola, bienvenido a Python
* print(&quot;La edad del alumno es &quot; + str(b))  La edad del alumno es 23


  > La función print en Python imprime automáticamente un salto de línea si no se indica el parámetro end. Si se
desea que imprima por pantalla sin efectuar un salto de línea, debemos incluir el parámetro end = “”, que evita
que se produzca un salto de línea en la impresión por pantalla.

**Operadores Aritméticos:**

![Alt](https://lh5.googleusercontent.com/proxy/l_uTj1DPMx5ZKyTLU5YCmWDt8DbbCIKgidakwMTOjTJG7WHrZCZzYdIfOVEJPHVTd2YXSrqYy9S9L-bCrKTjmw)



**Operadores Relacionales:**

![Alt](https://static.platzi.com/media/user_upload/3-cfdd4483-f912-448c-a65c-8e3e4682001c.jpg)

**Estructuras y condicionales**

Es una estructura cuyo interior se ejecuta en base a una condición, el contenido de una estructura alternativa se
ejecutará siempre que se cumpla una determinada condición (expresión), o, dicho de otra forma, si esa condición
es VERDADERA.
En lenguaje Python tenemos las siguientes estructuras alternativas:

**Condicion if:**

*Esta estructura ejecutará la sentencia o sentencias que se incluyan en ella cuando la condición de la
estructura if sea verdadera. En caso de que la condición sea falsa no entrará dentro de la estructura if y
continuará ejecutando el resto del programa. Puede darse el caso, depende del valor de la condición, si es
falsa, nunca entrará en esta estructura y no ejecutará el contenido que tenemos en el interior.*

**Condicion Doble(if-else):**

*Esta estructura ejecutará la sentencia o sentencias que se incluyan en ella cuando la condición de la
estructura if sea verdadera y en caso contrario, si es falsa, se ejecutarán las sentencias incluidas dentro de la
estructura else. Después de ejecutar una de las dos posibles estructuras (if o else) continuará ejecutando el
resto del programa. O bien se ejecuta la estructura if o bien se ejecuta la estructura else, pero siempre
ejecuta una de las dos de forma obligatoria.*

**Condición múltiple o condición anidada: (if-elif)**
*Esta estructura ejecutará las sentencias incluidas dentro de una estructura if si la condición1 es
verdadera, en caso de que sea falsa comprobará la condición2, si es verdadera ejecutará las sentencias
del elif, si es falsa la condición2 comprobará las siguientes condiciones y en caso de que alguna se
cumpla se ejecutarán sus sentencias, saldrá de la estructura y continuará ejecutando el resto del
programa.
Puede darse el caso que no se cumpla ninguna de las condiciones, si todas las condiciones son falsas,
no ejecutará ninguna de ellas, tal y como sucedía con la estructura condicional simple (if). Si queremos
evitar este problema podemos incluir al final una sentencia else para el caso o los casos en los que no
se cumplan ninguna de las condiciones anteriores.
Se pueden incluir todas las estructuras elif que se consideren oportunas. No hay un límite numérico de
las que se pueden utilizar.*

**ESTRUCTURAS REPETITIVAS O BUCLES.**

Son estructuras cuya ejecución se repite mientras se cumpla una determinada condición. La diferencia con
respecto a las estructuras condicionales (if) anteriores es que la estructura condicional únicamente se ejecuta
una vez, es decir, ejecuta lo que se incluye dentro de la estructura if una única vez si se cumple la condición, sale
del if y continúa con el resto del programa. En cambio, una estructura repetitiva ejecutará lo que se incluye
dentro de esa estructura de repetición mientras se cumpla la condición, mientras la condición siga siendo
verdadera.
En el momento en que la condición deja de cumplirse, es falsa, el bucle o la ejecución de esa estructura finaliza y
continúa ejecutando el resto del programa.
Es importante tener en cuenta que la condición en algún momento de la ejecución debe ser falsa y no debe
cumplirse para que la ejecución finalice, en caso contrario, nunca finalizará la ejecución y tendremos lo que se
denomina un bucle infinito.
Dentro de las estructuras de repetición tenemos 2 tipos en Python:

**Estructura de repetición con condición inicial: (while)**

+ Estructura en la que se evalúa la condición al principio o inicio de la estructura. Si se cumple la condición
entrará dentro de esa estructura y lo ejecutará mientras que la condición sea verdadera. Si no se cumple la
condición de inicio no entrará dentro de esa estructura, por tanto, existe la posibilidad que nunca se ejecuten
las sentencias que hay dentro de la estructura while y continuará ejecutando el resto del programa.
Esta estructura se utiliza cuando antes de comenzar el bucle sabemos con seguridad el valor de la variable
que se indica en la condición, bien porque la variable de la condición se inicializa justo antes del bucle (caso
A), bien porque el valor de la variable de la condición se ha pedido al usuario mediante teclado antes del
bucle (caso B), bien porque antes del bucle hemos realizado un cálculo que nos asigna el valor a la variable de
la condición (caso C). Para los tres casos el valor de la variable se obtiene antes del bucle.

**Ejemplos:**
…
A)
a = 0
while (a &gt; 0): No se cumple la condición. No ejecutará el interior del bucle
a = a + 2
print(a)

B)
a = 0
while (a &gt;= 0): Se cumple la condición. Ejecutará el interior del bucle.
a = a + 2 Siempre se cumplirá que a &gt;= 0. Bucle infinito
print(a) Mostrará los números pares: 2, 4, 6, 8, 10, 12, …

C)
a = 10;
while (a &gt;= 0): Se cumple la condición. Ejecutará el interior del bucle.
a = a - 2 Cuando a = 0 -2 = -2 ya no se cumple la condición, ejecución finalizará
print(a) Mostrará los números 8, 6, 4, 2, 0, -2

> Existe una variable de control que “controla” la ejecución del bucle, dentro de la estructura while se modifica esa
variable de control para que en algún momento la condición no se cumpla y la ejecución finalice. La variable de
control normalmente es la misma que la que está indicada en la condición del bucle.


**Estructura iterativa: (for)**

+ Estructura en la que se ejecutan una serie de sentencias incluidas dentro de la estructura for desde un valor
inicial hasta un valor final conocidos.
En esta estructura no tenemos variable de control dentro del bucle, sino que la propia estructura estructura
for realiza la modificación de la variable, dependiendo del rango indicado y los valores de este.

Dependiendo del número de valores indicados en el rango del bucle for, éste se comporta de diferente
forma:

1. Si indico únicamente un valor en el rango: Los valores serán desde 0 hasta el valor indicado en el
rango – 1, por tanto, si indico 11 se ejecutará desde 0 hasta el valor 10. Además, el incremento,
como tampoco se indica, será automáticamente de 1 en 1.

1. Si indico dos valores en el rango: Los valores serán desde el valor inicial hasta el valor final –
2, además, el incremento, que no se indica, será automáticamente de 1 en 1.
2. Si indico dos valores en el rango: Los valores serán desde el valor inicial hasta el valor final –
1, además, el incremento, que no se indica, será automáticamente de 1 en 1.
3. Si indico tres valores en el rango: Los valores serán desde el valor inicial hasta el valor final –
1, y se indica también el incremento.

> Si quiero comenzar desde 0 y que el incremento sea distinto de 1, por ejemplo 3, tengo que
ponerle 3 parámetros. No puedo omitir el 0 ya que si le pongo solo dos parametros Python
reconocerá la función únicamente como el anterior caso, es decir, con un inicio y un fin.

**Listas**

1. No están ordenadas, se inserta donde el programador desea que se realice: al final de la lista o en una
posición determinada de la lista.
2. Se pueden repetir sus elementos, permite duplicados.
3. Son indexadas, es decir, permite acceder a los elementos mediante el [i].
4. Se pueden anidar, es decir, añadir una lista dentro de otra lista  matriz.
5. Son mutables, sus elementos se pueden modificar, eliminar o intercambiar.
6. Son dinámicas, su tamaño crece o decrece automáticamente al insertar o al eliminar elementos.

Una lista en Python se define mediante los elementos encerrados entre []

+ lista1 = [] =&gt; lista vacía. Se representa con dos corchetes vacíos
+ lista2 = [1, 2, 3, 4] =&gt; lista con elementos, se declaran los elementos entre [] y separados por comas.
+ lista3 = [1, 2.8, ‘a’, ‘pepe’, [‘a’, ‘b’, ‘c’]] =&gt; lista con diferentes tipos de elemento.

**Metodos**
  	
| Metodos | Funcion | ejemplo |
| ----------- | ----------- | ------------ |
| len | Devuelve el tamaño o longitud de la lista | len(nombre de la lista) |
| count | Devuelve el número de veces que se encuentra el valor indicado en el parámetro dentro de la lista. | lista = [“pepe”, “antonio”, “luis”, “pepe”] lista.count(“pepe”) =&gt; 2 |
| append | Añade un elemento al final de la lista | lista = [1, 2, 3] lista.append(5) =&gt; [1, 2, 3, 5] |
| extend | Añade una lista al final de la lista actual | lista = [1, 2, 3]lista.extend([4, 5, 6]) =&gt; [1, 2, 3, 4, 5, 6] |
| Insert | Añade un elemento en un índice determinado. | lista = [1, 2, 3]lista.insert(1, 5) =&gt; [1, 2, 3] =&gt; [1, 5, 2, 3] |
| pop |Borrar un elemento de la lista. Si le indicamos posición como parámetro borrará el elemento situado en esa posición, si no le indicamos posición en el parámetro borrará el último elemento. | lista.pop(1) =&gt; [1, 2, 3]  |
| remove | Borrar el elemento pasado como parámetro de la lista. si le indicamos un elemento que noexiste en la lista, la aplicación dará un error indicando que ese elemento no está en lalista.| lista.remove(“Pepe”)=&gt[“Luis”,“Antonio”, “Pepe”, “Alfredo”] =&gt; [“Luis”, “Antonio”, “Alfredo”] |
| reverse | Invierte el orden de los elementos de la lista | lista = [1, 2, 3]lista.reverse() =&gt; [3, 2, 1] |
| sort |Ordena los elementos de la lista, en orden ascendente o descendente, dependiendo de un parámetro reverse que se le indica en el método sort. | lista.sort() =&gt; [1, 2, 3] |
| index | Devuelve la primera posición o índice donde se encuentra el elemento pasado como parámetro. | lista = [3, 1, 2] lista.index(2) =&gt; 2lista.index(3) =&gt; 0 |

**Tuplas**
Tipos o estructuras de datos que permiten almacenar un conjunto de elementos de forma muy parecida a las
listas, que, a diferencia de otros lenguajes, en Python sí permite que sean elementos de diferente tipo.

A continuacion para este apartado me gustaria dejar una explicacion muy completa de esta pagina web:

Esta todo perfectamente estructurado:

[Link_tuplas](https://www.w3schools.com/python/python_tuples.asp "Escuela")










