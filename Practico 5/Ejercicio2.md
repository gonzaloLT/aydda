# Ejercicio 2: Comparaciones en la Búsqueda de Fuerza Bruta

## Cálculo del número de comparaciones:

**Datos:**

- Longitud del texto: t = 47.

- Longitud del patrón: p = 6.

**El algoritmo va a realizar comparaciones desde cada posición del texto:**

*1. Posición 0 (THERE_):*

- Comparaciones: 1 (falla en la primera letra: T vs G).

*2. Posición 1 (HERE_I):*

- Comparaciones: 1 (falla en la primera letra: H vs G).

*3. Posición 2 (ERE_IS):*

- Comparaciones: 1 (falla en la primera letra: E vs G).

*4. Continuamos de la misma manera hasta la posición 26, donde cada intento falla en la primera letra.*

*5. Posición 27 (G_ITS_):*

- Comparación 1: G vs G → Coincide.
- Comparación 2: _ vs A → Falla.
- Total de comparaciones en esta posición: 2.

*6. Posiciones 28 a 41:*

- En cada una de estas posiciones, no hay coincidencias con la primera letra del patrón (G).
- Por lo tanto, en cada posición se realiza solo 1 comparación antes de fallar.

**Total de Comparaciones**

El patrón se intenta comparar desde las posiciones 0 hasta 47−6=41, ya que el patrón tiene 6 caracteres.

*1. Posiciones 0 a 26:* 27 posiciones con 1 comparación cada una:

27 * 1 = 27 comparaciones

*2. Posición 27:* 2 comparaciones.

*3. Posiciones 28 a 41:* 14 posiciones con 1 comparación cada una:

14×1=14 comparaciones

**Cálculo del Total Exacto**

- 27 + 2 + 14 = 43 comparaciones

**Resultado Final**

El total exacto de comparaciones es 43, teniendo en cuenta que en la posición G_ITS_ se realizan 2 comparaciones debido a una coincidencia parcial.