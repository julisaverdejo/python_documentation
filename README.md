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

| Función   | Descripción |
| --------- | ----------- |
| `print()` |             |
| `input()` |             |
| `len()`   |             |
| `str()`   |             |
| `int()`   |             |
| `bool()`  |             |
| `float()` |             |
| `list()`  |             |
| `tuple()` |             |
| `range()` |             |











```python
abcd
```





## Códigos

```python
```





## PEP8

* Una tabulación debe tener cuatro espacios.



