$\tau$ es el total

En el caso de la ultima clase:

$\mu$ valor promedio por cuenta

$\tau$ era la cantidad total de las 484 cuentas por cobrar

| Promedio                                           | Total                                                    |
| -------------------------------------------------- | -------------------------------------------------------- |
| $\hat{\mu} = \frac{\sum{y_i}}{n}$                  | $\hat{\tau} = \frac{\sum{N * y_i}}{n}$                   |
| $\hat{V}(\bar{y}) = \frac{S^2}{n}*(\frac{N-n}{N})$ | $\hat{V}(N\bar{y}) = N^2\frac{S^2}{n} * \frac{ N- n}{N}$ |
| $S^2 = \frac{\sum{(y_i - \bar{y})^2}}{n-1}$        | $S^2 = \frac{\sum{(y_i - \bar{y})^2}}{n-1}$              |
| $2 * \sqrt{V(\bar{y})}$                            | $2 * \sqrt{V(N\bar{y})}$                                 |

Recordando el ejercicio

### Ejercicio

Calcular el total poblacional a partir de una muesrta aleatoria de $n=9$ registros de un hospital que quiere estimar la cantidad promedio de la deuda sobre $N=484$ cuentas abiertas. Los valores de la muestra por estos nueve registros están listados en la tabla siguiente.

Estime $\mu$, la cantidad promedio de la deuda, y establezca un limite para el error de estimación.

Estime $\tau$ que es el total de la deuda que tienen con el hospital

| Datos |
| ----- |
| 33.5  |
| 32    |
| 52    |
| 43    |
| 40    |
| 41    |
| 45    |
| 42.5  |
| 39    |


Ver el excel adjunto

Calculo del tamaño de la muestra para estimar $\mu$

Si la población es desconocida o infinita

- $n$: es el tamaño de la muestra
- $Z$: es el nivel de confianza
- $s^2$: 

$$
n = \frac{\frac{Z_{\alpha}^2}{2} * S^2}{e^2}
$$

Selección para el tamaño de muestra

Tamaño de muestra requerido para estimar $\mu$ con un limite para el error de estimación B, esta fórmula es para una confianza del $95\%$

$$
n = \frac{N*\sigma^2}{(N-1) * D + \sigma^2}
$$

$$
D = \frac{B^2}{4}
$$

Tamaño de muestra requerido para estimar $\tau$ con un limite de para el error de estimación B:

$$
n = \frac{N*\sigma^2}{(N-1) * D + \sigma^2}
$$

$$
D = \frac{B^2}{4N^2}
$$

Donde $2*\sqrt{\hat{V}(\bar{y})}$ es la cota del error

Nota: Cuando $\hat{p} * \hat{q}$ sea $0.5 * 0.5$ el valor será maximo

Muestreo estratificado

Es partir la muestra en pequeñas poblaciones de forma que sea más homogeno al interior de cada subpoblación y más heterogeneo entre subpoblaciones

Caracteristicas

- Los limites pueden ser más pequeños

Notación:

- $L$ Número de estratos
- $N_{i}$ Número de unidades muestrales es el estrato $i$
- $N$ Número de unidades muestrales en la población

$$\bar{y}_{st} = \frac{1}{N} * \sum_{i=1}^{L}{N_i\bar{y}_i}$$