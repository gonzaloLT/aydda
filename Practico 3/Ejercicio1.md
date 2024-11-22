# Ejercicio 1 Practico 3: Relación de recurrencia para F(n)
Definición del problema: F(n) es un algoritmo recursivo para calcular n!, donde:

     
F(n) = { 1                  si 𝑛 = 0 o 𝑛 = 1

F(n) = { n * F (n−1)        si 𝑛 s> 1
​
 
**Relación de recurrencia para el número de llamadas:**

Sea T(n) el número de llamadas realizadas por el algoritmo:

- Caso base: T(0)=1 (solo se realiza la llamada inicial).
- Caso recursivo: Cada llamada a F(n) realiza una llamada a F(n−1). Por lo tanto:

T(n) = T(n−1) + 1

**Resolviendo la recurrencia:**

Expandimos la relación:

T(n) = T(n−1) + 1

T(n−1) = T(n−2) + 1

T(n) = T(n−2) + 2

Repetimos el proceso n veces hasta llegar al caso base:

T(n) = T(0) + n

Como T(0) = 1:

T(n) = 1 + n

**Número total de llamadas:**

El número total de llamadas realizadas por F(n) es T(n)=n+1.