# Laboratorio 1 - Computación Paralela

## Pruebas sobre el comportamiento de la memoria caché
El alumno debe realizar un informe en formato artículo (en Latex) donde la implementación, resultados y análisis de la ejecución para los siguientes problemas:
- Implementar y comparar los 2-bucles anidados FOR presentados en el cap. 2 del libro, pag 22.
- Implementar en C/C++ la multiplicación de matrices clásica, la versión de tres bucles anidados y evaluar su desempeño considerando diferentes tamaños de matriz.
- Implementar la versión por bloques (investigar en internet), seis bucles anidados, evaluar su desempeño y compararlo con la multiplicación de matrices clásica.
- Ejecutar ambos algoritmos paso a paso, y analizar el movimiento de datos entre la memoria principal y la memoria cache. Hacer una evaluación de acuerdo a la complejidad algorítmica.
- Ejecutar ambos algoritmos utilizando las herramientas valgrind y kcachegrind para obtener una evaluación mas precisa de su desempeño.

## Ejecución Valgrid y Kcachegrind

```bash
g++ -g -O0 ejercicio2.cpp -o ejercicio2
valgrind --leak-check=full --track-origins=yes ./ejercicio2
```