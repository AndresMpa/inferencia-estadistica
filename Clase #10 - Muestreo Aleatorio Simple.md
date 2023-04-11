# Muestreo Aleatorio Simple

Cada una de las muestras de un población tiene la misma probabilidad de ser escogida

Definición:

Es cuando una muestra es formulada de tal manera que cada elemento en la población tiene la misma oportunidad de ser incluido

La cuota de error sirve para estimar entre que valor se va a mover la cuouta poblacional

Formulas:

- $\hat{\mu} = \bar{y}$ Estimador para la media poblacional
- $\hat{V}(\bar{y})$ Varianza estimada de $y$
- $S^2$ Desviación estandar
- $2*\sqrt{\hat{V}(\hat{y})}$ Limite para el error de estimación

$$\hat{\mu} = \bar{y} = \frac{\sum y_i}{n}$$

$$\hat{V}(\bar{y}) = \frac{S^2}{n}*\frac{N-n}{N}$$

$$S^2 = \frac{\sum(y_i-\hat{y})^2}{n-1}$$

$$2*\sqrt{\hat{V}(\hat{y})} = 2*\sqrt{\frac{S^2}{n}*\frac{N - n}{N}}$$

$$li = \hat{\mu} - 2 \sqrt{V(\bar{y})}$$

$$ls = \hat{\mu} + 2 \sqrt{V(\bar{y})}$$

Para el calculos de $s^2$ se puede usar:

```
VAR.S()
```

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

Ejemplos en la hoja 3 y 4