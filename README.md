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

[![Captura-de-pantalla-2023-04-16-230338.png](https://i.postimg.cc/766sQvv8/Captura-de-pantalla-2023-04-16-230338.png)](https://postimg.cc/1gkrfj5J)

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

[![Captura-de-pantalla-2023-04-16-230403.png](https://i.postimg.cc/9f85fYC2/Captura-de-pantalla-2023-04-16-230403.png)](https://postimg.cc/d7ySHdhN)

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

[![Captura-de-pantalla-2023-04-16-230436.png](https://i.postimg.cc/JhhvSHJ2/Captura-de-pantalla-2023-04-16-230436.png)](https://postimg.cc/nX63Dz34)

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

[![Captura-de-pantalla-2023-04-16-230521.png](https://i.postimg.cc/Hn06rTXM/Captura-de-pantalla-2023-04-16-230521.png)](https://postimg.cc/sGXY8dnf)

## Punto #5

5. Calcular el valor de 2 elevado a la potencia n usando ciclos for.


***Solución***
```python

n = int(input("Ingrese el valor de n: ")) #Le solicitamos al usuario que ingrese el número

resultado = 1 #Inicializamos la variable en 1
for i in range(n): #Definimos el rango
    resultado *= 2 # Generamos el bucle junto con la potencia

print("2 elevado a la potencia", n, "es igual a", resultado) #Imprimimos el resultado

```

***Código funcionando***

[![Captura-de-pantalla-2023-04-16-233026.png](https://i.postimg.cc/SRzf9k9d/Captura-de-pantalla-2023-04-16-233026.png)](https://postimg.cc/hQcmWFpQ)

## Punto #6

6. Leer un número natural n, leer otro dato de tipo real x y calcular x^n usando ciclos for.


***Solución***

``` python
n = int(input("Ingrese el valor de n: ")) #Se le solicita al usuario que ingrese el entero
x = float(input("Ingrese el valor de x: ")) #Se le solicita al usuario que ingrese el real
resultado = 1 #Se inicializa la variable en 1
for i in range(n): #Se define el rango
    resultado *= x #Se define la operación a realizar
print(x, "elevado a la potencia", n, "es igual a", resultado) #Imprimimos los resultados
```

***Código funcionando***

[![Captura-de-pantalla-2023-04-16-231128.png](https://i.postimg.cc/zBrWVKjd/Captura-de-pantalla-2023-04-16-231128.png)](https://postimg.cc/wtw3rtnJ)}

## Punto #7

7. Diseñe un programa que muestre las tablas de multiplicar del 1 al 9.


***Solución***

``` python
for i in range(1, 10): #Comenzamos definiedo en rango de 1 a 9
    print("Tabla de multiplicar del", i) #Imnprimimos el enunciado para cada número del rango
    for j in range(1, 11): # Colocamos el rango desde 1 hasta 10
        resultado = i * j #Multiplicamos el primer término por el segundo por medio del bucle
        print(i, "x", j, "=", resultado) #Imprimimos el resultado
    print () #Utilizamos este print para que haya una línea en blanco después de cada tabla y no queden todas juntas
```

***Código funcionando***

[![Captura-de-pantalla-2023-04-16-230645.png](https://i.postimg.cc/SsN3F2MP/Captura-de-pantalla-2023-04-16-230645.png)](https://postimg.cc/t1w2FgDd)

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

