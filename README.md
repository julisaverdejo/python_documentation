# python_documentation

## Metodología Git-GitHub

1. `git clone https://github.com/julisaverdejo/python_documentation.git ` 
2. `git status`
3. `git add .`  
4. `git commit -m "descripcion" -m "extenso"`
5. `git push origin main` 

___

## Instalación python

Esta es la [página](https://www.python.org/) oficial para descargar python

Con el siguiente comando se puede checar la versión de python en el cmd.

```
python --version
```

Para poder ejecutar python en cmd, únicamente es necesario escribir python seguido del nombre del archivo. Ubicándonos en la carpeta que contiene nuestro código basta con borrar la ruta y escribir cmd en ese directorio para abrir una consola.

```
python a0_hola_mundo.py
```

 

---



## Sintaxis

**Tipos de datos**

| Tipo de dato   | Descripción                                                  | Ejemplo                  |
| -------------- | ------------------------------------------------------------ | ------------------------ |
| Integer        | Tipo de dato inmutable.                                      | `-1, -5, 0, 6`           |
| Booleano       | Tipo de dato inmutable solo tiene dos valores: True o False. | `True` `False`           |
| Floating point | Tipo de dato inmutable.                                      | `5.5, 3.8, 8.0`          |
| Strings        | Tipo de dato **inmutable**, se define por tener comillas simples. | `'hola', 'perro'`        |
| Lists          | Tipo de dato **mutable**, los valores de una lista están dentro de corchete. Posee índices por lo tanto sus valores siempre están ordenados. | `[25, 'de', 'junio']`    |
| Dictionaries   | Tipo de dato **mutable**, se define por almacenar sus valores en llaves. Los diccionarios tienen dos valores: key y value, esto hace que sus valores no estén ordenados. | `{'huevos':5,'ajo':'2'}` |
| Tuplas         | Tipo de dato **inmutable**, que se define por almacenar sus valores en paréntesis. Las tuplas también poseen índices. | `(25.5,'cat')`           |



**Operadores**

Los operadores son símbolos matemáticos con los que puedes hacer diversas operaciones. La tabla que se muestra a continuación indica la jerarquía de los operadores.

| Operador | Operación       | Ejemplo   | Resultado |
| -------- | --------------- | --------- | --------- |
| `**`     | Potencia        | `2 ** 3`  | `8`       |
| `%`      | Módulo/restante | `22 % 8`  | `6`       |
| `//`     | División entera | `22 // 8` | `2`       |
| `/`      | División        | `22 / 8`  | `2.75`    |
| `*`      | Multiplicación  | `3 * 5`   | `15`      |
| `-`      | Resta           | `5 - 2`   | `3`       |
| `+`      | Suma            | `2 + 2`   | `4`       |



**Operadores de asignación aumentada**

Estos operadores sirven de "atajo" en python para dejar de escribir la variable dos veces cada que hacemos una operación con ella.

| Operador | Ejemplo  | Equivalencia    |
| -------- | -------- | --------------- |
| +=       | spam +=1 | spam = spam + 1 |
| -=       | spam -=1 | spam = spam - 1 |
| *=       | spam *=1 | spam = spam * 1 |
| /=       | spam /=1 | spam = spam / 1 |
| %=       | spam %=1 | spam = spam % 1 |



**Operadores de comparación**

Los operadores de comparación devuelven valores booleanos: True o False.

| Operador | Operación                | Descripción  |
| -------- | ------------------------ | ------------ |
| ==       | Igual a                  | `a == b`     |
| !=       | Diferente a              | `a != b`     |
| <        | Menor que                | `a < b`      |
| >        | Mayor que                | `a > b`      |
| <=       | Menor o igual a          | `a <= b`     |
| >=       | Mayor o igual a          | `a >= b`     |
| is       | Identity                 | `a is b`     |
| is not   | Negated identity         | `a is not b` |
| in       | Containment test         | `a in b`     |
| not in   | Negated containment test | `a not in b` |



**Operadores booleanos**

Son operadores lógicos que comparan valores y determinan si el resultado es True o False.

La siguiente tabla está ordenada conforme a la prioridad que python le da a los operadores.

| Operador | Descripción                                                  |
| -------- | ------------------------------------------------------------ |
| `and`    | Devuelve un valor False cuando una de sus condiciones no se cumple. Si todas las condiciones se cumplen entonces devolverá un True. |
| `or`     | Siempre devolverá un True cuando al menos una de sus condiciones se cumpla. Si las condiciones no se cumplen entonces devolverá un False. |
| `not`    | Devuelve el operador inverso de una condición, si una condición es True entonces será False y viceversa. |

> Una cadena en blanco, los números 0 y 0.0 también son valores False, todos los demás son True.



## Variables

Una variable es como una caja en la memoria de tu computadora, esta caja solo puede almacenar un valor.

Para nombrar una variable debes tomar en cuenta lo siguiente

1. Puede usarse solo una palabra
2. Solo se pueden utilizar letras, números y guión bajo.
3. No puede empezar con un número.

```python
>>> spam = 40
>>> spam
40

>>> spam = 'Hello'		# Una variable se puede reescribir y olvidar
>>> spam + ' World'		# su antiguo valor
'Hello World'
```



## Funciones

Las funciones son miniprogramas dentro de tu programa y son muy importantes en Python. Supongamos que tienes un conjunto de instrucciones que debe ejecutarse varias veces en tu programa. En lugar de escribir esas instrucciones repetidamente, se puede usar una función para realizar esa acción.

Una función se escribe una sola vez pero puedes ejecutarla tantas veces como quieras en tu programa. El uso de funciones **evita las redundancias en tu código**. Puedes usar funciones integradas o **definirlas tú mismo**.

**Cómo definir una función**

Para definir una función en Python creada por ti debes seguir la sintaxis presentada a continuación:

```python
def function_name(parameter_1, parameter_2,..., parameter_n):
    statement(s)
```

1. Usar la palabra **def**

2. Escribir el **nombre de la función**. El nombre puede tener letras, números y guión bajo pero no puede empezar con un número.

3. **Argumentos** encerrados entre paréntesis y separados por comas. Algunas funciones no tienen argumentos.

4. Dos puntos

5. Bloque de código identado (`statement(s)`)

   

> Definir una función no significa que el programa la ejecute, solo la estamos nombrando y especificando que es lo que hace cuando esta sea llamada.

> Una función debe ser definida antes de ser llamada.



**Return values and return statements**

Al crear una función, puedes especificar qué valor devolverá con la sentencia **return**, esta consiste de lo siguiente:

1. La palabra return
2. El valor o expresión que la función devolverá

Si una función no cuenta con la sentencia return el valor por default que devuelve es **None** (es la ausencia de valor), a estas funciones se les llama **void functions**. 

> La función `print()` devuelve un valor None.



**Variables locales y globales**

En python existen dos tipos de entornos: *global* y *local*, los cuales tienen sus respectivas variables:

**Global** : Son aquellas que están definidas fuera de una función y estas son destruídas cuando el programa termina.

**Local** : Son todas las variables definidas dentro de una función. Una variable local es creada y destruída cada vez que una función es llamada y ningún código fuera de la función puede acceder a ella.

Existen algunas reglas que se deben aplicar al momento de definir las variables globales y locales:

1. Las variables locales no pueden usarse en un entorno global.
2. Entornos locales no pueden usar variables definidas en otros entornos locales.
3. Evita nombrar igual a variables locales y globales.
4. Las variables globales pueden usarse en entornos locales, si necesitas modificar una variable global desde dentro de una función, usa la declaración `global`.



**Manejo de errores con try/except**

Cuando tienes un error en tu código todo tu programa fallará, mandará un mensaje de error y la ejecución se detendrá, lo ideal sería que tu programa detecte el error y siga ejecutándose. Esto es posible usando las sentencias try y except.

Cuando el código dentro de una sentencia try tiene un error, el programa rápidamente salta a la sentencia except, después de esto la ejecución del código sigue igual.

> Las sentencias try y except pueden ser utilizadas en funciones.



**Ejemplo de función y sentencias try y except**

Supongamos que quieres hacer una función que divida el número 42 con cualquier número, el código se vería así:

```python
def divide(number):
    return 42 / number

print(divide(2))
print(divide(0))	#El programa marcará un error
print(divide(6))


#El programa devuelve lo siguiente
>>> print(divide(2))
21.0
>>> print(divide(0))
Traceback (most recent call last):
  File "<pyshell#4>", line 1, in <module>
    print(divide(0))
  File "<pyshell#2>", line 2, in divide
    return 42 / number
ZeroDivisionError: division by zero
```

El programa marcará un error ZeroDivisionError debido a que ningún número es divisible entre cero, pero podemos mejorar el código con try y except.

```python
def divide(number):
    try: 
    	return 42 / number
    except ZeroDivisionError:
        print('Argumento no válido')

print(divide(2))
print(divide(0))	
print(divide(6))
```

> No es necesario escribir el tipo de error en except, si no escribes el programa funciona igual.



**Funciones integradas en python**

| Función              | Descripción                                                  |
| -------------------- | ------------------------------------------------------------ |
| `print()`            | Muestra en la pantalla del valor dentro del paréntesis. Esta función tiene las palabras clave **end** y **sep**; con end puedes hacer que dos cadenas se impriman en la misma línea de código; con sep puedes separar varias cadenas con cualquier caracter. Con esta función también podemos unir cadenas que se encuentran en diferentes renglones`print('Te' + \ ' amo')`. En este caso ' amo' debería estar en otro renglón. |
| `input()`            | Esta función sirve para introducir valores.                  |
| `len()`              | Cuenta el número de caracteres en una cadena, lista, diccionario y tupla. |
| `str()`              | Convierte los tipos de dato int y float en cadena.           |
| `int()`              | Convierte los tipos de dato str y float en entero.           |
| `bool()`             | Convierte un int, string o float en booleano.                |
| `float()`            | Convierte un int o string en flotante.                       |
| `list()`             | Convierte un string, tuple o dictionary en una lista.        |
| `tuple()`            | Convierte un string, list o diccionary en una tupla.         |
| `range()`            | Genera una secuencia de números, esta función puede tener hasta tres argumentos, los cuales pueden ser números positivos o negativos. `range(n)`: Indica que la secuencia empieza en cero y termina en n-1; `range(n1, n2)`: Es parecido a `range(n)` pero la secuencia comienza en el número que desees; `range(n1, n2, step)`: Con `range(n)` y `range(n1,n2)` el step por default es 1, pero lo puedes modificar indicando cuantos pasos de separación habrá entre n~1~ y n~2~. |
| `sys.exit()`         | Termina un programa inmediatamente.                          |
| `copy()`             |                                                              |
| `paste()`            |                                                              |
| `sum()`              | Suma todos los elementos de un tipo de dato iterable, como list, tuple, diccionaries and set. |
| `sorted(<iterable>)` | Devuelve una lista ordenada de los elementos de un tipo de dato iterable (list, str, tuples, dictionary, sets). Esta función puede llegar a tener hasta tres argumentos. |
| `zip()`              | Devuelve una secuencia que agrega elementos de iterables (listas, strings o diccionarios). Si pasas dos iterables, uno que contiene dos elementos y otro que contiene cinco elementos, entonces la función `zip()` devuelve una secuencia de dos tuplas. Con un único argumento iterable, devuelve un iterador de una tupla. Sin argumentos, devuelve un iterador vacío. Esta función puedes usarla para relacionar iterables en un ciclo for. |



## Flow control statements

El corazón de la programación se encuentra en las sentencias de control, Python (al igual que otros lenguajes de programación), tiene un conjunto de sentencias que permiten que tu programa pueda omitir instrucciones, repetirlas o elegir una de varias instrucciones para ejecutar.

Las sentencias de control que ofrece Python son:

1. **Sentencias secuenciales** : Son las sentencias que se ejecutan dependiendo del orden en que aparecen en el programa.
2. **Sentencias de decisión** : Son aquellas que dependen de una condición, si esta es True o False, el programa puede omitir la ejecución de un bloque o ejecutar un bloque en lugar de otro. **If**, **else** y **elif** pertenecen a estas sentencias.
3. **Sentencias cíclicas** : Estas estructuras de control ejecutan un bloque varias veces hasta que la condición del ciclo se cumpla. Los ciclos **for** y **while** son sentencias cíclicas.

**if**

La sentencia if ejecuta el código si la condición o expresión booleana es True, si es False entonces el programa no se ejecutará.

Un if en Python debe tener lo siguiente:

* La palabra if
* Una condición que sea True o False
* Dos puntos después de la condición
* Un bloque de código identado (llamada if clause)

```python
#Ejemplo de una sentencia if
print('What is your name?')
name = input()

if name == 'Julie':
    print('Hello ' + name)
```



**else**

La sentencia else puede ir seguida de un if cuando la condición de esta es False; *else no tiene condición* y en Python se define de la siguiente manera:

* La palabra clave else
* Dos puntos
* Un bloque de código identado (else clause)

```python
#Ejemplo de una sentencia else
print('What is your name?')
name = input()

if name == 'Julie':
    print('Hello ' + name)
else:
    print('Hello, stranger')
```



**elif**

Esta sentencia es útil cuando necesitas definir varias opciones posibles; elif puede ir seguido de un if o de un mismo elif; además es la abreviación de else if.

En Python elif se define como sigue:

* La palabra elif
* Una condición que tiene como valor True o False
* Dos puntos
* Un bloque de código identado (elif clause)

*Ejemplo* : Escribe un programa que te de una puntuación entre 0.0 y 1.0. Si la puntuación es cero o mayor a 1 imprime 'Calificación incorrecta'

| Score  | Grade |
| ------ | ----- |
| >= 0.9 | A     |
| >= 0.8 | B     |
| <= 0.7 | F     |

```python
score = float(input('Ingresa una puntuación: '))
if score <= 0 or score > 1:
    print('Calificación incorrecta')
elif score >= 0.9:
    print('A')
elif score >= 0.8:
    print('B')
else:
    print('F')
```



**x if C else y**

A veces llamado *operador ternario* tiene la prioridad más baja de todas las operaciones de python.

La expresión primero evalúa la condición **C** en lugar de **x**. Si **C** es **verdadero**, se evalúa **x** y se devuelve su valor, de lo contrario, se evalúa **y** y se devuelve su valor.

Es similar a un **if else** normal, pero el operador ternario tiene la ventaja de que se evalúa en una sola línea.

```python
number = 15
# if else normal
if number%2 == 0:
    print('par')
else:
    print('impar')
    
#Operador ternario
print('par' if (number%2 == 0) else 'impar')
```



**while**

Un ciclo while puede hacer que un bloque de código se *ejecute una y otra vez* (iteración) solo si la *condición es True*, cuando sea False el ciclo terminará. El ciclo while se define de la siguiente forma:

* La palabra while
* Una condición que devuelva un valor booleano
* Dos puntos
* Un bloque de código identado

*Ejemplo*: Realizar la suma de los números del 1 al 100

```python
total = 0
num = 0
i = 0
while i < 101:
    total = total + num
    num += 1
    i += 1
print(total)
```



**for**

Un ciclo for ejecuta un bloque de código *determinado número de veces* y esto lo puede hacer con la función `range()`.

En Python este ciclo se define así:

* La palabra for
* Una variable
* La palabra **in**
* Función `range()`
* Dos puntos
* Un bloque de código identado

> No necesariamente tienes que ocupar la función `range()`, en su lugar puedes usar una lista, tupla, cadena o diccionario.

*Ejemplo* : Realizar la suma de los números del 1 al 100

```python
total = 0
for i in range(101):	#La variable es i
    total = total + i

print(total)
```



**break y continue**

Estas sentencias sirven para controlar código dentro de un ciclo **while** o **for**.

**break** : Salta a la primera línea **fuera del ciclo**, siempre y cuando la condición del ciclo sea verdadera.

**continue** : Hace que el programa vaya inmediatamente al **inicio del ciclo** y **reevalúe** la condición.

```python
#Ejemplo de ciclo while con break y continue
#Este programa pregunta por tu nombre y contraseña
while True:
    print('Who are you?')
    name = input()
    if name != 'Julie':
        continue #Irá al inicio del ciclo si name!=Julie
    print('Hello, Julie. What is the password? (Name of your pet)')
    password = input()
    if password == 'blacki': #Irá al inicio de ciclo si la contraseña no es blacki
        break	#Cuando la contraseña es correcta entonces salimos del ciclo.
print('Access granted.')
```

```python
#Ejemplo de ciclo for con break:Programa que indica si un número es primo o no 
number = int(input('Enter a number > 1: '))
prime = True
for i in range(2,number):   #range(n,n) hará que el ciclo for no se ejecute
    if number % i == 0:
        prime = False
        break
if prime:
    print(str(number) + ' is a prime number')
else:
    print(str(number) + ' is not a prime number')
```

```python
#Ejemplo de ciclo for con continue
#Este programa identifica si hay una letra i en la cadena, si existe no la imprime
for val in 'string':
    if val == 'i':
        continue
    print(val)
```



## Referencias



## List

Una lista es un tipo de dato **mutable** que contiene múltiples valores en una secuencia ordenada, los valores de una lista se llaman items y se encuentran encerrados entre corchetes.

Para facilitar la lectura de una lista se pueden usar saltos de línea cuando hay muchos elementos o estructuras anidadas dentro de una lista.

```python
>>> flowers = [
    'rose'
    'sunflower'
    'tulip' 
]

>>> animals = [
    {'fish':'gold', 'monkey': 'brown'},
    ('mammal', 'bird')
    ['water', 'jungle']
]
```

Para acceder a los índices de una lista puede hacerse de izquierda a derecha, los índices serán números positivos y el primer elemento tendrá el índice **0**, pero si deseas acceder a los índices de derecha a izquierda los índices serán negativos y el último elemento tendrá el índice **-1**.

| left → right |   0    |   1    |   2    |   3    |   4    |   5    |                  |
| :----------: | :----: | :----: | :----: | :----: | :----: | :----: | :--------------: |
|              |   p    |   y    |   t    |   h    |   o    |   n    |                  |
|              | **-6** | **-5** | **-4** | **-3** | **-2** | **-1** | **right → left** |

**Operaciones con listas**

La mayoría de las operaciones que se muestran a continuación solo son posibles hacerlas si sabes el índice con el que deseas trabajar.

Supongamos que tenemos la siguiente lista

```python
>>> spam = [['cat', 'bat'],['rat', 'elephant'], [25, 5]]
```

| Operación             | Definición                                                   | Ejemplo                                                      |
| --------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Indexación            | Puedes acceder a cualquier valor de una lista. En caso de que una lista estuviera conformada de otras listas puedes acceder a cualquier lista y valor usando dos corchetes `spam[0][1]`. Los índices también pueden ser números negativos. | `spam[0]`                                                    |
| Concatenación         | Puedes concatenar listas con listas o con cadenas con el signo + | `'The ' + spam[0][-2] + ' is fat' = 'The cat is fat'`        |
| Replicación           | La replicación de listas se da con el signo * y un número, el número indica cuantas veces se replicará la lista. | `['X','Y']*3`                                                |
| Slicing               | Los slices son secciones que contienen más de un valor. Generalmente los slices tienen dos argumentos pero también pueden lucir así `[:n]` o así `[n:]`, el primero indica que el slice iniciará en 0 hasta n-1 y el segundo que iniciará desde n hasta el final de la lista. Si en algún momento te encuentras un slice así `[:]` significa que abarcará todos los valores de una lista. | `spam[:2]`                                                   |
| Eliminar valores      | Podemos eliminar valores de una lista usando la sentencia `del` | `del spam[0]  `                                              |
| Longitud de una lista | La longitud de una lista se hace usando la función `len()`   | `len(spam)`                                                  |
| Conversión a listas   | Puedes convertir cualquier un str, dictionary o tuple en una lista | `list('Hola')`                                               |
| in                    | Este operador se usa para saber si un valor está en una lista, el valor de retorno de este operador es True o False. | `'rat' in spam[1][0]`                                        |
| not in                | Este operador se usa para saber si un valor no está en una lista, el valor de retorno de este operador es True o False. | `'gato' not in spam[1][0]`                                   |
| Asignación múltiple   | Es un "atajo" que te permite asignar múltiples variables a una lista. | `cat = ['fat', 'black', 'loud']` `size, color, disposition = cat` |

**Métodos de una lista**

Un método es parecido a una función, después del nombre de la lista sigue un punto y después el método. El argumento de los métodos siempre serán valores nunca índices.

Supongamos que tenemos las siguientes listas:

```python
>>> bacon = ['Ciro', 'Yoye', 26, 'enero', 'Ciro']
>>> spam = [4, 0, -20, 33, 1, 7, 4, 55]
```

| Método                      | Definición                                                   | Ejemplo                     |
| --------------------------- | ------------------------------------------------------------ | --------------------------- |
| `index(<item>, start, end)` | Devuelve el índice de cierto valor en una lista. Si ingresas un valor que no esté dentro de la lista, python, enviará un mensaje de error. Si tienes valores repetidos en una lista, el método  `index()`, devolverá el índice del valor repetido que aparezca primero, pero también puedes especificar en que sección de la lista buscar el índice con `start` y `end`. | `bacon.index('Ciro', 1, 5)` |
| `append()`                  | Este método agrega un valor al final de la lista.            | `bacon.append('guapo')`     |
| `insert()`                  | Agrega un valor en cualquier posición de la lista. Este método consta de dos argumentos `insert(i,v)`, siendo `i` el índice (o posición) en la cual quieres que se agregue el nuevo valor y `v` es el valor que deseas ingresar en la lista. | `bacon.insert(1,'amor')`    |
| `remove()`                  | Este método quita un valor de la lista. Si un valor se encuentra repetido solo se quitará el valor que aparezca primero. | `bacon.remove(26)`          |
| `sort()`                    | Ordena valores de menor a mayor, también de mayor a menor para esto debes usar `nombredelalista.sort(reverse=True)`y alfabéticamente, pero este método ordena primero las mayúsculas y después las minúsculas si quieres que `sort()` ordene los valores de la forma tradicional debes usar lo siguiente `nombredelalista.sort(key = str.lower)`. En caso de que no quieras mutar la lista original puedes usar la función `sorted(<iterable>)` y esta te devolverá una copia de la lista ordenada. | `spam.sort()`               |
| `extend(item)`              | Combina listas con otros tipos de datos con elementos iterables como set, tuple, str o list. Los elementos son transformados a listas y son anexados a la lista de forma ordenada. | `bacon.extend(spam)`        |
| `pop(<index>)`              | Toma un index, elimina el item de la lista y lo devuelve, si el index no es ingresado, entonces el método eliminará el último elemento de la lista. | `bacon.pop(-1)`             |
| `clear()`                   | Elimina todos los elementos de una lista, a este método no se le ingresan argumentos. | `bacon.clear()`             |
| `reverse()`                 | Invierte los elementos de una lista.                         | `spam.reverse()`            |
| `count(<item>)`             | Devuelve el número de veces que aparece un item en una lista. | `spam.count(4)`             |

> Los métodos append, insert, remove y sort solo son válidos para las listas, además nunca se asignan a una variable porque el valor de retorno de estos métodos es None.

> El método sort no ordena listas que tengan dos tipos de datos, por ejemplo: int y strings.



**Ciclo for en listas**

```python
#Este código funciona para cualquier lista sin importar cuantos valores tenga
>>> supplies = ['pens', 'staplers', 'flame-throwers', 'binders']
>>> for i in range(len(supplies)):
	print('Index ' + str(i) + ' in supplies is: ' + supplies[i])

	
Index 0 in supplies is: pens
Index 1 in supplies is: rulers
Index 2 in supplies is: eraser
Index 3 in supplies is: sharpener
```



## Tuple

Una tupla es un tipo de dato inmutable y ordenado, los valores de las tuplas van dentro de paréntesis y separados por comas.

+ Las tuplas pueden almacenar cualquier tipo de dato.
+ Las tuplas son iterables, por lo tanto puede emplearse el ciclo for y `enumerate(<tuple>)` 
+ Cualquier estructura de dato incluyendo las mismas tuplas pueden  anidarse en una tupla.
+ Si conviertes un `str` a `tuple` cada caracter del `str` será un elemento en la tupla.

Los beneficios de usar una tupla son los siguientes

1. Es una **secuencia ordenada de valores que nunca cambia**.
2. Python **ejecuta el código más rápido** con tuplas debido a que estas son inmutables
3. Indican a cualquier persona que lea tu código que no tienes intención de cambiar cierta secuencia de valores.



**Operaciones con tuplas**

```python
>>>	tupla = (5,2,1,4,6,3)
```

| Operación       | Definición                                                   | Ejemplo                |
| --------------- | ------------------------------------------------------------ | ---------------------- |
| `len()`         | Esta función devuelve el número de elementos en una tupla.   | `len(tupla)`           |
| `sum()`         | La función devuelve la suma de números en una tupla.         | `sum(tupla)`           |
| `sorted()`      | Devuelve una copia ordenada de la tupla como una lista mientras deja intacta la tupla original. | `sorted(tupla)`        |
| `in` / `not in` | Estos operadores indican si un item es parte de una tupla o no. | `9 in tupla`           |
| Concatenación   | Es la "suma" de tuplas. La concatenación se realiza con el signo `+` | `tupla + ('numbers',)` |
| Replicación     | La replicación de tuplas se da con el signo `* `y un número, el número indica cuantas veces se replicará la tupla. | `tupla * 2`            |
| Slicing         | Los slices son secciones que contienen más de un valor. Generalmente los slices tienen dos argumentos pero también pueden lucir así `[:n]` o así `[n:]`, el primero indica que el slice iniciará en 0 hasta n-1 y el segundo que iniciará desde n hasta el final de la lista. Si en algún momento te encuentras un slice así `[:]` significa que abarcará todos los valores de una tupla. | `tupla[0::2]`          |



**Métodos de tuplas**

| Método    | Sintaxis                 | Descripción                                                  |
| --------- | ------------------------ | ------------------------------------------------------------ |
| `count()` | `tuple_name.count(item)` | Devuelve el número de veces que un item aparece en la tupla. |
| `index()` | `tuple_name.index(item)` | Devuelve el índice del item en la tupla. Si el item aparece más de una vez, devolverá el índice del item que aparezca primero. Si el item no se encuentra en la tupla, entonces tendrás un *ValueError*. |



## Dictionary

Un diccionario es un tipo de dato mutable, es una colección de muchos valores encerrados en llaves. A diferencia de las listas, los **índices** de los diccionarios pueden ser **diferentes tipos de datos**, no solo enteros.

Los índices de los diccionarios se llaman keys y una key con su valor asociado se llama key-value pair. Los key y sus valores se separan con dos puntos.

Ejemplo de un diccionario

```python
myCat = {'size':'fat', 'color', 'gray', 'disposition':'loud'}
```

Las key son `'size'`,  `'color'` y `'disposition'`

Mientras que en las listas el orden de los valores es importante, en los diccionarios el orden no es relevante, por lo tanto los diccionarios no pueden tener **slices**.

```python
>>> spam = ['cat', 'dog', 'moose']
>>> bacon = ['dog', 'moose', 'cat']
>>> spam == bacon
False
```

```python
eggs = {'name':'Zophie', 'species':'cat', 'age': '8'}
ham = {'species':'cat', 'age':'8', 'name':'Zophie'}
eggs == ham
True
```

> Aunque los diccionarios no están ordenados, el hecho de que pueda tener valores arbitrarios para las keys le permite organizar sus datos de formas poderosas.

Los operadores **in** y **not in** verifican si una key está o no en un diccionario.

```python
>>> 'color' in eggs
False
>>> 'age' not in eggs
False
```

Si intentas acceder sin los operadores in y not in a un key que no existe tendrás un KeyError.

```python
>>> eggs = {'name':'Zophie', 'species':'cat', 'age': '8'}
>>> eggs['color']
Traceback (most recent call last):
  File "<pyshell#4>", line 1, in <module>
    eggs['color']
KeyError: 'color'
```



**Métodos de diccionarios**

Supongamos que tenemos el siguiente diccionario

```python
cocina = {'manzana': 5, 'plátano': 1, 'kg de frijol': 100, 'rebanadas de pan': 6}
```

| Método         | Definición                                                   | Sintaxis                                       |
| -------------- | ------------------------------------------------------------ | ---------------------------------------------- |
| `keys()`       | Este método devuelve un tipo de dato dict con todas las keys de tu diccionario. | `cocina.keys()`                                |
| `values()`     | Devuelve un tipo de dato dict con todos los valores de tu diccionario | `cocina.values()`                              |
| `items()`      | Devuelve un tipo de dato dict que contiene todos los key-value pairs en tuplas. Estas tuplas tienen dos valores cada una. | `cocina.items()`                               |
| `get()`        | Este método devuelve un valor asociado con la key especificada en el diccionario. Consta de dos argumentos `(key, default)`, si la key que ingresaste no existe en el diccionario entonces `get()` devuelve el valor `default` (puede ser cualquier tipo de dato). Si no proporcionaste ningún valor `default`entonces el método regresará un tipo de valor None, de modo que este método nunca generará un **KeyError**. | `cocina.get('kiwi', 'No tienes en la cocina')` |
| `setdefault()` | Este método ingresa una key y un value a tu diccionario, solo si esta key no existe, en caso de que la key ya existiera el método devolverá el valor de la key original. | `cocina.setdefault('pera', '3')`               |
| `pop(<key>)`   | Elimina el par key-value y devuelve value. Si ingresamos una key que no esté en el diccionario tendremos un KeyError, para evitar ese error podemos ingresar un segundo argumento, `default`, `pop()` devolverá el valor `default`. | `cocina.pop('kiwi', 'Unknown')`                |

> Los tipos de datos dict no pueden manejarse con facilidad por lo tanto es mejor convertirlos a listas. `list(cocina.keys())`

Los métodos `keys()`, `values()` e `items()` pueden utilizarse en ciclos for.

```python
>>> cocina = {'manzana': 5, 'plátano': 1, 'kg de frijol': 100, 'rebanadas de pan': 6}
>>> for k,v in cocina.items():
	print(k,v)

	
manzana 5
plátano 1
kg de frijol 100
rebanadas de pan 6
```



**Pretty Printing**

Si importas el módulo `pprint` en tus programas. tendrás acceso a las funciones `pprint()` y `pformat()`, estas funciones imprimirán de forma elegante los valores de un diccionario.

`pprint.pprint()`: Es útil cuando el propio diccionarios contiene listas anidadas o diccionarios.

`pprint.pformat`: Devuelve el texto como un string en lugar de mostrarlo en la pantalla.



## Sets



**Operaciones matemáticas**

| Operación           | Símbolo | Sintaxis                                                     | Descripción                                                  |
| ------------------- | ------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| union               | `|`     | `<set>.union(other_iterables)`<br />`<set> | <other_set_1> | ... | <other_set_n>` | Esta operación devuelve un nuevo set con todos los elementos de set y other_iterables u other_sets. |
| difference          | `-`     | `<set>.difference(other_iterables)`<br />`<set> - <other_set_1> - ... - <other_set_n>` | Devuelve otro set con los elementos del set original que no estaban en other_iterables u other_sets. |
| intersection        | `&`     | `<set>.intersection(<other_iterables>)`<br />`<set> & <other_set_1> & ... & <other_set_n>` | Intersection regresa un nuevo set con todos los elementos en común del set original y other_iterables u other_sets. |
| symetric difference | `^`     | `<set>.symmetric_difference(<other_iterables>)`<br />`<set> ^ <other_set>` | Retorna un set que contiene elementos que están en set o en other_iterables u other_sets pero no en ambos. |



**Métodos**

| Método         | Símbolo | Sintaxis                                                     | Descripción                                                  |
| -------------- | ------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `issubset()`   | `<=`    | `<set>.issubset(other_collection)`<br />`<set> <= <other_set>` | Este método devuelve `True` si cada elemento de set está en other_collection u other_set. |
| `issuperset()` | `>=`    | `<set>.issuperset(other_collection)`<br />`<set> >= <other_set>` | Es usado para verificar si cada elemento de other_collection u other_set se encuentra en set y devuelve `True` en caso de que sea cierto. |
| `isdisjoint()` |         | `<set>.isdisjoint(other_collection)`                         | Este método se usa para comprobar que set **no tiene elementos en común** con other_collection. El método acepta cualquier tipo de dato iterable o set como argumento. El método devuelve `True` si no tienen nada en común. |



## Strings

Una cadena es un tipo de dato inmutable y puede ser definida con comillas simples `''` o dobles `""`. Las cadenas multilíneas se definen con tres comillas simples `'''` o triples comillas dobles `"""`.

> Con cadenas multilíneas también podemos hacer comentarios en nuestro código.



**Escape characters**

Un caracter de escape te permite utilizar caracteres que serían imposibles usar en un string. Por ejemplo, si queremos escribir la siguiente string `'That is Alice's cat'`, python creerá que la cadena termina en `Alice`, para indicar que `'s cat` también forma parte de la cadena, usamos un backslash \ seguido de `Alice`.

```python
>>> 'That is Alice's cat'
SyntaxError: invalid syntax
    
>>> 'That is Alice\'s cat'
"That is Alice's cat"
```

Python tiene los siguientes caracteres de escape

| Escape character | Prints as            |
| ---------------- | -------------------- |
| `\'`             | Single quote         |
| `\"`             | Double quote         |
| `\t`             | Tab                  |
| `\n`             | Newline (line break) |
| `\\`             | Blackslash           |

> Tab, newline y blackslash funcionan si usas la función print.

```python
>>> print('Hola\ncomo\nestan?')
Hola
como
estan?
```

> raw strings son cadenas que ignoran todos los caracteres de escape, este tipo de cadenas llevan una r, `r'That is Carol\'s cat` →  `That is Carol\'s cat`



**Operaciones con cadenas**

```python
>>> name = 'Zophie'
```

| Operación     | Ejemplo            |
| ------------- | ------------------ |
| Concatenación | `'Julie' + 'Ciro'` |
| Replicación   | `'Julie' * 3`      |
| Indexación    | `name[0]`          |
| Slices        | `name[1:3]`        |
| in            | `'Zo' in name`     |
| not in        | `'p' not in name`  |



**Métodos de cadenas**

Todos los métodos de cadenas devuelven una nueva cadena, no modifican a la cadena original. Recordemos que una cadena es un tipo de dato inmutable.

Supongamos que tenemos la siguiente cadena

```python
>>> mensaje = '		el arte de amar por eric fromm		'
>>> mensaje_2 = 'ME ENCANTA EL CHOCOLATE'
>>> contraseña = 'CH0co14t325'
>>> numbers = '12345'
```

| Método                                          | Definición                                                   | Sintaxis                              |
| ----------------------------------------------- | ------------------------------------------------------------ | ------------------------------------- |
| `upper()`                                       | Devuelve una copia de la cadena con todas las letras en mayúsculas. | `mensaje.upper()`                     |
| `lower()`                                       | Devuelve una copia de la cadena con todas las letras en minúsculas. | `mensaje_2.lower()`                   |
| `isupper()`                                     | Devuelve `True` si todas las letras en una cadena son mayúsculas. | `mensaje_2.isupper()`                 |
| `islower()`                                     | Devuelve `True` si todas las letras en una cadena son minúsculas. | `mensaje_2.islower()`                 |
| `isalpha()`                                     | Devuelve `True` si la cadena consiste solo de letras y no tiene espacios en blanco. | `mensaje.isalpha()`                   |
| `isalnum()`                                     | Devuelve `True ` si la cadena consiste de números y letras y no tiene espacios en blanco. | `contraseña.isalnum()`                |
| `isdecimal()`                                   | Devuelve `True` si la cadena solo está compuesta de caracteres numéricos y no tiene espacios en blanco. | `numbers.isdecimal()`                 |
| `isspace()`                                     | Devuelve `True` si la cadena solo tiene espacios en blanco, tabs, nuevas lineas, si la cadena está en blanco devolverá `False`. | `'\t'.isspace()`                      |
| `istitle()`                                     | Devuelve `True` si todas las palabras de la cadena inician con mayúsculas, seguidas de minúsculas. | `mensaje_2.istitle()`                 |
| `startswith(<prefix>)`                          | Devuelve `True` si la cadena comienza con `<prefix>`.        | `mensaje_2.startswith('ME')`          |
| `endswith(<suffix>)`                            | Devuelve `True` si la cadena termina con `<suffix>`.         | `mensaje_2.endswith('CHOCOLATE')`     |
| `join()`                                        | Combina listas, tuplas, cadenas, sets o cualquier otra colección de cadenas con otra cadena y devuelve una nueva. Cualquier cadena puede ser utilizada para unir cadenas, incluso emojis. | `', '.join(['cats', 'rats', 'bats'])` |
| `split()`                                       | Devuelve una lista de strings separadas (sin ingresar argumentos).  Este método también sirve para eliminar elementos de las cadenas; `split()[<index>]` eliminará un valor en la cadena y `split('value')` eliminará todos los value que aparezcan en la cadena. | `mensaje_2.split()`                   |
| `rjust(s, caracter)`                            | Justifica (agrega espacios) una cadena hacia la derecha; la justificará `s - len(string)` espacios. Este método puede tener un segundo argumento, con este argumento podemos rellenar los espacios de la cadena con algún caracter u otra cadena. | `hello.rjust(10, '*')`                |
| `ljust()`                                       | Justifica una cadena hacia la izquierda, este método también puede tener dos argumentos. | `hello.ljust(10,'-')`                 |
| `center()`                                      | Justifica una cadena hacia el centro y agrega espacios tanto a la derecha como a la izquierda. También puede tener dos argumentos. | `hello.center(20,'=')`                |
| `strip()`                                       | Elimina elementos de los extremos de una cadena; `strip()` devuelve una cadena sin espacios en blanco al principio y al final de la cadena. | `mensaje.strip()`                     |
| `rstrip()`                                      | Elimina espacios en blanco que se encuentren a la derecha de la cadena. | `mensaje.rstrip()`                    |
| `lstrip()`                                      | Elimina espacios en blanco que se encuentren a la izquierda de la cadena. | `mensaje.lstrip()`                    |
| `title()`                                       | Cambia a mayúscula el primer caracter de cada palabra encontrada. | `mensaje.title()`                     |
| `replace(<substring>, <replacement substring>)` | Toma un substring y lo reemplaza con replacement substring.  | `'salt&pepper'.replace('&', ' & ')`   |



> Nota 1

Los métodos isX son muy útiles al momentos de validar la entrada del usuario.

```python
while True:
 print('Enter your age:')
 age = input()
 if age.isdecimal():
     break
 print('Please enter a number for your age')
```

> Nota 2

Los métodos `ljust()`, `rjust()` y `center()` son útiles cuando quieres imprimir datos de manera tabular.

```python
def printPicnic(itemsDict, leftWidth, rightWidth):
	print('PICNIC ITEMS'.center(leftWidth + rightWidth, '-'))
	for k, v in itemsDict.items():
		print(k.ljust(leftWidth, '.') + str(v).rjust(rightWidth))

picnicItems = {'sandwiches': 4, 'apples': 12, 'cups': 4, 'cookies': 8000}
printPicnic(picnicItems, 12, 5)


---PICNIC ITEMS--
sandwiches.. 4
apples...... 12
cups........ 4
cookies..... 8000
>>>
```



**String formatting**

Con los caracteres **%s** puedes crear cadenas. Más específicamente, **%s** convierte un valor especificado en una cadena usando la función `str()`.

```python
>>> name = 'Alice'
>>> place = 'Main Street'
>>> time = '6 pm'
>>> food = 'turnips'
>>> 'Hello %s, you are invite to a party at %s at %s. Please bring %s.'%(name,place,time,food)
'Hello Alice, you are invite to a party at Main Street at 6 pm. Please bring turnips.'
```

> Usar %s hace más fácil la concatenación de strings.







## Importar módulos a python

## Códigos

```python
```





## PEP8

* Una tabulación debe tener cuatro espacios.



