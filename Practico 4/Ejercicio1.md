# Ejercicio 1 Practico 4: Alternando discos

Se usara un algoritmo que recorra la lista de discos y realice intercambios siempre que se encuentre un disco rojo a la derecha de un disco azul.

**pseudocódigo**

ALGORITHM AlternarDiscos(A[0..2n - 1])

  movimientos ← 0

  for i ← 0 to 2n - 2 do

    for j ← 0 to 2n - 2 - i do

      if A[j] = 🔵 and A[j + 1] = 🔴 then

        Intercambiar(A[j], A[j + 1])

        movimientos ← movimientos + 1

  return movimientos

**Número de Movimientos**

- En el peor caso, la complejidad del algoritmo es de O(n^2), ya que es similar a un algoritmo de ordenación burbuja.
- El número exacto de movimientos dependerá del estado inicial de la lista. En el peor caso, si empezamos con la secuencia alternada ideal, se requerirá hacer un máximo de n^2 movimientos para llevar los discos a su posición final.


