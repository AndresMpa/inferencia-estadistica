# Recap

Exposión combinatorial: Cuando se dispara el número de calculos de una combinatoría

$E(x_{barra}) = u$ -> Media

$V(x_{barra}) = \frac{(∇_{x})^2 }{n}$ -> Varianza

$σ(x_{barra}) = \frac{σ_{x}}{\sqrt{n}}$ -> Desviación

## Distribución normal

Distribución normal

Dominio: (-∞, ∞)
Rango: [0, 1]

## Formas de calcular distribuciones

Para distribuciones normal de probabilidad

$z = \frac{x_{barra} - u}{∇}$

Para distribución muestral de probabilidad

$z = \frac{x_{barra} - u}{\frac{∇}{\sqrt{n}}}$

## Ejemplo

Una maquina embotelladora puede ser regulada para que descargue
un promedio de $μ$ onzas por botella. Se ha observado que la cantidad
de líquido dosificado por una máquina está distribuida normalmente con
$σ = 1.0$. Una muestra de $n = 9$ botellas se selecciona aleatoriamente
de la poblaciónde la máquina en un día determinado (todas embotelladas
con el mismo ajuste de la maquina) y las onzas de contenido líquido
se miden para cada una. Determine la probabilidad de que la media muestral
se encuentre a no más de 0.3 onza de la verdadera media $μ$ para ajuste
seleccionado de la maquina

## Solución

$σ = 1.0$
$n = 9$

$-0.3 ≤ x_{barra} - μ ≤ 0.3$ dividio entre $\frac{σ}{\sqrt{n}}$

$ \frac{-0,3}{\frac{1}{\sqrt{9}}} ≤ z ≤ \frac{0,3}{\frac{1}{\sqrt{9}}} $

$ -0,9 ≤ z ≤ 0,9 $

$P(-0,9 ≤ z ≤ 0,9)$

$P(z ≤ 0,9) - P(z ≤ -0,9)$

# TODO: Robarse la grafica de Nicole

## Ejemplo #2

$N = 122$

Calcular la media $μ$ y variancia $σ$ para los eventos

$μ = (∑_{x_i}/N)$

$μ = (28 + 21 + ... + 27 + 21)/122$
$μ = 26.3360656$

$σ = 4.72976389$

## Ejemplo #3

Calcular las probabilidades de que al tomar una muestra de 20 jugadores
del circuito, esos esten más o menos 4 eventos de la media poblacional

$n = 20$
$μ = 26.3360656$
$σ = 4.72976389$

Es valido afirmar que la media poblacional es $μ = 26.3360656$, por tanto
si se está pidiendo z de $μ + 4$ y $μ - 4$

$z_1 = \frac{30.3360 - 26.3360}{\frac{4.72976389}{\sqrt{20}}}$
$z_1 = 3.7822$

$z_2 = \frac{22.3360 - 26.3360}{\frac{4.72976389}{\sqrt{20}}}$
$z_2 = -3.7822$

$P(22.3360 ≤ x ≤ 30.3360) = P(-3.7822 ≤ z ≤ 3.7822) = P(z ≤ 3.7822) - P(z ≤ -3.7822) = 0.9998$

## Ejemplo #4

¿Cual es la probabilidad de que al tomar una muestra de 30 jugadores, hayan
participado en 27 o más eventos? Sabiendo que media $μ$ y variancia $σ$ son
los valores calculados previamente

$n = 30$
$μ = 26.3360656$
$σ = 4.72976389$

Si $μ = 26.3360656$ es la media poblacional, $x_{barra}$ 27

$z = \frac{27 - 26.3360}{\frac{4.72976389}{\sqrt{30}}}$
$z = 0.7688$

Ahora bien con el valor de $z$ se calcula

$P(x_{barra} ≤ 27) = P(z ≥ 0.7688) = 1 - (z ≤ 0.7688)$

$1 - 0.7790$

$0.2210$
