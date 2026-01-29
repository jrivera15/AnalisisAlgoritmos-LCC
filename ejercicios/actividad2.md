# Análisis de Algoritmos I
Ciencias de la Computación<br>
Departamento de Matemáticas<br>
Universidad de Sonora

## ✏️ ACTIVIDAD 2 - COMPLEJIDAD ALGORÍTMICA Y NOTACIÓN ASINTÓTICA

### Parte 1 — Conceptos
Explica con tus palabras:<br><br>
a) ¿Qué significa la complejidad de un algoritmo “crezca”?
<br><br>
b) ¿Qué debemos considerar si contamos el tiempo en segundos?

### Parte 2 — Contar operaciones


| ID | Algoritmo | # operaciones | T(n) | O() |
|---|---|----------|----------|----------|
| A | <pre><code>def sum_list(lst):</code><br><code>  total = 0</code><br><code>  for value in lst:</code><br><code>    total += value</code><br><code>  return total   </code></pre>   |    |
| B | <pre><code>def distancia(p, q):</code><br><code>  dx = (p[0] - q[0]) ** 2</code><br><code>  dy = (p[1] - q[1]) ** 2</code><br><code>  return (dx + dy) ** 0.5  </code></pre> |   |
| C | <pre><code>def minimum(lst):</code><br><code>  min_value = lst[0]</code><br><code>  for i in range(1, len(lst)):</code><br><code>    min_value = min(min_value, lst[i])</code><br><code>  return min_value</code></pre>   |    |
| D | <pre><code>def matrix_mul(A, B):</code><br><code>  n = len(A)</code><br><code>  res = [[0 for _ in range(n)] for _ in range(n)]</code><br><code>  for i in range(n):</code><br><code>    for j in range(n):</code><br><code>      for k in range(n):</code><br><code>        res[i][j] += A[i][k] * B[k][j]</code><br><code>  return res</code></pre>   |    |
| E | <pre><code>import itertools</code><br><code>for order in itertools.permutations([1, 2, 3]):</code><br><code>  print(order)</code></pre>  |    |
| F | <pre><code>def contar_divisiones(n):</code><br><code>  contador = 0</code><br><code>  while n > 1:</code><br><code>      n //= 2</code><br><code>      contador += 1</code><br><code>  return contador</code></pre>  |    |
| F | <pre><code>def process_data(data):</code><br><code>  clean_data(data)     # O(N<sup>2</sup>)</code><br><code>  analyze_data(data)   # O(N<sup>3</sup>)</code></pre>  |    |
| G | Supongamos que estamos analizando 4 diferentes funciones. Todas tienen un ciclo _for_ y dentro del ciclo se ejecuta lo mismo. Considera los siguientes ciclos y compara explícita e implícitamente el costo del ciclo:<pre><code>a) for(i = 0; i < n; i++)</code><br><code>       x = 1 + 1;</code><br><code>b) for(i = 0; i < n; i += 2)</code><br><code>       x = 1 + 1</code><br><code>c) for(i = 1; i < n; i *= 2)</code><br><code>       x = 1 + 1;</code><br><code>d) for(i = n; i > 1; i /= 2)</code><br><code>       x = 1 + 1;</code></pre>¿Cuál función será la más eficiente? |    |



### Parte 3 — Función de costo 𝑇(𝑛)  a Big-O

> [!NOTE]
> O(1) < O(log 𝑛) < O(𝑛) < O(𝑛 log 𝑛) < O(𝑛<sup>2</sup>) < O(2<sup>𝑛</sup>) < O(𝑛!)

| ID | Función de costo | ¿Qué término domina? | Big-O |
|---|---|----------|----------|
| A |𝑇(𝑛)=5𝑛<sup>2</sup> + 2𝑛 + 7 |
| B |𝑇(𝑛)=𝑛<sup>3</sup> + 𝑛<sup>2</sup> + 1 |
| C |𝑇(𝑛)=2<sup>𝑛</sup> + log 𝑛 + 10 |
| D |𝑇(𝑛)=10 + 2𝑛 |

¿Cuál algoritmo será el más eficiente?


### Parte 3 — Graficar funciones de costo
Grafica e indica a que función corresponde:

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

d)
| Tamaño de entrada (n) | # de operaciones |
| ----------------------- | --------------------- |
| 1                       | 0                     |
| 2                       | 1                     |
| 4                       | 2                     |
| 8                       | 3                     |
| 16                      | 4                     |
| 32                      | 5                     |

