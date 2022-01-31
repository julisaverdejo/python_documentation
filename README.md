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
| `print()`    | Muestra en la pantalla del valor dentro del paréntesis. Esta función tiene las palabras clave **end** y **sep**; con end puedes hacer que dos cadenas se impriman en la misma línea de código; con sep puedes separar varias cadenas con cualquier caracter. |
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

**if**

**else**

**elif**

**while**

**for**



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
| Indexación            | Puedes acceder a cualquier valor de una lista. En caso de que una lista estuviera conformada de otras listas puedes acceder a cualquier lista y valor usando dos corchetes `spam[0][1]`. Los índices también pueden ser números negativos. | `spam[0] = ['cat', 'bat']                                         ` |
| Concatenación         | Puedes concatenar listas con listas o con cadenas con el signo + | `'The ' + spam[0][-2] + ' is fat' = 'The cat is fat'`        |
| Replicación           | La replicación de listas se da con el signo * y un número, el número indica cuantas veces se replicará la lista. | `['X','Y'] * 3 = ['X', 'Y', 'X', 'Y', 'X', 'Y']`             |
| Slices                | Los slices son secciones que contienen más de un valor. Generalmente los slices tienen dos argumentos pero también pueden lucir así [:n] o así [n:], el primero indica que el slice iniciará en 0 hasta n-1 y el segundo que iniciará desde n hasta el final de la lista. Si en algún momento te encuentras un slice así [:] significa que abarcará todos los valores de una lista. | `spam[:2] = [['cat', 'bat'],['rat', 'elephant']] `           |
| Eliminar valores      |                                                              |                                                              |
| Longitud de una lista |                                                              |                                                              |
| Conversión a listas   |                                                              |                                                              |
| in                    |                                                              |                                                              |
| not in                |                                                              |                                                              |
| Asignación múltiple   |                                                              |                                                              |

**Métodos de una lista**

| Método     | Definición | Ejemplo |
| ---------- | ---------- | ------- |
| `index()`  |            |         |
| `append()` |            |         |
| `insert()` |            |         |
| `remove()` |            |         |
| `sort()`   |            |         |













## Importar módulos a python

## Códigos

```python
```





## PEP8

* Una tabulación debe tener cuatro espacios.



