Teorema central del limite

El Teorema centra del limite dice que si se tiene una población de
de tamañan N y se toman muestras de tamaño de esa población con
reemplazar entonces se cumplen los siguientes supuestos

$∈(x) = u$

$∇_{x} = ∇_{población} / \sqrt{n}$

Si dado el caso se toman muestras sin reemplazar entonces se tienen
los siguientes supuestos:

$∈_x = u$

$(∇_{x})^2 = ∇^2 / n * (N - n / N - 1)$

Ejemplo: Se tiene un población de N = 5 elementos

$N = {1, 2, 3, 4, 5}$

Demostrar el teorema central del limite con reemplazo

Calcular μ y ∇ de la población

$μ = (∑_{x_i}/N)$

$μ = (1 + 2 + 3 + 4 + 5)/5$

$μ = 3$

Tomando muestras de tamaño $n=2$. Cuantas muestras se tienen

$(∇_{x})^2 = (∑_{(x_i - μ)^2}/N)$

$(∇_{x})^2 = ((1 - 3)^2 + (2 - 3)^2 + (3 - 3)^2 + (4 - 3)^2 + (5 - 3)^2/5)$

$(∇_{x})^2 = 2$

$∇_{x} = \sqrt{2}$

El número de muestras posibles será igual a:

$muestras = N^n$

$muestras = 5^2$

$muestras = 25$

$N = {1, 2, 3, 4, 5}$

$N = {x_1, x_2, x_3, x_4, x_5}$

Todas las muestras posibles de tamaño 2 serán:

$x_1x_1 = 1      x_2 x_1=1,5     x_3x_1      x_4x_1      x_5x_1$

$x_1x_2 = 1      x_2 x_2=1,5     x_3x_1      x_4x_1      x_5x_1$

$x_1x_1 = 1      x_2 x_1=1,5     x_3x_1      x_4x_1       x_5x_1$

$x_1x_1 = 1      x_2 x_1=1,5     x_3x_1      x_4x_1      x_5x_1$

$x_1x_1 = 1      x_2 x_1=1,5     x_3x_1      x_4x_1       x_5x_1$

Nota: La representación en matriz se denommina datos NO agrupados

Para demostrar que las todas las muestras serán iguales a $u$

$∈_{x_{barra}} = u$

$∈_x = (1 + 1,5 + 2 + ... + 5 / 25)$

$∈_{x_{barra}} = (75 / 25)$

$∈_{y_{barra}} = 3$

| $y_i$ | $n_i$ | $y_i * n_i$ |
| ----- | ----- | ----------- |
| 1     | 1     | 1           |
| 1,5   | 2     | 3           |
| 2     | 3     | 6           |
| 2,5   | 4     | 10          |
| 3     | 5     | 15          |
| 3,5   | 4     | 14          |
| 4     | 3     | 12          |
| 4,5   | 2     | 9           |
| 5     | 1     | 5           |
| Total | 25    | 75          |

Nota: La representación en tabla se denommina datos agrupados

$∈_{x_{barra}} = u$

$∈_{x_{barra}} = (75 / 25)$

$∈_{y_{barra}} = 3$

El máximo está en $y_i = 3$, $n_i=5$ Donde la suma de todo será igual a 25

$Y_{barra} = \frac{∑Y_i * n_i}{n}$

Con esta formula se calculan los datos agrupados

---

Con esta formula podemos llegar a una expresión diferente

$∇^2 = S^2 = \frac{(∑x_i - x_{barra})^2}{n}$

$S^2 = \frac{∑x_i^2}{n} - ∑x_{barra}^2$

$S^2 = \frac{(∑x_i - x_{barra})^2}{n}$

$S^2 = \frac{(∑(x_i^2 - 2x_ix_{barra} + x_{barra}^2)}{n}$

$S^2 = \frac{∑x_i^2}{n} - \frac{∑2x_ix_{barra}}{n} + \frac{∑x_{barra}^2}{n}$

$S^2 = \frac{∑x_i^2}{n} - 2x_{barra}\frac{∑x_i}{n} + x_{barra}^2\frac{∑1}{n}$

Como ${∑x_i}$ será igual que ${n}$ se puede decir que $\frac{∑x_i}{n}$
es igual a 1

$S^2 = \frac{∑x_i^2}{n} - 2x_{barra}^2 + x_{barra}^2\frac{∑1}{n}$

De forma similar $\frac{∑1}{n}$ será $\frac{n}{n}$ es decir $1$

$S^2 = \frac{∑x_i^2}{n} - 2x_{barra}^2 + x_{barra}^2$

> Por tanto se afierma que $S^2 = \frac{∑x_i^2}{n} - x_{barra}^2$

| $y_i$ | $n_i$ | $y_i * n_i$ | $y_i^2 * n_i$ |
| ----- | ----- | ----------- | ------------- |
| 1     | 1     | 1           | 1             |
| 1,5   | 2     | 3           | 4,5           |
| 2     | 3     | 6           | 12            |
| 2,5   | 4     | 10          | 25            |
| 3     | 5     | 15          | 45            |
| 3,5   | 4     | 14          | 49            |
| 4     | 3     | 12          | 48            |
| 4,5   | 2     | 9           | 40,5          |
| 5     | 1     | 5           | 25            |
| Total | 25    | 75          | 250           |

Aplicando la formula a la que se llegó

$S^2 = \frac{∑x_i^2}{n} - ∈_{y_barra}^2$

$∈_{x_{barra}} = (75 / 25)$

$∈_{y_{barra}} = 3$

Usando la formula

$S^2 = \frac{250}{25} - 3^2$

$S^2 = 10 - 9$

> Por tanto $S^2=1$

---

Este mismo ejercicio pero sin reemplazo sería:

$muestras = \frac{N!}{n!(N-n)!}$

$muestras = \frac{5!}{2!(5-2)!}$

$muestras = 10$

Por tanto ya que no se repiten como en el ejercicio anterior se dice que
la forma no agrupada quedaría:

|                |              |              |              |
| -------------- | ------------ | ------------ | ------------ |
| $x_1x_2 = 1,5$ | $x_2x_3=2,5$ | $x_2x_3=3,5$ | $x_2x_3=4,5$ |
| $x_1x_3 = 2$   | $x_2x_4=3$   | $x_2x_3=4$   |              |
| $x_1x_4 = 2,5$ | $x_2x_5=3,5$ |              |              |
| $x_1x_5 = 3$   |              |              |              |

Calculamos la varianza de forma no agrupada:

$(∇_{x})^2 = \frac{∇_{población}^2}{n} * (N - n / N - 1)$

$(∇_{x})^2 = \frac{2}{2} * (5 - 2 / 5 - 1)$

$(∇_{x})^2 = 1 * (3 / 4)$

> Por lo tanto $(∇_{x})^2 = 0,75$

Ahora expresando este en forma ordenando tenemos

| $y_i$ | $n_i$ | $y_i*n_i$ | $y_i^2*n_i$ |
| ----- | ----- | --------- | ----------- |
| 1,5   | 1     | 1,5       | 2,25        |
| 2     | 1     | 2         | 4           |
| 2,5   | 2     | 5         | 12,5        |
| 3     | 2     | 6         | 18          |
| 3,5   | 2     | 7         | 24,5        |
| 4     | 1     | 4         | 16          |
| 4,5   | 1     | 4,5       | 20,25       |
| Total | 10    | 30        | 97,5        |

Ahora comprobamos que con estos datos se cumpla el teorema de central del limite

$∈_{y_{barra}} = \frac{∑y_i*n_i}{n}$

$∈_{y_{barra}} = (30 / 10)$

> Por tanto $∈_{y_{barra}} = 3$

Ahora comprobamos la varianza:

$S^2 = \frac{∑y_i^2*n_i}{n} - ∈_{y_{barra}}^2$

$S^2 = \frac{97,5}{10} - 9$

$S^2 = 9,75 - 0$

> Por tanto $S^2 = 0,75$
