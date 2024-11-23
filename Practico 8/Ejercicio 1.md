# Ejercicio 1 Practico 8

Array=[3, 14, 27, 31, 39, 42, 55, 70, 74, 79, 100, 110, 120]

Longitud n = 13

**En búsqueda binaria:**

- Divide el array en mitades en cada iteración.
- En el peor caso, realiza comparaciones hasta que el tamaño del subarray sea 1.

El número máximo de comparaciones está dado por el techo del logaritmo base 2 de n:


Maximo de comparaciones = ⌈log 2(n)⌉ = ⌈log 2(13)⌉ = ⌈3.7⌉ = 4.

## 1. Número medio de comparaciones en una búsqueda exitosa
Cuando se realiza una búsqueda exitosa, cada elemento del array tiene una profundidad determinada en el árbol de búsqueda binaria.

**Construcción del árbol de búsqueda:**

En el nivel 0 (raíz): 70 (1 comparación).

En el nivel 1: 39 y 85 (2 comparaciones cada uno).

En el nivel 2: 14,55,81,93 (3 comparaciones cada uno).

En el nivel 3: 3,27,42,74,98,31 (4 comparaciones cada uno).

**Calcular el total de comparaciones:**

Suma de todas las comparaciones:

S=(1⋅1)+(2⋅2)+(4⋅3)+(6⋅4)=1+4+12+24=41.

**Promedio:**
El promedio de comparaciones es:

Promedio = Suma de comparaciones / Número de elementos = 41 / 13 = 3.15.

Resultado: El número medio de comparaciones en una búsqueda exitosa es 3.15.

## 2. Número promedio de comparaciones en una búsqueda sin éxito

En una búsqueda sin éxito, las comparaciones se realizan en los n + 1 = 14 intervalos formados entre los elementos del array, incluyendo antes del primer elemento y después del último.

**Profundidades de los intervalos:**

- Los intervalos están en las mismas profundidades que los nodos más cercanos en el árbol.
- Profundidades por intervalos (de izquierda a derecha):
[4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 3, 3, 3, 3, 3, 3, 3, 3, 2, 2, 2, 2, 2, 2, 2, 1, 1, 1, 1, 1, 1, 1]

**Calcular el total de comparaciones:**

- Suma de profundidades:

S=(5⋅4)+(7⋅3)+(2⋅2)=20+21+4=45.

**Promedio:**

- El promedio de comparaciones es:

Promedio = Suma de comparaciones / Número de intervalos = 45 / 14 = 3.21.

Resultado: El número promedio de comparaciones en una búsqueda sin éxito es3.21.