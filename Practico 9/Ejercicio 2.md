# Ejercicio 2 Practico 9

**pseudocodigo**

## QuickSelect

**ALGORITHM QuickSelect(A[0..n-1], k)**

  // A es el array de tamaño n

  // k es el índice del elemento que queremos encontrar (0 <= k < n)
  
  left ← 0
  right ← n - 1
  
  while left ≤ right do

    // Selecciona un pivote, aca se usara el último elemento como pivote

    pivotIndex ← Partition(A, left, right)
    
    if pivotIndex = k then

      // Si el pivote es el k-ésimo elemento, se devolvera su valor

      return A[pivotIndex]

    else if pivotIndex < k then

      // Si el pivote está antes del k-ésimo, ajusta el rango a la derecha

      left ← pivotIndex + 1

    else

      // Si el pivote está después del k-ésimo, ajusta el rango a la izquierda

      right ← pivotIndex - 1
      
  end while

END ALGORITHM



## Algoritmo auxiliar para realizar la partición en el array

**ALGORITHM Partition(A[0..n-1], left, right)**

  // Usa el último elemento como pivote

  pivot ← A[right]

  i ← left - 1
  
  for j ← left to right - 1 do

    if A[j] ≤ pivot then

      i ← i + 1

      Intercambiar(A[i], A[j])

    end if

  end for
  
  // Coloca el pivote en la posición correcta

  Intercambiar(A[i + 1], A[right])

  return i + 1  // Retorna la posición final del pivote

END ALGORITHM

**ALGORITHM Intercambiar(A[0..n-1], i, j)**
  
  // Intercambia los elementos en las posiciones i y j
  
  temp ← A[i]
  
  A[i] ← A[j]
  
  A[j] ← temp

END ALGORITHM
