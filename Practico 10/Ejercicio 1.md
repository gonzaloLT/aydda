# Ejercicio 1 Practico 10

Lista inicial: E, X, A, M, P, L, E

## Paso 1: Dividir la lista
**Dividimos la lista en dos mitades:**

1. E, X, A
2. M, P, L, E

## Paso 2: Dividir recursivamente las mitades

**1. Para la primera mitad E, X, A:**

La dividimos en:
- E
- X, A

Dividimos X, A en:
- X
- A

**2. Para la segunda mitad M, P, L, E:**

La dividimos en:
- M, P
- L, E

Dividimos M, P en:
- M
- P

Dividimos L, E en:
- L
- E

## Paso 3: Comenzar a fusionar las sublistas

Ahora empezamos a combinar las sublistas en orden alfabético:

**1. Combinar X y A:**

- Ordenado: A, X

**2. Combinar E con A, X:**

- Ordenado: A, E, X

**3. Combinar M y P:**

- Ordenado: M, P

**4. Combinar L y E:**

- Ordenado: E, L

**5. Combinar M, P con E, L:**

Comparando y fusionando en orden:
- E viene primero.
- Luego L.
- Después M.
- Finalmente P.

Ordenado: E, L, M, P

## Paso 4: Fusionar las dos mitades ordenadas

Finalmente, fusionamos A, E, X con E, L, M, P:

**1. Comparando los elementos de ambas sublistas:**

- A viene primero.
- Luego E de la primera mitad.
- Después E de la segunda mitad.
- Luego L.
- Después M.
- Luego P.
- Finalmente X.

**2. La lista ordenada final es:**

A, E, E, L, M, P, X
