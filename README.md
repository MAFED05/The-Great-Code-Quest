# The Great Code Quest

Buen día, bienvenidos otra vez a otro reto, en este caso el reto #8 en el que resolveremos algunos ejercicios sobre la segunda parte de los bucles, así que sin más que añadir comencemos...

## Punto #1

1. Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.

***Solución***

``` python
for a in range(1, 101): #Para cada a en el rango desde 1 hasta 100
    Resultado = a ** 2 #Definimos la operación donde llamamos a todos los números del rango y se encuentra su potencia
    print(" El cuadrado de " + str(a) + " es " + str(Resultado)) #Imprimimos el resultado
```

***Código funcionando***

## Punto #2

2. Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.


***Solución***

``` python
# Listado de números impares
for b in range(1, 1000, 2): #Rango que va desde 1 hasta 999 y va aumentando de a 2, de manera que siempre será impar
    print(b) #Imprimos los números impares

# Listado de números pares
for b in range(2, 1001, 2): #Rango que va desde 2 hasta 1000 y aumenta de a 2
    print(b) #Imprimimos los números pares
```

***Código funcionando***

## Punto #3

3. Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado


***Solución***

``` python
n = int(input("Ingresa un número natural mayor o igual a 2: ")) #Se le solicita al usuario que ingrese un número mayor o igual a 2

# Si n es impar, lo convertimos a par disminuyéndolo en 1
if n % 2 != 0: #Se halla el módulo de la división y si es diferente de 0 entonces se le resta 1
    n -= 1

# Imprimimos los números pares en forma descendente hasta 2
for i in range(n, 1, -2): #Inicia el rango en n hasta 2, disminuyendo de a 2
    if i % 2 == 0: #Definimos un condicional para verificar que el número si sea par
        print(i) #Imprimimos i
```

***Código funcionando***

## Punto #4

4. Imprimir los números de 1 hasta un número natural n dado, cada uno con su respectivo factorial


***Solución***

``` python
n = int(input("Ingresa un número natural: ")) #Se le solicita al usuario que ingrese un número entero

for i in range(1, n+1): #Para un rango desde 1 hasta n, se le espeficia el +1 para que no vaya a restar nada
    factorial = 1 #Se inicializa la variable en 1
    for j in range(1, i+1): #Para un rango desde 1 hasta i y al mismo que el anterior se le suma 1 para que no quite un valor
        factorial *= j #Se le dice que la variable será factorial a la potencia de j
    print("El factorial de "+ str(i)+ " es", factorial) #Se imprime el resultado
```

***Código funcionando***

## Punto #5

5. Calcular el valor de 2 elevado a la potencia n usando ciclos for.


***Solución***

``` python
n = int(input("Ingresa un número natural: ")) #Se le solicita al usuario que ingrese un número entero

for i in range(1, n+1): #Para un rango desde 1 hasta n, se le espeficia el +1 para que no vaya a restar nada
    factorial = 1 #Se inicializa la variable en 1
    for j in range(1, i+1): #Para un rango desde 1 hasta i y al mismo que el anterior se le suma 1 para que no quite un valor
        factorial *= j #Se le dice que la variable será factorial a la potencia de j
    print("El factorial de "+ str(i)+ " es", factorial) #Se imprime el resultado
```

***Código funcionando***

## Punto #6

6. Leer un número natural n, leer otro dato de tipo real x y calcular x^n usando ciclos for.


***Solución***

``` python

```

***Código funcionando***


## Punto #7

7. Diseñe un programa que muestre las tablas de multiplicar del 1 al 9.


***Solución***

``` python
```

***Código funcionando***

## Punto #8

8. Diseñar una función que permita calcular una aproximación de la función exponencial alrededor de 0 para cualquier valor x (real), utilizando los primeros n términos de la serie de Maclaurin


***Solución***

``` python
```

***Código funcionando***

## Punto #9

9. Diseñar una función que permita calcular una aproximación de la función seno alrededor de 0 para cualquier valor x (real), utilizando los primeros n términos de la serie de Maclaurin.


***Solución***

``` python
```

***Código funcionando***

## Punto #10

10. Diseñar una función que permita calcular una aproximación de la función arcotangente alrededor de 0 para cualquier valor x en el rango [-1, 1], utilizando los primeros n términos de la serie de Maclaurin. 

***Solución***

``` python
```

***Código funcionando***

