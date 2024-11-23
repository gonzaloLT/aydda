# Ejercicio 1 Practico 6

## Paso a Paso del Enfoque de Búsqueda Exhaustiva
**Definición del Problema:** Queremos asignar a 4 personas a 4 trabajos de tal manera que el coste total sea el mínimo. La matriz de coste está dada por C, que define el coste C[i,j] si la persona i es asignada al trabajo j.

**Formato de Solución:** Cada solución factible se representa como una permutación de { 1 , 2 , 3 , 4 } , donde cada número en la tupla indica el trabajo asignado a cada persona en orden.

**Generación de Permutaciones:** Hay 4!=24 permutaciones posibles de las asignaciones de trabajos. Para cada permutación, calculamos el coste total sumando los valores correspondientes de la matriz C.

## Evaluación Detallada de las Asignaciones
Permutaciones posibles y sus respectivos costos:

1. ⟨ 1 , 2 , 3 , 4 ⟩:

- Coste = C[1,1] + C[2,2] + C[3,3] + C[4,4] = 9 + 4 + 1 + 4 = 18

2. ⟨ 1 , 2 , 4 , 3 ⟩:
- Coste = 9 + 4 + 8 + 9 = 30

3. ⟨ 1 , 3 , 2 , 4 ⟩:
- Coste = 9 + 3 + 8 + 4 = 24

4. ⟨ 1 , 3 , 4 , 2 ⟩:
- Coste = 9 + 3 + 8 + 6 = 26

5. ⟨ 1 , 4 , 2 , 3 ⟩:
- Coste = 9 + 7 + 8 + 9 = 33

6. ⟨ 1 , 4 , 3 , 2 ⟩:
- Coste = 9 + 7 + 1 + 6 = 23

7. ⟨ 2 , 1 , 3 , 4 ⟩:
- Coste = C[1,2] + C[2,1] + C[3,3] + C[4,4] = 2 + 6 + 1 + 4 = 13

8. ⟨ 2 , 1 , 4 , 3 ⟩:
- Coste = 2 + 6 + 8 + 9 = 25

9. ⟨ 2 , 3 , 1 , 4 ⟩:
- Coste = 2 + 3 + 5 + 4 = 14

10. ⟨ 2 , 3 , 4 , 1 ⟩:
- Coste = 2 + 3 + 8 + 7 = 20

11. ⟨ 2 , 4 , 1 , 3 ⟩:
- Coste = 2 + 7 + 5 + 9 = 23

12. ⟨ 2 , 4 , 3 , 1 ⟩:
- Coste = 2 + 7 + 1 + 7 = 17

13. ⟨ 3 , 1 , 2 , 4 ⟩:
- Coste = 7 + 6 + 8 + 4 = 25

14. ⟨ 3 , 1 , 4 , 2 ⟩:
- Coste = 7 + 6 + 8 + 6 = 27

15. ⟨ 3 , 2 , 1 , 4 ⟩:
- Coste = 7 + 4 + 5 + 4 = 20

16. ⟨ 3 , 2 , 4 , 1 ⟩:
- Coste = 7 + 4 + 8 + 7 = 26

17. ⟨ 3 , 4 , 1 , 2 ⟩:
- Coste = 7 + 7 + 5 + 6 = 25

18. ⟨ 3 , 4 , 2 , 1 ⟩:
- Coste = 7 + 7 + 8 + 7 = 29

19. ⟨ 4 , 1 , 2 , 3 ⟩:
- Coste = 8 + 6 + 8 + 9 = 31

20. ⟨ 4 , 1 , 3 , 2 ⟩:
- Coste = 8 + 6 + 1 + 6 = 21

21. ⟨ 4 , 2 , 1 , 3 ⟩:
- Coste = 8 + 4 + 5 + 9 = 26

22. ⟨ 4 , 2 , 3 , 1 ⟩:
- Coste = 8 + 4 + 1 + 7 = 20

23. ⟨ 4 , 3 , 1 , 2 ⟩:
- Coste = 8 + 3 + 5 + 6 = 22

24. ⟨ 4 , 3 , 2 , 1 ⟩:
- Coste = 8 + 3 + 8 + 7 = 26

## Conclusión:

La asignación óptima es ⟨ 2 , 1 , 3 , 4 ⟩, con un coste total mínimo de 13.
Esto indica que:

- Persona 1 se asigna al Trabajo 2.
- Persona 2 se asigna al Trabajo 1.
- Persona 3 se asigna al Trabajo 3.
- Persona 4 se asigna al Trabajo 4.