# Tarea 1

Resuelve los siguientes ejercicios.

## Ejercicio 1
Orden de crecimiento: ¿cuántas operaciones se ejecutan a medida que N crece? Calcula y anota en la tabla.

| Descripción | Función | N=1 | N=10 | N=100 | N=1000 |
|---|---|---|---|---|---|
| constante | 1 |   |   |   |   |
| logaritmico | log N |   |   |   |   |
| lineal | N |   |   |   |   |
| linearítmico | N log N |   |   |   |   |
| cuadrático | N<sup>2</sup> |   |   |   |   |
| cúbico | N<sup>3</sup> |   |   |   |   |
| exponencial | 2<sup>N</sup> |   |   |   |   |

## Ejercicio 2
Asume que se ha hecho el análisis teórico para varios algoritmos y se ha calculado su _T(n)_. Anota el término dominante y especifica, en el peor de los casos, cuál sería la complejidad _O(n)_ para cada uno.

| _T(n)_ | Término dominante | _O(n)_ |
|---|---|---|
| 5 + 0.001n<sup>3</sup> + 0.025n|   |   |  
| 500n + 100n<sup>1.5</sup> + 50n log<sub>10</sub> n  |   |   |
| 0.3n + 5n<sup>1.5</sup> + 2.5 · n<sup>1.75</sup> |   |   |  
| n<sup>2</sup>log2 n + n(log<sub>2</sub> n)<sup>2</sup> |   |   |   
| n log<sub>3</sub> n + n log<sub>2</sub> n |   |   |   
| 3 log<sub>8</sub> n + log<sub>2</sub>log<sub>2</sub>log<sub>2</sub> n |   |   |  
| 100n + 0.01n<sup>2</sup>|   |   | 
| 0.01n + 100n<sup>2</sup>|   |   |   
| 2n + n<sup>0.5</sup> + 0.5n</up>1.25</sup> |   |   |   
| 0.01n log<sub>2</sub> n + n(log<sub>2</sub> n)<sup>2</sup> |   |   | 
| 100n log<sub>3</sub> n + n<sup>3</sup> + 100n |   |   | 
| 0.003 log<sub>4</sub> n + log<sub>2</sub>log<sub>2</sub> n |   |   | 

## Ejercicio 3
Calcular el tiempo de ejecución (redondedo hacia arriba a segundos, minutos, días, años, etc.) para diferentes algoritmos con distintos órdenes de complejidad, dependiendo de cómo varía el tamaño de la entrada n, y considerando que la computadora ejecuta 1 millón de operaciones por segundo.

Notas:
- Si el tiempo es menor que 1 segundo se puede poner la etiqueta "<1 seg" 
- Si el tiempo excede los 30 años se puede poner la etiqueta: "intratable". 

| Tamaño de la entrada | n | n log n | n<sup>2</sup> | n<sup>3</sup> | 1.5<sup>n</sup> | 2<sup>n</sup> | n! |
|-------|---|---|---|---|---|---|---|
| n=10         | <1 seg  | <1 seg  | <1 seg  | <1 seg  | <1 seg  | <1 seg  | 4 seg  |
| n=30         | <1 seg  |   |   |   |   |   |   |
| n=50         | <1 seg  |   |   |   |   |   |   |
| n=100        | <1 seg   |   |   |   |   |   |   |
| n=1,000      | <1 seg   |   |   |   |   |   |   |
| n=100,000    | <1 seg   |   |   |   |   |   |   |
| n=1,000,000  | 1 seg  |   |   |   |   |   |   |