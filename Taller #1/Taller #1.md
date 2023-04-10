<p align="center">
Taller de Distribuciones Muestrales
</p><p align="center">
Marzo 10 de 2023
</p>

1. Según un estudio realizado por una empresa hotelera durante un año, la distribución del tiempo de estancia de cada viajero fue normal con una media de $3.7$ días y una desviación típica de $0.75$ días.

a. A lo largo del año 2022 se analizó el tiempo de estancia y se quiere determinar ¿Cuál es la probabilidad que un turista se quede más de 3,5 días en una muestra de 49 viajeros elegidos al azar?

$μ = 3.7$

$σ = 0.75$

$\bar{x} = 3.5$

$n = 49$

Para calcular la probabilidad $z$ se usa:

$$
z = \frac{\bar{x} - μ}{\frac{σ}{\sqrt{n}}}
$$

Por tanto:

$$
z = \frac{3.5 - 3.7}{\frac{0.75}{\sqrt{49}}}
$$

Simplificando la expresión interna:

$$
\frac{0.75}{\sqrt{49}} = \frac{0.75}{7}
$$

Reemplanzando la expresión:

$$
z = \frac{3.5 - 3.7}{\frac{0.75}{7}}
$$

Restando $3.5 - 3.7$ y efectuando $\frac{0.75}{\sqrt{49}}$:

$$
z = \frac{-0.2}{0.1071}
$$

Por tanto:

$z \approx -1.866$

$P(z >= 3.5) = 1 - 0.031020683$

$P(z >= 3.5) = 0.968979317$

> Por tanto la probabilidad es de aproximadamente $96.899\%$

b. Si se quiere una diferencia de un cuarto de día con respecto a la media poblacional de que tamaño debe ser la muestra, si se quiere una confianza del $98\%$

$NC = 100\% - α\%$
$98\% = 100\% - α\%$
$α\% = 100\% - 98\%$
$α\% = 2\%$
$\frac{α\%}{2} = 2\%$
$α\% = 1\%$

Por tanto $α = 0.01$

```
=DISTR.NORM.ESTAND.INV(0,01)
```

$z = -2.326347874 \approx -2.33$

$σ = 0.75$

Ya que es un $1/4$ de día, se tomat $ε = 0.25$

$$
n = (\frac{z*\sigma}{\epsilon})^2
$$

$$
n = (\frac{-2.33 * 0.75}{0.25})^2
$$

$$
n = \frac{-2.33^2 * 0.75^2}{0.25^2} \approx 51.87
$$

> Por tanto, la muestra debe ser de tamaño $52$ aproximadamente

2. El Instituto de Mercadotecnia de Alimentos de un país indica que el $17\%$ de las familias gastan más de $450000$ pesos por mes en alimentación. Se sabe que la proporción poblacional es $P=0.17$, si se selecciona una muestra aleatoria de $800$ familias.

¿Cuál es la probabilidad que la proporción muestral este $± 0,02$ de la proporción poblacional?

$n = 800$

$P = 0.17$

Ya que $P = 0.17$ entonces

$Q = 0.83$

$\epsilon = 0.02$

$\hat{P} = 0.17$

Ya que el error $ε$ será de 0.02, se puede afirmar que:

$\hat{P}_{1} = \hat{P} - \epsilon$

$\hat{P}_{1} = 0.15$

$\hat{P}_{2} = \hat{P} + \epsilon$

$\hat{P}_{2} = 0.19$

Para calcular la probabilidad $Z$ podemos usar la formula

$$
Z = \frac{\hat{P} - P}{\sqrt{\frac{P * Q}{n}}}
$$

Por tanto se deberá de calcular:

$$
Z_{1} = \frac{\hat{P}_{1} - 0.17}{\sqrt{\frac{0.17 * 0.83}{800}}}
$$

$$
Z_{1} = \frac{0.15 - 0.17}{\sqrt{\frac{0.17 * 0.83}{800}}}
$$

$Z_{1} = -1.505953223$

$$
Z_{2} = \frac{\hat{P}_{2} - 0.17}{\sqrt{\frac{0.17 * 0.83}{800}}}
$$

$$
Z_{2} = \frac{0.19 - 0.17}{\sqrt{\frac{0.17 * 0.83}{800}}}
$$

$Z_{2} = 1.505953223$

Por ende parar calcular la probabilidad se puede decir que, la probabilidad de que la proporción muestral este $± 0.02$ de la proporción poblacional será

$P(\hat{P}_{1} ≤ \hat{P} ≤ \hat{P}_{2})$

$P(0.15 ≤ 0.17 ≤ 0.19)$

Lo que es equivalente a

$P(-1.505953223 ≤ Z ≤ 1.505953223)$

Así que, para determinar la probabilidad se ha de tomar la diferencia entre ambas probabilidades, la probabilidad de que se esté $ε$ por debajo (-0.02) y $ε$ por encima (+0.02), por ende:

$P_{2}(Z ≤ 1.505953223)$

```
=DISTR.NORM.ESTAND(1.505953223)
```

$P_{2} = 0.93396041$

$P_{1}(Z ≤ -1.505953223)$

```
=DISTR.NORM.ESTAND(-1.505953223)
```

$P_{1} = 0.06603959$

$P = P_{2} - P_{1}$

$P = 0.93396041 - 0.06603959$

$P = 0.86792082$

$P \approx 86.79\%$

> Por tanto la probabilidad de que la probabilidad que la proporción muestral este ±0,02 de la proporción poblacional, será de aproximadamente 86.79%

¿Cuál es la probabilidad que la proporción muestral de p sea de más de $0.22$?

$P(\hat{P} \gt 0.22) = ?$

$n = 800$

$P = 0.17$

Ya que $P = 0.17$ entonces

$Q = 0.83$

$\hat{P} = 0.22$

Para ello se puede usar la formula

$$
Z = \frac{\hat{P} - P}{\sqrt{\frac{P * Q}{n}}}
$$

Usando la formula:

$$
Z = \frac{0.22 - 0.17}{\sqrt{\frac{0.17 * 0.83}{800}}}
$$

$Z = 3.764883057$

Por tanto, la probabilidad de que la proporción muestral de p sea de más de $0.22$, será equivalente a

$P(\hat{P} \gt 0.22) = P(Z \gt 3.764883057)$

Ya que se busca la probabilidad de que sea "de más de $0.22$", esto se representa como la diferencia entre el total y la probabilidad de $0.22$

$P = 1 - P(Z \gt 3.764883057)$

```
=DISTR.NORM.ESTAND(3.764883057)
```

$P \approx 1 - 0.9999$

$P \approx 0.0001$

> Por tanto la probabilidad de que la probabilidad que la proporción muestral de p sea de más de $0.22$ es de $0.001\%$

3. Los datos sobre el perfil de la audiencia del sitio de la Red ESPN indicaron que el $31\%$ de los usuarios son mujeres. Suponga que este porcentaje se basó en una muestra de $600$ usuarios.

$P = 0.31$

$Q = 0.69$

$n = 600$

a. Que probabilidad hay de encontrar de que la proporción muestral este a $± 0.025$ de la proporción poblacional

$\epsilon = 0.025$

Por tanto tomando los datos preliminares

$\hat{P} = 0.31$

$\hat{P}{1} = 0.31 - \epsilon$

$\hat{P}_{1} = 0.31 - 0.025$

$\hat{P}_{1} = 0.285$

$\hat{P}_{2} = 0.31 + \epsilon$

$\hat{P}_{2} = 0.31 + 0.025$

$\hat{P}_{2} = 0.335$

Para calcular la probabilidad se puede usar

$$
Z = \frac{\hat{P} - P}{\sqrt{\frac{P * Q}{n}}}
$$

Por ende $Z$ será

$$
Z_{1} = \frac{\hat{P}_{1} - P}{\sqrt{\frac{P * Q}{n}}}
$$

$$
Z_{1} = \frac{\hat{P}_{1} - 0.31}{\sqrt{\frac{0.31 * 0.69}{600}}}
$$

$$
Z_{1} = \frac{0.285 - 0.31}{\sqrt{\frac{0.31 * 0.69}{600}}}
$$

$Z_{1} = -1.324067853$

$$
Z_{2} = \frac{\hat{P}_{2} - P}{\sqrt{\frac{P * Q}{n}}}
$$

$$
Z_{2} = \frac{\hat{P}_{2} - 0.31}{\sqrt{\frac{0.31 * 0.69}{600}}}
$$

$$
Z_{2} = \frac{0.335 - 0.31}{\sqrt{\frac{0.31 * 0.69}{600}}}
$$

$Z_{2} = 1.324067853$

Para calcular la probabilidad

$P(0.285 \le x \le 0.335)$

Lo que es equivalente a

$P(-1.324067853 \le Z \le 1.324067853)$

Así que, para determinar la probabilidad de encontrar que la proporción muestral este a ±0.025 de la proporción poblacional, se dice que:

$P_{1}(Z ≤ -1.324067853)$

```
=DISTR.NORM.ESTAND(-1.324067853)
```

$P_{1} = 0.09274026$

$P_{2}(Z ≤ 1.324067853)$

```
=DISTR.NORM.ESTAND(1.324067853)
```

$P_{2} = 0.90725974$

$P = P_{2} - P_{1}$

$P = 0.90725974 - 0.09274026$

$P = 0.81451949$

$P \approx 81.45\%$

> Por ende se puede decir que, la probabilidad de encontrar que la proporción muestral este a ±0.025 de la proporción poblacional, es de $81.45\%$

b. Que probabilidad hay que al tomar una muestra de $210$ mujeres ellas mujeres escuchen Red ESPN

$\hat{P} = \frac{210}{600}$

$\hat{P} = 0.35$

Para calcular la probabilidad se puede usar

$$
Z = \frac{\hat{P} - P}{\sqrt{\frac{P * Q}{n}}}
$$

Usando la formula

$$
Z = \frac{0.35 - 0.31}{\sqrt{\frac{0.31 * 0.69}{600}}}
$$

$Z = 2.1185$

Por tanto la probabilidad con una muestra de que al tomar una muestra de $210$ mujeres ellas mujeres escuchen Red ESPN

$P(x = 210)$

$P(z = 2.1185)$

$P = 0.9829$

> Por tanto la probabilidad de que al tomar una muestra de $210$ mujeres ellas escuchen Red ESPN es de: $98.29\%$

c. Que tamaño debe tener la muestra para que el margen de error sea del $4\%$ con una confianza del $98\%$

Primero calculamos el nivel de confianza:

$NC = 100\% - α\%$
$98\% = 100\% - α\%$
$α\% = 100\% - 98\%$
$α\% = 2\%$
$\frac{α\%}{2} = 2\%$
$α\% = 1\%$

$\epsilon = 0.04$

Por tanto podemos usar

$$
n = \frac{Z^2 * P * Q}{\epsilon^2}
$$

Usando la formula

$$
n = \frac{Z^2 * 0.31 * 0.69}{0.04^2}
$$

Por lo que para calcular Z:

$Z = P(x \le 0.01)$

```
=DISTR.NORM.ESTAND.INV(0,01)
```

$Z = -2.326347874$

$$
n = \frac{-2-326347874^2 * 0.31 * 0.69}{0.04^2}
$$

$n = 723.5026368$

$n \approx 724$

> La población debe ser de aproximadamente $724$

4. Las estaturas de $1000$ estudiantes están distribuidas aproximadamente en forma normal con una media de $174.5$ centímetros y una desviación estándar de $6.9$ centímetros. Si se extrae una muestra aleatoria de tamaño $50$ de esta población, determine:

$μ = 174.5$
$σ = 6.9$
$n = 50$

a. ¿Cuál es la probabilidad que un alumno tenga una estatura entre $172.5$ y $175.8$ centímetros?

Para calcular la probabilidad se puede usar:

$$
Z = \frac{\bar{x} - μ}{\frac{σ}{\sqrt{n}}}
$$

Usando la formula:

$$
Z_{1} = \frac{172.5 - 174.5}{\frac{6.9}{\sqrt{50}}}
$$

$Z_{1} = -2.04958$

$$
Z_{2} = \frac{175.8 - 174.5}{\frac{6.9}{\sqrt{50}}}
$$

$Z_{2} = 1.33223$

$P(-2.04958 \le x \le 1.33223)$

$P_{1} = P(x \le -2.04958)$

$P_{2} = P(x \le 1.33223)$

$P = P_{2} - P_{1}$

$P = 0.908607689 - 0.020202717$

$P = 0.888404972$

> Por tanto, la probabilidad que un alumno tenga una estatura entre $172.5$ y $175.8$ centímetros será igual a: $88.84\%$

b. ¿Cuál es la probabilidad que un alumno tenga una estatura por debajo de $172$ centímetros?

$$
Z = \frac{172 - 174.5}{\frac{6.9}{\sqrt{50}}}
$$

$Z = -2.25454336$

$P(x \lt -2.25454336)$

$P = 1 - 0.012081003$

$P = 0.987918997$

> Por tanto se la probabilidad que un alumno tenga una estatura por debajo de $172$ centímetros $98.79\%$

c. Si se quiere una diferencia de un $8$ cm con respecto a la media poblacional de que tamaño debe ser la muestra, si se quiere una confianza del $98\%$

$NC = 100\% - α\%$
$98\% = 100\% - α\%$
$α\% = 100\% - 98\%$
$α\% = 2\%$
$\frac{α\%}{2} = 2\%$
$α\% = 1\%$

Para calcular la muestra se puede usar

$$
n = \frac{Z^2 * σ}{\epsilon^2}
$$

Para calcular z se puede usar la distribución inversa

```
=DISTR.NORM.ESTAND.INV(0,01)
```

$Z = -2.326347874$

$$
n = \frac{2.326347874^2 * 6.9^2}{8^2}
$$

$n = 4.025942092$

$n \approx 4$

> Por ende, de diferir en 8 cm con respecto a la media poblacional con un intervalo de confianza del 98% se debe tener una muestra de aproximadamente 4 personas

5. Una compañía aérea sabe que en promedio sus aviones tienen retrasos que siguen una distribución normal con media de $10$ minutos y desviación estándar de $5$ minutos. Determinar:

$\mu = 10$
$\sigma = 5$

a. La probabilidad que en una muestra de $15$ aviones, un avión llegue con no más de $10$ minutos de retraso

$P(x \leq 10)$

$\bar{x} = 10$

$n = 15$

Para esto se puede usar la formula:

$$
z = \frac{\bar{x} - \mu}{\frac{\sigma}{\sqrt{n}}}
$$

Usando la formula:

$$
z = \frac{10 - 10}{\frac{5}{\sqrt{15}}}
$$

$z = 0$

```
=DISTR.NORM.ESTAND(0)
```

$P(z \leq 0) = 0.5$

$P = 0.5$

> Por tanto, la probabilidad que en una muestra de $15$ aviones, un avión llegue con no más de $10$ minutos de retraso es del 50%

b. La probabilidad que en una muestra de $15$ aviones, un avión tenga un retraso de más de $15$ minutos

$P(x \gt 15)$

$\bar{x} = 15$

$n = 15$

Para esto se puede usar la formula:

$$
z = \frac{\bar{x} - \mu}{\frac{\sigma}{\sqrt{n}}}
$$

Usando la formula:

$$
z = \frac{15 - 10}{\frac{5}{\sqrt{15}}}
$$

$z = 3.872983346$

```
=DISTR.NORM.ESTAND(3.872983346)
```

$P = 1 - P(z \gt 3.872983346)$

$P = 1 - 0.999946244$

$P = 0.00005$

> Por tanto la probabilidad de que en una muestra de $15$ aviones, un avión tenga un retraso de más de $15$ minutos, es casi nula con una probabilidad del 0.0005%

c. Si en un día llegan $10$ aviones de esa compañía al aeropuerto de la ciudad, ¿Cuantos llegaran con retrasos de más de $20$ minutos?

$P(x \gt 20)$

$\bar{x} = 20$

$n = 10$


Para esto se puede usar la formula:

$$
z = \frac{\bar{x} - \mu}{\sigma}
$$

Usando la formula:

$$
z = \frac{20 - 10}{5}
$$

$z = 2$

```
=DISTR.NORM.ESTAND(2)
```

$P = 1 - P(z \gt 2)$

$P = 1 - 0.977249868$

$P = 0.02275$

$P \approx 0.0228$

Por lo tanto, la probabilidad de que un avión tenga un retraso de más de 20 minutos es de aproximadamente $0.228\%$

Dada la probabilidad de $0.228\%$, es decir; $P \approx 0.0228$, por tanto:

$$
E(X) = n * p = 10 * 0.0228 = 0.228
$$

> Por lo anterior se concluye que $0.228$ aviones llegarían con retrasos de más de $20$ minutos de los $10$ que llegan en un día. Usando una aserción logica, no se puede tener $0.228$ partes de un avión (A no ser que este estrellado), por lo cual se puede afirmar que no llegarían aviones con un retraso de más de $20$ minutos