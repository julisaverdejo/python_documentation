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
| **       | Potencia        | `2 ** 3`  | `8`       |
| %        | Módulo/restante | `22 % 8`  | `6`       |
| //       | División entera | `22 // 8` | `2`       |
| /        | División        | `22 / 8`  | `2.75`    |
| *        | Multiplicación  | `3 * 5`   | `15`      |
| -        | Resta           | `5 - 2`   | `3`       |
| +        | Suma            | `2 + 2`   | `4`       |



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

| Operador | Significado     |
| -------- | --------------- |
| ==       | Igual a         |
| !=       | Diferente a     |
| <        | Menor que       |
| >        | Mayor que       |
| <=       | Menor o igual a |
| >=       | Mayor o igual a |



**Operadores booleanos**

Son operadores lógicos que comparan valores y determinan si el resultado es True o False.

La siguiente tabla está ordenada conforme a la prioridad que python le da a los operadores.

| Operador | Descripción                                                  |
| -------- | ------------------------------------------------------------ |
| and      | Devuelve un valor False cuando una de sus condiciones no se cumple. Si todas las condiciones se cumplen entonces devolverá un True. |
| or       | Siempre devolverá un True cuando al menos una de sus condiciones se cumpla. Si las condiciones no se cumplen entonces devolverá un False. |
| not      | Devuelve el operador inverso de una condición, si una condición es True entonces será False y viceversa. |

> Una cadena en blanco, los números 0 y 0.0 también son valores False, todos los demás son True.



**Funciones**

| Función      | Descripción                                                  |
| ------------ | ------------------------------------------------------------ |
| `print()`    | Muestra en la pantalla del valor dentro del paréntesis. Esta función tiene las palabras clave **end** y **sep**; con end puedes hacer que dos cadenas se impriman en la misma línea de código; con sep puedes separar varias cadenas con cualquier caracter. Con esta función también podemos unir cadenas que se encuentran en diferentes renglones`print('Te' + \ ' amo')`. En este caso ' amo' debería estar en otro renglón. |
| `input()`    | Esta función sirve para introducir valores.                  |
| `len()`      | Cuenta el número de caracteres en una cadena, lista, diccionario y tupla. |
| `str()`      | Convierte los tipos de dato int y float en cadena.           |
| `int()`      | Convierte los tipos de dato str y float en entero.           |
| `bool()`     | Convierte un int, string o float en booleano.                |
| `float()`    | Convierte un int o string en flotante.                       |
| `list()`     | Convierte un string, tuple o diccionary en una lista.        |
| `tuple()`    | Convierte un string, list o diccionary en una tupla.         |
| `range()`    | Genera una secuencia de números, esta función puede tener hasta tres argumentos. `range(n)`: indica que la secuencia empezará en cero pero no incluirá el número n, es decir n-1; `range(n1, n2)`: es parecido a `range(n)` solo que la secuencia puede comenzar en el número que desees pero termina en (n~2~-1); `range(n1, n2, step)`: el tercer argumento indica cuantos pasos de separación habrá entre n~1~ y n~2~, step también puede ser un número negativo. |
| `sys.exit()` | Termina un programa inmediatamente.                          |
| `copy()`     |                                                              |
| `paste()`    |                                                              |



## Definir una función

Agregar como se define una funcion

return values

none value

**Variables locales y globales**

**Manejo de errores con try/except**



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
#Uso de sentencias break y continue en ciclo while
while True:
    print('Who are you?')
    name = input()
    if name != 'Julie':
        continue #Irá al inicio del ciclo si name!=Julie
    print('Hello, Julie. What is the password? (Name of your pet)')
    password = input()
    if password == 'blacki': #Irá al inicio de ciclo si la 										 #contraseña no es blacki
        break				 #Cuando la contraseña es correcta 									 #entonces salimos del ciclo.
print('Access granted.')
```





## Listas

Una lista es un tipo de dato mutable que contiene múltiples valores en una secuencia ordenada, los valores de una lista se llaman items y se encuentran encerrados entre corchetes.

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
| Slices                | Los slices son secciones que contienen más de un valor. Generalmente los slices tienen dos argumentos pero también pueden lucir así `[:n]` o así `[n:]`, el primero indica que el slice iniciará en 0 hasta n-1 y el segundo que iniciará desde n hasta el final de la lista. Si en algún momento te encuentras un slice así `[:]` significa que abarcará todos los valores de una lista. | `spam[:2]`                                                   |
| Eliminar valores      | Podemos eliminar valores de una lista usando la sentencia `del` | `del spam[0]  `                                              |
| Longitud de una lista | La longitud de una lista se hace usando la función `len()`   | `len(spam)`                                                  |
| Conversión a listas   | Puedes convertir cualquier una cadena, diccionario o tupla en una lista | `list('Hola')`                                               |
| in                    | Este operador se usa para saber si un valor está en una lista, el valor de retorno de este operador es True o False. | `'rat' in spam[1][0]`                                        |
| not in                | Este operador se usa para saber si un valor no está en una lista, el valor de retorno de este operador es True o False. | `'gato' not in spam[1][0]`                                   |
| Asignación múltiple   | Es un "atajo" que te permite asignar múltiples variables a una lista. | `cat = ['fat', 'black', 'loud']` `size, color, disposition = cat` |

**Métodos de una lista**

Un método es parecido a una función, después del nombre de la lista sigue un punto y después el método. El argumento de los métodos siempre serán valores nunca índices (números).

Supongamos que tenemos las siguientes listas:

```python
>>> bacon = ['Ciro', 'Yoye', 26, 'enero']
>>> spam = [4, 0, -20, 33, 1, 7, 4, 55]
```

| Método     | Definición                                                   | Ejemplo                  |
| ---------- | ------------------------------------------------------------ | ------------------------ |
| `index()`  | Devuelve el índice de cierto valor en una lista. Si ingresas un valor que no esté dentro de la lista, python, enviará un mensaje de error. Si tienes valores repetidos en una lista, el método  `index()`, devolverá el índice del valor repetido que aparezca primero. | `bacon.index('Ciro')`    |
| `append()` | Este método agrega un valor al final de la lista.            | `bacon.append('guapo')`  |
| `insert()` | Agrega un valor en cualquier posición de la lista. Este método consta de dos argumentos `insert(i,v)`, siendo `i` el índice (o posición) en la cual quieres que se agregue el nuevo valor y `v` es el valor que deseas ingresar en la lista. | `bacon.insert(1,'amor')` |
| `remove()` | Este método quita un valor de la lista. Si un valor se encuentra repetido solo se quitará el valor que aparezca primero. | `bacon.remove(26)`       |
| `sort()`   | Ordena valores de menor a mayor, también de mayor a menor para esto debes usar `nombredelalista.sort(reverse=True)`y alfabéticamente, pero este método ordena primero las mayúsculas y después las minúsculas si quieres que `sort()` ordene los valores de la forma tradicional debes usar lo siguiente `nombredelalista.sort(key = str.lower)`. | `spam.sort()`            |

> Los métodos append e insert solo son válidos para las listas, además nunca se asignan a una variable porque el valor de retorno de estos métodos es None.

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



## Tuplas

Una tupla es un tipo de dato inmutable y ordenado, los valores de las tuplas van dentro de paréntesis.

Los beneficios de usar una tupla son los siguientes

1. Si necesitas una **secuencia ordenada de valores que nunca cambie** usa una tupla.
2. Python **ejecuta el código más rápido** con tuplas debido a que estas son inmutables
3. Indican a cualquier persona que lea tu código que no tienes intención de cambiar cierta secuencia de valores.

Algunas operaciones que puedes hacer con tuplas son:

```python
#Para acceder a un valor de una tupla se hace por medio de índices.
>>> diego = ('7', 'godzilla', '31 minutos')
>>> diego[0]
'7'

#Si quieres acceder a varios valores se hace por medio de slices
>>> diego[1:3]
('godzilla', '31 minutos')

#También puedes saber cuantos valores tiene una tupla usando len()
>>> len(diego)
3

#Para indicar que una tupla tiene un solo valor se hace lo siguiente
>>> julie = ('orizaba',)
>>> type(julie)

#Puedes convertir una lista, cadena y diccionario a tupla
>>> tuple(['cat', 'dog', 5])	
('cat', 'dog', 5)
```



## Diccionarios

Un diccionario es un tipo de dato mutable, es una colección de muchos valores encerrados en llaves. A diferencia de las listas, los índices de los diccionarios pueden ser diferentes tipos de datos, no solo enteros.

Los índices de los diccionarios se llaman keys y una key con su valor asociado se llama key-value pair. Los key y sus valores se separan con dos puntos.

Ejemplo de un diccionario

| myCat = {'size' : 'fat', 'color' : 'gray', 'disposition' : 'loud'} |
| :----------------------------------------------------------: |

Las key son 'size', 'color' y 'disposition'



**Operaciones con diccionarios**



**Métodos de diccionarios**

| Método       | Definición  | Ejemplo |
| ------------ | ----------- | ------- |
| keys()       | Este método |         |
| values()     |             |         |
| items()      |             |         |
| get()        |             |         |
| setdefault() |             |         |



## Cadenas

Una cadena es un tipo de dato inmutable y se define por usar comillas simples.

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







## Importar módulos a python

## Códigos

```python
```





## PEP8

* Una tabulación debe tener cuatro espacios.



