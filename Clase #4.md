# Tamaños de muestra

$Z = \frac{x - μ}{\frac{σ}{\sqrt{n}}}$

- Z para la distribucióno muestral, que tiene a una normal
- Es simetrica

Si despejamos μ

$Z = \frac{x - μ}{\frac{σ}{\sqrt{n}}}$

$x - μ = Z * \frac{σ}{\sqrt{n}}$

Estos son invervalos de confianza donde alpha se puede dividir
en 2 partes iguales, demanera tal que

$α = 0,05$

$Z * \frac{α}{2} = 0,025$

$Z * (1 - \frac{α}{2}) = 0,975$

Donde $ε$ será el error de estimación

$μ = x ± (Z * \frac{σ}{\sqrt{n}})$

$μ = x ± ε$

Despejar n

$ε^2 = (Z * \frac{σ}{\sqrt{n}})^2$

$ε^2 = \frac{Z^2 * σ^2}{n}$

$n = (\frac{Z * σ}{ε})^2$

## Ejercicio

Es una población de 2000 personas se sabe que 1100 de ellas tiene
como su fuente de información para las noticias, la radio y
televisión tradicionales.

- Si se toma una muestra de 1350 personas que probabilidad hay de
que 1350 o más

- Si se quiere un error de estimación de 5% con una confianza del
96% cuantas personas se deberían encuestar

- Si se quiere un error estimación de 5% con una cuanfianza 94%
cuantas personas se deberían encuestar

- Si se quiere un error del 3,5% con una confianza del 96% cuantas
personas se deberían encuestar

- Si se quiere un error del 3,5% con una confianza del 94% cuantas
personas se deberían encuestar

#### Medida

$n = (\frac{z*σ}{ε})^2$

#### Proporción

$n = \frac{z^2*P*Q}{ε^2}$

## Soluciones

### Ejercicio #1
$p = \frac{1100}{2000}$

$p = 0.55$

$p_{gorrito} = \frac{1350}{2000}$

$p_{gorrito} = 0.675$

$z = \frac{0.675 - 0.55}{\sqrt{\frac{0.55 * 0.45}{2000}}}$

$P(x >= 1350) = P_{gorrito} >= 0.675 = P(z >= 11.23) = 1 - P(z <= 0.45)$

$Z = 11.23$

### Ejercicio #2

Nivel de confianza = NC

$ NC = 100\% - α\%$
$ 96\% = 100\% - α\%$
$ α\% = 100\% - 96\%$
$ α\% = 4\%$

Ahora se divide por 2 para sacar ambas partes de la simetría

$ \frac{α\%}{2} = 4\%$ 
$ α\% = 2\%$

Nivel de significación

$ α = 0.02$

Niveles de confianza

$n = \frac{2.054^2*0.55*0.45}{0.05^2}$

$n = 417,5675$

$n ≈ 418$


$n = \frac{-1.881^2*0.55*0.45}{0.05^2}$

$n = 350.27$

$n ≈ 351$

$n = \frac{z^2*P*Q}{ε^2}$

$n$ y $z$ son directamente proporcionales
$n$ y $ε$ son inversamente proporcionales
