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





