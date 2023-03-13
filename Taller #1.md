<p align="center">
Ejercicios de Distribuciones Muestrales
</p><p align="center">
Marzo 10 de 2023
</p>

1. Según un estudio realizado por una empresa hotelera durante un año, la distribución del tiempo de estancia de cada viajero fue normal con una media de $3.7$ días y una desviación típica de $0.75$ días.

a. A lo largo del año 2022 se analizó el tiempo de estancia y se quiere determinar ¿Cuál es la probabilidad que un turista se quede más de 3,5 días en una muestra de 49 viajeros elegidos al azar?

$μ = 3.7$

$σ = 0.75$

$x_{barra} = 3.5$

$n = 49$

Para calcular la probabilidad $z$ se usa:

$z = \frac{x_{barra} - μ}{\frac{σ}{\sqrt{n}}}$

Por tanto:

$z = \frac{3.5 - 3.7}{\frac{0.75}{\sqrt{49}}}$

Simplificando la expresión interna:

$\frac{0.75}{\sqrt{49}} = \frac{0.75}{7}$

Reemplanzando la expresión:

$z = \frac{3.5 - 3.7}{\frac{0.75}{7}}$

Restando $3.5 - 3.7$ y efectuando $\frac{0.75}{\sqrt{49}}$:

$z = \frac{-0.2}{0.1071}$

Por tanto:

$z \approx -1.866$

$P(z >= 3,5) = 1 - 0,031020683$

$P(z >= 3,5) = 0,968979317$

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

$n = (\frac{z*σ}{ε})^2$

$n = (\frac{-2.33 * 0.75}{0.25})^2$

$n = \frac{-2.33^2 * 0.75^2}{0.25^2} \approx 51.87$

> Por tanto, la muestra debe ser de tamaño $52$ aproximadamente

2. El Instituto de Mercadotecnia de Alimentos de un país indica que el $17\%$ de las familias gastan más de $450000$ pesos por mes en alimentación. Se sabe que la proporción poblacional es $P=0.17$, si se selecciona una muestra aleatoria de $800$ familias.

¿Cuál es la probabilidad que la proporción muestral este $± 0,02$ de la proporción poblacional?

$n = 800$

$P = 0.17$

Ya que $P = 0.17$ entonces

$Q = 0.83$

$ε = 0.02$

$P_{gorrito} = 0.17$

Ya que el error $ε$ será de 0.02, se puede afirmar que:

$P_{gorrito_{1}} = P_{gorrito} - ε$

$P_{gorrito_{1}} = 0.15$

$P_{gorrito_{2}} = P_{gorrito} + ε$

$P_{gorrito_{2}} = 0.19$

Para calcular la probabilidad $Z$ podemos usar la formula

$Z = \frac{P_{gorrito} - P}{\sqrt{\frac{P * Q}{n}}}$

Por tanto se deberá de calcular:

$Z_{1} = \frac{P_{gorrito_{1}} - 0.17}{\sqrt{\frac{0.17 * 0.83}{800}}}$

$Z_{1} = \frac{0.15 - 0.17}{\sqrt{\frac{0.17 * 0.83}{800}}}$

$Z_{1} = -1.505953223$

$Z_{2} = \frac{P_{gorrito_{2}} - 0.17}{\sqrt{\frac{0.17 * 0.83}{800}}}$

$Z_{2} = \frac{0.19 - 0.17}{\sqrt{\frac{0.17 * 0.83}{800}}}$

$Z_{2} = 1.505953223$

Por ende parar calcular la probabilidad se puede decir que, la probabilidad de que la proporción muestral este $± 0,02$ de la proporción poblacional será

$P(P_{gorrito_{1}} ≤ P_{gorrito} ≤ P_{gorrito_{2}})$

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

$P(P_{gorrito} \gt 0.22) = ?$

$n = 800$

$P = 0.17$

Ya que $P = 0.17$ entonces

$Q = 0.83$

$P_{gorrito} = 0.22$

Para ello se puede usar la formula

$Z = \frac{P_{gorrito} - P}{\sqrt{\frac{P * Q}{n}}}$

$Z = \frac{0.22 - 0.17}{\sqrt{\frac{0.17 * 0.83}{800}}}$

$Z = 3.764883057$

Por tanto, la probabilidad de que la proporción muestral de p sea de más de $0.22$, será equivalente a

$P(P_{gorrito} \gt 0.22) = P(Z \gt 3.764883057)$

Ya que se busca la probabilidad de que sea "de más de $0.22$", esto se representa como la diferencia entre el total y la probabilidad de $0.22$

$P = 1 - P(Z \gt 3.764883057)$

```
=DISTR.NORM.ESTAND(3.764883057)
```

$P \approx 1 - 0.9999$

$P \approx 0.0001$

> Por tanto la probabilidad de que la probabilidad que la proporción muestral de p sea de más de $0.22$ es de $0.001%$

3. Los datos sobre el perfil de la audiencia del sitio de la Red ESPN indicaron que el $31\%$ de los usuarios son mujeres. Suponga que este porcentaje se basó en una muestra de $600$ usuarios.

a. Que probabilidad hay de encontrar de que la proporción muestral este a $± 0.025$ de la proporción poblacional

b. Que probabilidad hay que que al tomar una muestra de $210$ mujeres ellas mujeres escuchen Red ESPN

c. Que tamaño debe tener la muestra para que el margen de error sea del $4\%$ con una confianza del $98\%$

4. Las estaturas de $1000$ estudiantes están distribuidas aproximadamente en forma normal con una media de $174.5$ centímetros y una desviación estándar de $6.9$ centímetros. Si se extrae una muestra aleatoria de tamaño $50$ de esta población, determine:

a. ¿Cuál es la probabilidad que un alumno tenga una estatura entre $172.5$ y $175.8$ centímetros?

b. ¿Cuál es la probabilidad que un alumno tenga una estatura por debajo de $172$ centímetros?

c. Si se quiere una diferencia de un $80$ mms con respecto a la media poblacional de que tamaño debe ser la muestra, si se quiere una confianza del $98\%$

5. Una compañía aérea sabe que en promedio sus aviones tienen retrasos que siguen una distribución normal con media de $10$ minutos y desviación estándar de $5$ minutos. Determinar:

a. La probabilidad que en una muestra de $15$ aviones, un avión llegue con no más de $10$ minutos de retraso

b. La probabilidad que en una muestra de $15$ aviones, un avión tenga un retraso de más de $15$ minutos

c. Si en un día llegan $10$ aviones de esa compañía al aeropuerto de la ciudad, cuantos llegaran con retrasos de más de $20$ minutos?
