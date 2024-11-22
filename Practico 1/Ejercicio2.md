# Ejercicio 2: Algoritmo para calcular ⌊√n⌋

**pseudocodigo**

ALGORITHM FloorSquareRoot(n)

// Calcula ⌊√n⌋ para un entero positivo n

// Input: Un entero positivo n

// Output: El mayor entero k tal que k^2 ≤ n


k ← 0

while (k + 1) * (k + 1) ≤ n do

  k ← k + 1

return k