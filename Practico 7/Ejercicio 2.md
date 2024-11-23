# Ejercicio 2 Practico 7

**Pasos del Algoritmo**

Dado que los vasos están inicialmente ordenados en dos grupos: los primeros n están llenos y los últimos n están vacíos, identificamos que el patrón alternado ideal es tener:

- Los vasos en posiciones impares llenos.
- Los vasos en posiciones pares vacíos.

Se usara un método de intercambios, donde se tomara un vaso lleno en una posición incorrecta y lo intercambiaremos con un vaso vacío en una posición incorrecta.

**Pseudocodigo**

ALGORITHM AlternateVasos(Vasos[1..2n])

  // Supone que Vasos está inicializado con los primeros n llenos y los últimos n vacíos

  i ← 1  // Índice para buscar vasos llenos en posiciones incorrectas

  j ← 2  // Índice para buscar vasos vacíos en posiciones incorrectas

  while i <= 2n and j <= 2n do
    // Buscar un vaso lleno en posición incorrecta (posición par)

    while i <= 2n and (i % 2 ≠ 0 or Vasos[i] = 'vacío') do

      i ← i + 2

    // Buscar un vaso vacío en posición incorrecta (posición impar)

    while j <= 2n and (j % 2 ≠ 1 or Vasos[j] = 'lleno') do

      j ← j + 2

    // Intercambiar si ambos índices están en rango

    if i <= 2n and j <= 2n then

      intercambiar(Vasos[i], Vasos[j])

      i ← i + 2

      j ← j + 2
  end while
END ALGORITHM


**Número de Movimientos**

Cada intercambio corrige dos posiciones incorrectas. Por lo tanto, el número total de movimientos necesarios será n, ya que necesitamos corregir la mitad de los vasos llenos (que están inicialmente en posiciones incorrectas) con la mitad de los vasos vacíos.