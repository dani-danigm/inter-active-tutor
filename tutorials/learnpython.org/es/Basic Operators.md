Tutorial
--------

Esta sección explica un poco sobre como usar los operadores básicos en Python. 

### Operadores Aritméticos  


Tal como cualquier otro lenguaje de programación, los operadores de sumas, restas, multiplicaciones y divisiones pueden ser usadas con números.<br> 

    numeros = 1 + 2 * 3 / 4.0

Intenta predecir cual será la respuesta. Si python sigue las ordenes de los operadores?

Otro operador disponible es el de modulo (%), este regresa el integral remanente de una división, tal que dividendo % divisor = remanente.

    remanente = 11 % 3

Usando dos simbolos de multiplicación (*) crea una relación de potencia.

    cuadrado = 7 ** 2
    cubico = 2 ** 3

### Usando operadores con texto

Python soporta unir texto usando el operador de adición:

    holamundo = "hola" + " " + "mundo"

Python también soporta multiplicar texto o cadenas para formar una cadena con una secuencia repetitiva:

    muchosholas = "hola" * 10

### Usar Operadores con listas

Listas pueden ser unidas con los operadores de adición:

    numeros_pares = [2,4,6,8]
    numeros_impares = [1,3,5,7]
    numeros_todos = numeros_pares + numeros_impares

Al igual que con los Strings, Python soporta la creacion de nuevas listas, repitiendo una secuencia utilizando el operador multiplicacion (*) :

    print [1,2,3] * 3

### Ejercicios

El objetivo de este ejercicio es crear dos listas llamadas `x_lista` y `y_lista`, las cuales contendrán 10 instancias de las variables `x` e `y`,respectivamente. También se requiere crear una lista llamada "gran_lista", la cual contendrá las variables `x` e `y`, 10 veces cada una, concatenando las dos listas que has creado.

Tutorial de Código
-------------

x = object()
y = object()

# Cambia este código
x_lista = [x]
y_lista = [y]
gran_lista = []

print "x_lista contiene %d objetos" % len(x_lista)
print "y_lista contiene %d objetos" % len(y_lista)
print "gran_lista contiene %d objetos" % len(gran_lista)

# Código de prueba
if x_lista.count(x) == 10 and y_lista.count(y) == 10:
    print "Casi llegamos..."
if gran_lista.count(x) == 10 and gran_lista.count(y) == 10:
    print "Genial!"

Expected Output
---------------

x_lista contiene 10 objetos
y_lista contiene 10 objetos
gran_lista contiene 20 objetos
Casi llegamos...
Genial!

Solucion
--------
x = object()
y = object()

# Cambia este codigo
x_lista = [x]*10
y_lista = [y]*10
gran_lista = x_lista + y_lista

print "x_lista contiene %d objetos" % len(x_lista)
print "y_lista contiene %d objetos" % len(y_lista)
print "gran_lista contiene %d objetos" % len(gran_lista)

# Código de prueba
if x_lista.count(x) == 10 and y_lista.count(y) == 10:
    print "Casi llegamos..."
if gran_lista.count(x) == 10 and gran_lista.count(y) == 10:
    print "Genial!"
