# Ejercicio 1: Métrica de tamaño, operación básica y recuento

## 1. Calcular la suma de los primeros \(n\) números naturales
- **Métrica de tamaño**: El número \(n\).
- **Operación básica**: Una suma.
- **Recuento diferente por entradas del mismo tamaño**: No, el número de sumas es fijo e igual a \(n\).

---

## 2. Calcular \(n!\)
- **Métrica de tamaño**: El número \(n\).
- **Operación básica**: Una multiplicación.
- **Recuento diferente por entradas del mismo tamaño**: No, el número de multiplicaciones es fijo e igual a \(n - 1\).

---

## 3. Encontrar el elemento más grande en una lista de \(n\) números
- **Métrica de tamaño**: El número de elementos \(n\).
- **Operación básica**: Una comparación.
- **Recuento diferente por entradas del mismo tamaño**: Sí, en el mejor caso (elemento mayor al principio) se pueden realizar menos comparaciones que en el peor caso (elemento mayor al final).

---

## 4. Algoritmo de Euclides
- **Métrica de tamaño**: Los valores iniciales de los números \(a\) y \(b\).
- **Operación básica**: Un cálculo del residuo.
- **Recuento diferente por entradas del mismo tamaño**: Sí, depende de las entradas iniciales y la rapidez con la que se reduzcan al MCD.

---

## 5. Tamiz de Eratóstenes
- **Métrica de tamaño**: El número \(n\).
- **Operación básica**: Marcar un número como eliminado (asignación en el array).
- **Recuento diferente por entradas del mismo tamaño**: No, el número de operaciones depende de \(n\) de manera fija.

