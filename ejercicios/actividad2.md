# Análisis de Algoritmos I
Ciencias de la Computación<br>
Departamento de Matemáticas<br>
Universidad de Sonora

## ✏️ ACTIVIDAD 2 - COMPLEJIDAD ALGORÍTMICA Y NOTACIÓN ASINTÓTICA

### Parte 1 — Conceptos
Explica con tus palabras:<br><br>
a) ¿Qué significa que un algoritmo “crezca”?
<br><br>
b) ¿Por qué contamos el número de operaciones y no el tiempo en segundos?

### Parte 2 — Contar operaciones


| ID | Algoritmo | # operaciones | T(n) | O() |
|---|---|----------|----------|----------|
| A | <pre><code>x = x + 1</code></pre>   |    |
| B | <pre><code>for i = 1 to n:</code><br><code>    a = a + 1</code></pre> |   |
| C | <pre><code>for i = 1 to n:</code><br><code>    for j = 1 to n:</code><br><code>        a = a + 1</code></pre>   |    |
| D | <pre><code>for i = 1 to n:</code><br><code>    x = x + 1</code><br><br><code>for j = 1 to n:</code><br><code>    y = y + 1</code></pre>   |    |
| E | <pre><code>for i = 1 to n:</code><br><code>    x = x + 1</code><br><br><code> for j = 1 to n:</code><br><code>    for k = 1 to n:</code><br><code>        y = y + 1</code></pre>  |    |


### Parte 3 — Graficar funciones de costo

a)
|Tamaño de entrada (n) | # de operaciones |
|---|---|
| 1 | 4 |
| 2	| 4 |
| 3	| 4 |
| 4	| 4|
| 5	| 4|

b)
|Tamaño de entrada (n) | # de operaciones |
|---|---|
| 1 | 2 |
| 2	| 4 |
| 3	| 6 |
| 4	| 8|
| 5	| 10|

c)
|Tamaño de entrada (n) | # de operaciones |
|---|---|
| 1 | 1 |
| 2	| 4 |
| 3	| 9 |
| 4	| 16|
| 5	| 25|

### Parte 4 — Función de costo 𝑇(𝑛)  a Big-O

> [!NOTE]
> O(1) < O(log 𝑛) < O(𝑛) < O(𝑛 log 𝑛) < O(𝑛<sup>2</sup>) < O(2<sup>𝑛</sup>) < O(𝑛!)

| ID | Función de costo | ¿Qué término domina? | Big-O |
|---|---|----------|----------|
| A |𝑇(𝑛)=5𝑛<sup>2</sup>+2𝑛+7 |
| B |𝑇(𝑛)=𝑛<sup>3</sup>+𝑛<sup>2</sup>+1 |
| C |𝑇(𝑛)=2<sup>𝑛</sup>+ log 𝑛+10 |







