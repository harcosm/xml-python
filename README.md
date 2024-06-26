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

**Diccionarios**

Un diccionario es una estructura de datos donde cada elemento está formado por un par de valores clave y valor.
La clave de un diccionario es única y no se puede repetir, el valor para esa clave puede ser un tipo básico
(enteros, decimales, cadenas de texto) o un tipo compuesto (lista, otro diccionario)

1. Son dinámicos: crecen o decrecen, se pueden añadir y eliminar elementos.
2. Son idexados: los elementos de un diccionario se pueden acceder a través de la clave.
3. Son anidados: un diccionario puede contener a otro diccionario en su campo value.

![Alt](https://www.bigbaydata.com/wp-content/uploads/2022/07/diccionarios-en-python.webp)

_METODOS PARA EL MANEJO DE DICCIONARIOS DE PYTHON_


+ len: Devuelve el número de elementos que tiene el diccionario.
+ clear: Eliminar todo el contenido del diccionario.
+ get(clave [, valor_defecto]): Devuelve el valor para la clave indicada dentro del parámetro. El valor por
defecto es opcional, en caso de indicarlo es el valor que devolverá si no encuentre la clave dentro del
diccionario. Si no encuentra la clave y no se le ha indicado valor por defecto, devolverá el objeto vacío
None.
+ items: Devuelve una lista con las claves y los valores del diccionario, cada elemento de esta lista será
una tupla donde el primer elemento es la clave y el segundo elemento es el valor.
+ keys: Devuelve una lista con las claves del diccionario.
+ values: Devuelve una lista con los valores del diccionario.
+ copy: Realiza una copia del diccionario en otra dirección de memoria, para que los cambios en uno de
los diccionarios no afecten al diccionario copiado. En caso de realizar únicamente una asignación entre
diccionarios con el operador = estamos asignando la misma posición de memoria para ambos objetos,
por tanto, cualquier cambio en uno de ellos se verá reflejado en el otro.
+ pop(clave [, valor_defecto]): Busca y elimina la clave que se le pasa por parámetro, devuelve el valor
asociado para esa clave antes de eliminarlo, en caso que no encuentre la clave a eliminar devuelve el
valor por defecto. En caso que no se indique el valor por defecto y no exista la variable , la función pop
devuelve una Excepción KeyError.


### XML: ###
> XML, o Extensible Markup Language, es un lenguaje de marcado diseñado para describir datos de manera estructurada. A diferencia de HTML, que está diseñado para mostrar información y contenido en la web, XML se enfoca en describir los datos en sí mismos. Fue creado para ser legible tanto por humanos como por máquinas, y su flexibilidad lo hace adecuado para una amplia gama de aplicaciones.

**Elementos Basicos de xml**

+ Elementos: Los datos en XML están organizados en elementos. Un elemento XML comienza con una etiqueta de apertura, contiene los datos, y termina con una etiqueta de cierre. Por ejemplo: <nombre>Juan</nombre>.
+ Atributos: Los elementos pueden tener atributos que proporcionan información adicional sobre el elemento. Por ejemplo: <persona id="123">.
+ Comentarios: Se pueden incluir comentarios en XML usando la sintaxis <!-- comentario -->.
+ Procesamiento de Instrucciones: Se pueden incluir instrucciones de procesamiento XML, que son instrucciones para aplicaciones que procesan el documento XML.


**Estructura Jerarquica:**

  <libro>
  <titulo>El Gran Gatsby</titulo>
  <autor>F. Scott Fitzgerald</autor>
</libro>

Documento XML Bien Formado y Válido:

Documento XML Bien Formado: Un documento XML bien formado sigue todas las reglas de sintaxis de XML.
Documento XML Válido: Además de ser bien formado, un documento XML válido sigue una estructura definida por un esquema XML (como un documento DTD o un esquema XML).

**Aqui os dejo una fuente de información:**

![Tutorial_xml] https://www.w3schools.com/xml/)

**DTD:**
> DTD (Document Type Definition) es una especificación formal que define la estructura, el tipo de datos y las restricciones de un documento XML. En otras palabras, un DTD describe la gramática o la estructura de un documento XML. Se utiliza para validar documentos XML y garantizar que cumplan con ciertas reglas o estándares específicos.

+ 1. Definición de Elementos y Atributos:

En un DTD, se pueden definir los elementos que pueden aparecer en el documento XML, así como los atributos que pueden tener esos elementos.
Se especifica qué elementos pueden contener otros elementos, el orden en que deben aparecer y qué atributos son permitidos para cada elemento.

+ 2. Tipos de Datos:

Los DTD pueden definir tipos de datos para los valores de los atributos y elementos.
Los tipos de datos comunes incluyen cadenas de texto, números enteros, números decimales, fechas, etc.

+ 3. Entidades:

_Las entidades en un DTD son símbolos que representan valores de texto o fragmentos de XML.
Se pueden usar para definir valores comunes que se utilizan en múltiples lugares dentro del documento XML, lo que facilita la reutilización y la mantenibilidad del código._

+ 4. Validación:

_Un DTD se utiliza para validar documentos XML para asegurarse de que cumplan con las reglas especificadas en la definición.
La validación puede realizarse durante el proceso de análisis (parsing) del documento XML para detectar errores estructurales o semánticos._

+ 5. Integración con XML:

_Un DTD se puede incluir dentro de un documento XML usando la declaración DOCTYPE.
La declaración DOCTYPE especifica la ubicación del DTD que define la estructura del documento XML._

**Ejemplo dtd**


![image](https://github.com/harcosm/xml-python/assets/130600270/c1587c79-be16-4e82-88ee-0a21725590ad)


**Aqui os dejo un Tutorial con mas profundidad del temario de DTD**


![Tutorial_xml] https://www.w3schools.com/xml/xml_dtd_intro.asp)

**XSD:**

> XSD (XML Schema Definition), también conocido como XML Schema, es un lenguaje de definición de esquemas XML que se utiliza para describir la estructura y las restricciones de un documento XML de una manera más poderosa y flexible que los DTD (Document Type Definitions). Al igual que los DTD, los esquemas XML son utilizados para validar documentos XML y garantizar su conformidad con una estructura y semántica específicas.


_ XSD (XML Schema Definition), también conocido como XML Schema, es un lenguaje de definición de esquemas XML que se utiliza para describir la estructura y las restricciones de un documento XML de una manera más poderosa y flexible que los DTD (Document Type Definitions). Al igual que los DTD, los esquemas XML son utilizados para validar documentos XML y garantizar su conformidad con una estructura y semántica específicas. _

> Aquí hay algunos aspectos importantes sobre XSD:

1. Definición de Estructuras:

+ XSD permite definir estructuras complejas para los elementos XML, incluyendo la composición de elementos anidados y la especificación de tipos de datos para los elementos y atributos.

2. Tipos de Datos:

+ A diferencia de los DTD, XSD ofrece un conjunto más amplio de tipos de datos, como cadenas de texto, números enteros, decimales, fechas, booleanos, entre otros.
También permite la definición de tipos de datos complejos y derivados, como tipos enumerados, tipos de listas y tipos de uniones.

3. Restricciones y Validación:

+XSD permite establecer restricciones sobre los valores de los elementos y atributos, como rangos numéricos, expresiones regulares para cadenas de texto, entre otros.
Los documentos XML que siguen un esquema XML pueden ser validados contra ese esquema para garantizar su conformidad con las reglas especificadas.

4. Reutilización:

+ XSD facilita la reutilización de componentes y la modularidad a través de la definición de elementos y tipos complejos que pueden ser referenciados desde múltiples documentos XML.
Los esquemas XML pueden ser importados y extendidos para permitir la construcción de esquemas más grandes y complejos.

5. Espacios de Nombres:

+ XSD soporta la especificación de espacios de nombres XML, lo que permite evitar conflictos de nombres entre diferentes partes de un documento XML o entre documentos XML relacionados.

  **Ejemplo XSD:**

  ![image](https://github.com/harcosm/xml-python/assets/130600270/155e6a4a-2696-4034-adff-930d44a8e698)

  **Aqui os dejo un Tutorial con mas profundidad del temario de DTD**

![Tutorial_xml] https://www.w3schools.com/xml/schema_intro.asp)



| Característica              | XML                       | DTD                             | XSD (XML Schema)               |
|-----------------------------|---------------------------|---------------------------------|--------------------------------|
| Definición de estructuras   | Sí                        | Limitada                        | Sí                             |
| Tipos de datos              | Limitados                 | Básicos                         | Amplia gama                    |
| Restricciones y validación  | No                        | Básica                          | Compleja                       |
| Reutilización               | No                        | Limitada                        | Sí                             |
| Espacios de nombres         | No                        | Limitada                        | Sí                             |
| Legibilidad                 | Sí                        | Sí                              | Sí                             |
| Extensibilidad              | Sí                        | No                              | Sí                             |
| Soporte                     | Amplio                    | Limitado                        | Amplio                         |


**DOM:**

> DOM (Document Object Model) es una interfaz de programación para documentos HTML, XML y XHTML. Define la estructura lógica de los documentos y la forma en que se accede y manipula un documento. En resumen, el DOM representa el documento como un árbol de objetos, donde cada nodo del árbol representa parte del documento, como elementos HTML, atributos, texto y otros tipos de nodos.






Al igual que HTML (HyperText Markup Language), XML utiliza etiquetas para definir la estructura y el significado de los datos dentro del documento. Sin embargo, a diferencia de HTML, que está diseñado específicamente para la presentación de contenido en la web, XML no tiene una estructura predefinida y puede utilizarse para describir cualquier tipo de información.

Las características clave de XML incluyen:

Flexibilidad: XML permite definir etiquetas personalizadas y estructurar los datos de la manera que sea necesaria para una aplicación específica.

Legibilidad: Los documentos XML están diseñados para ser legibles tanto para humanos como para máquinas. Las etiquetas descriptivas facilitan la comprensión del contenido.

Extensibilidad: XML es "extensible" en el sentido de que los usuarios pueden definir sus propias etiquetas y atributos según sus necesidades específicas.

Interoperabilidad: XML se utiliza ampliamente como un formato estándar para el intercambio de datos entre diferentes sistemas y plataformas.

Soporte multiplataforma: XML es independiente de la plataforma y del lenguaje de programación, lo que significa que puede ser utilizado en una variedad de entornos de desarrollo.

XML se utiliza en una amplia variedad de aplicaciones, incluyendo la representación de datos en la web (por ejemplo, en la configuración de servicios web), el intercambio de datos entre sistemas heterogéneos, el almacenamiento de configuraciones y metadatos, y mucho más.



1. ¿Qué es XML?
XML, o Extensible Markup Language, es un lenguaje de marcado diseñado para describir datos de manera estructurada. A diferencia de HTML, que está diseñado para mostrar información y contenido en la web, XML se enfoca en describir los datos en sí mismos. Fue creado para ser legible tanto por humanos como por máquinas, y su flexibilidad lo hace adecuado para una amplia gama de aplicaciones.

2. Sintaxis Básica de XML:

Elementos: Los datos en XML están organizados en elementos. Un elemento XML comienza con una etiqueta de apertura, contiene los datos, y termina con una etiqueta de cierre. Por ejemplo: <nombre>Juan</nombre>.
Atributos: Los elementos pueden tener atributos que proporcionan información adicional sobre el elemento. Por ejemplo: <persona id="123">.
Comentarios: Se pueden incluir comentarios en XML usando la sintaxis <!-- comentario -->.
Procesamiento de Instrucciones: Se pueden incluir instrucciones de procesamiento XML, que son instrucciones para aplicaciones que procesan el documento XML.
3. Estructura Jerárquica:
XML organiza los datos en una estructura jerárquica de elementos anidados. Esto significa que los elementos pueden contener otros elementos, creando una estructura de árbol. Por ejemplo:


<libro>
  <titulo>El Gran Gatsby</titulo>
  <autor>F. Scott Fitzgerald</autor>
</libro>
Aquí, el elemento <libro> contiene los elementos <titulo> y <autor>.

4. Espacios de Nombres (Namespaces):
Los espacios de nombres permiten evitar conflictos de nombres al definir etiquetas. Esto es útil cuando se integran documentos XML de diferentes fuentes. Los espacios de nombres se definen usando la sintaxis xmlns. Por ejemplo: <documento xmlns:ejemplo="http://www.ejemplo.com">.

5. Documento XML Bien Formado y Válido:

Documento XML Bien Formado: Un documento XML bien formado sigue todas las reglas de sintaxis de XML, como tener una única raíz, etiquetas correctamente anidadas, y etiquetas cerradas correctamente.
Documento XML Válido: Además de ser bien formado, un documento XML válido sigue una estructura definida por un esquema XML (como un documento DTD o un esquema XML).
6. Aplicaciones de XML:
XML se utiliza en una variedad de aplicaciones, incluyendo intercambio de datos entre sistemas, configuración de servicios web, almacenamiento de configuraciones y metadatos, entre otros. Su flexibilidad y legibilidad lo hacen adecuado para una amplia gama de casos de uso.

En resumen, XML es un lenguaje de marcado diseñado para describir datos de manera estructurada, legible tanto por humanos como por máquinas. Su flexibilidad y capacidad para representar una amplia variedad de datos lo hacen ampliamente utilizado en el desarrollo de software y la integración de sistemas.



Características Principales:

Flexibilidad: XML es un lenguaje extensible, lo que significa que permite a los usuarios definir sus propias etiquetas y estructuras de datos según sea necesario para una aplicación particular.

Legibilidad: Los documentos XML están diseñados para ser legibles tanto por humanos como por máquinas. Las etiquetas descriptivas y la estructura jerárquica facilitan la comprensión del contenido.

Extensibilidad: XML permite la creación de vocabularios específicos de dominio mediante la definición de etiquetas personalizadas y la especificación de reglas para su uso.

Interoperabilidad: XML se utiliza ampliamente como un formato estándar para el intercambio de datos entre diferentes sistemas y plataformas. Su uso generalizado facilita la comunicación entre aplicaciones heterogéneas.

Independencia de Plataforma: XML es independiente de la plataforma y del lenguaje de programación, lo que significa que puede ser utilizado en una variedad de entornos de desarrollo.

Sintaxis Básica de XML:

Elementos: Los datos en XML se organizan en elementos, que consisten en una etiqueta de apertura, datos y una etiqueta de cierre. Por ejemplo: <nombre>Juan</nombre>.
Atributos: Los elementos pueden tener atributos que proporcionan información adicional sobre el elemento. Por ejemplo: <persona id="123">.
Comentarios: Los comentarios en XML se insertan entre <!-- y -->.
Procesamiento de Instrucciones: Se pueden incluir instrucciones de procesamiento XML, que son instrucciones para aplicaciones que procesan el documento XML.
Estructura Jerárquica:

Los datos en XML se organizan en una estructura jerárquica de elementos anidados, creando una representación de árbol. Por ejemplo:


<libro>
  <titulo>El Gran Gatsby</titulo>
  <autor>F. Scott Fitzgerald</autor>
</libro>
Aquí, el elemento <libro> contiene los elementos <titulo> y <autor>.

Espacios de Nombres (Namespaces):

Los espacios de nombres permiten evitar conflictos de nombres al definir etiquetas. Se definen usando la sintaxis xmlns. Por ejemplo: <documento xmlns:ejemplo="http://www.ejemplo.com">.

Documento XML Bien Formado y Válido:

Documento XML Bien Formado: Un documento XML bien formado sigue todas las reglas de sintaxis de XML.
Documento XML Válido: Además de ser bien formado, un documento XML válido sigue una estructura definida por un esquema XML (como un documento DTD o un esquema XML).
Aplicaciones de XML:

XML se utiliza en una variedad de aplicaciones, incluyendo intercambio de datos entre sistemas, configuración de servicios web, almacenamiento de configuraciones y metadatos, entre otros. Su flexibilidad y legibilidad lo hacen adecuado para una amplia gama de casos de uso.



Aquí hay algunos aspectos importantes sobre los DTD:

1. Definición de Elementos y Atributos:

En un DTD, se pueden definir los elementos que pueden aparecer en el documento XML, así como los atributos que pueden tener esos elementos.
Se especifica qué elementos pueden contener otros elementos, el orden en que deben aparecer y qué atributos son permitidos para cada elemento.
2. Tipos de Datos:

Los DTD pueden definir tipos de datos para los valores de los atributos y elementos.
Los tipos de datos comunes incluyen cadenas de texto, números enteros, números decimales, fechas, etc.
3. Entidades:

Las entidades en un DTD son símbolos que representan valores de texto o fragmentos de XML.
Se pueden usar para definir valores comunes que se utilizan en múltiples lugares dentro del documento XML, lo que facilita la reutilización y la mantenibilidad del código.
4. Validación:

Un DTD se utiliza para validar documentos XML para asegurarse de que cumplan con las reglas especificadas en la definición.
La validación puede realizarse durante el proceso de análisis (parsing) del documento XML para detectar errores estructurales o semánticos.
5. Integración con XML:

Un DTD se puede incluir dentro de un documento XML usando la declaración DOCTYPE.
La declaración DOCTYPE especifica la ubicación del DTD que define la estructura del documento XML.
Ejemplo de DTD:


<!DOCTYPE libro [
  <!ELEMENT libro (titulo, autor, año)>
  <!ELEMENT titulo (#PCDATA)>
  <!ELEMENT autor (#PCDATA)>
  <!ELEMENT año (#PCDATA)>
]>

En este ejemplo, se define un DTD para un documento XML que representa información sobre libros. Se especifica que un libro debe contener elementos titulo, autor y año, donde #PCDATA indica datos de caracteres.

En resumen, un DTD proporciona una especificación formal para la estructura y el contenido de un documento XML, lo que permite la validación y garantiza la consistencia y la integridad de los datos.



Aquí hay algunos aspectos importantes sobre XSD:

1. Definición de Estructuras:

XSD permite definir estructuras complejas para los elementos XML, incluyendo la composición de elementos anidados y la especificación de tipos de datos para los elementos y atributos.
2. Tipos de Datos:

A diferencia de los DTD, XSD ofrece un conjunto más amplio de tipos de datos, como cadenas de texto, números enteros, decimales, fechas, booleanos, entre otros.
También permite la definición de tipos de datos complejos y derivados, como tipos enumerados, tipos de listas y tipos de uniones.
3. Restricciones y Validación:

XSD permite establecer restricciones sobre los valores de los elementos y atributos, como rangos numéricos, expresiones regulares para cadenas de texto, entre otros.
Los documentos XML que siguen un esquema XML pueden ser validados contra ese esquema para garantizar su conformidad con las reglas especificadas.
4. Reutilización:

XSD facilita la reutilización de componentes y la modularidad a través de la definición de elementos y tipos complejos que pueden ser referenciados desde múltiples documentos XML.
Los esquemas XML pueden ser importados y extendidos para permitir la construcción de esquemas más grandes y complejos.
5. Espacios de Nombres:

XSD soporta la especificación de espacios de nombres XML, lo que permite evitar conflictos de nombres entre diferentes partes de un documento XML o entre documentos XML relacionados.
Ejemplo de XSD:


<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:element name="libro">
    <xs:complexType>
      <xs:sequence>
        <xs:element name="titulo" type="xs:string"/>
        <xs:element name="autor" type="xs:string"/>
        <xs:element name="año" type="xs:gYear"/>
      </xs:sequence>
    </xs:complexType>
  </xs:element>
</xs:schema>

En este ejemplo, se define un esquema XML utilizando XSD para validar documentos XML que representan información sobre libros. Se especifica que un libro debe contener elementos titulo, autor y año, y se establecen los tipos de datos para cada uno de estos elementos.


| Característica              | XML                       | DTD                             | XSD (XML Schema)               |
|-----------------------------|---------------------------|---------------------------------|--------------------------------|
| Definición de estructuras   | Sí                        | Limitada                        | Sí                             |
| Tipos de datos              | Limitados                 | Básicos                         | Amplia gama                    |
| Restricciones y validación  | No                        | Básica                          | Compleja                       |
| Reutilización               | No                        | Limitada                        | Sí                             |
| Espacios de nombres         | No                        | Limitada                        | Sí                             |
| Legibilidad                 | Sí                        | Sí                              | Sí                             |
| Extensibilidad              | Sí                        | No                              | Sí                             |
| Soporte                     | Amplio                    | Limitado                        | Amplio                         |

**DOM**

_ Características principales del DOM: _

1. Estructura en forma de árbol: El DOM organiza los elementos de un documento en una estructura jerárquica de árbol, donde cada nodo del árbol representa un elemento, atributo o texto del documento.

2. Acceso y manipulación: El DOM proporciona métodos para acceder y manipular los elementos del documento. Esto permite a los desarrolladores modificar dinámicamente el contenido, la estructura y los estilos de una página web utilizando JavaScript u otros lenguajes de programación.

3. Interfaz estandarizada: El DOM proporciona una interfaz de programación estandarizada que es independiente del lenguaje de programación utilizado. Esto permite a los desarrolladores acceder y manipular los documentos de manera consistente en diferentes entornos de desarrollo.

4. Representación de objetos: Cada nodo en el árbol DOM es un objeto, y los diferentes tipos de nodos (como elementos, atributos y texto) tienen sus propias interfaces y métodos asociados para acceder y manipular sus propiedades y contenido.

5. Eventos: El DOM también maneja eventos, como clics del mouse o cambios en los campos de entrada, permitiendo a los desarrolladores agregar interactividad a las páginas web.

















