# Diferencia de proporciones

## Diferencia de proporción poblacional

$$
\epsilon(\hat{P}_1 - \hat{P}_2)
$$

Donde $\epsilon$ es el valor esperado

$$
\sigma_{\hat{P}_1 - \hat{P}_2} = \sqrt{\frac{P_1Q_1}{n_1} + \frac{P_2Q_2}{n_2}}
$$

$$
Z = \frac{(\hat{P}_1 - \hat{P}_2) - (P_1 - P_2)}{\sqrt{\frac{P_1Q_1}{n_1} + \frac{P_2Q_2}{n_2}}}
$$

### Ejemplo

Un tratamiento para el refriado se probó en una población de 300 personas de las cuales 270 respondiendo positivamente. Otro medicamento distinto se probo a en una población de 400 personas de las cuales 350 respondieron positivamente.

- Calcular la probabilidad que exista una diferecia de 0.03 a favor del tratamiento 1

- Calcular la probabilidad que exista una diferencia de 0.03 a favor del tratamiento 2

### Solución

$P_1 = \frac{270}{300} = 0.9$

$P_2 = \frac{350}{400} = 0.875$

La diferencia entre los 2 es de $0.025$

---

$$
P(\hat{P}_1 - \hat{P}_2 \geq 0.03)
$$

$$
Z = \frac{0.03 - 0.025}{\sqrt{\frac{0.9*0.1}{300} + \frac{0.875*0.125}{400}}}
$$

$Z = 0.2087$

$1 - P(Z \leq 0.2087)$
$1 - 0.58265878$
$0.41734122$

---

$$
P(\hat{P}_2 - \hat{P}_1 \geq 0.03)
$$

$$
Z = \frac{0.03 - (0.875 - 0.9)}{\sqrt{\frac{0.9*0.1}{300} + \frac{0.875*0.125}{400}}}
$$

$Z = 2.29677781304$

$1 - P(Z \leq 2.29677781304)$

$1 - 0.989184276$

$0.010815724$

## Pruebas de hipotesis

- Pruebas para una media
- Pruebas para una diferencia de medias
- Pruebas para una proporción
- Prueba para una diferencia de proporciones

### Prueba de hipotesis

Es un procedimiento estadistico que nos permite a permite a partir de una muestra, generalizar los resultados para una población

### Pasos para una prueba de hipotesis

1. Establecer las hispotesis nula y alternativa

2. Fijar el nivel de significancia

3. Calcular el estadistico de prueba de pendiendo del tipo de hipotesis

4. Fijar dos puntos criticos

5. Concluir de acuerdo a las resultados

### Ejemplo

Se quiere probar si el rendimiento de un nuevo motor, es superior a $24 km/lt$ (Kilometros por litro), se toma una muestra de 40 automatas que nos dio como resultado una media de $25.2 km$ con una desviación, de $1.5 km$. Con estos datos se puede concluir que el rendimiento del nuevo motor es superior al valor afirmado use un $\alpha$ del $5\%$

Siempre que se habla de hipostesis se plantea:

- Hipotesis nula (Igualdad); esta puede ser menor igual $\leq$

- Hipotesis alternativa (Desigualdad); este es estrictamente mayor $\gt$

Luego se busca el parametro de una poblacion, es el parametro mediante el cual se puede acceder a toda la población $24 km/lt$; este parametro es un valor que no cambia cambia ni el tiempo ni en lugar.

$\mu$ será la media de la población

Y se quiere saber basicamente si esta media cambiará o no

$S$ será una muestra que se toma de la población

### Solución

1. Se plantean las hispotesis

- Hipotesis nula:

$H_0: \mu \leq 24$

- Hipotesis alternativa:

$H_1: \mu \gt 24$

---

2. Se determina el nivel de significacia: Este venía en el problema

$\alpha = 0.05$

---

3. Se calcula el valor de z

$$
Z = \frac{\bar{x}-\mu}{\frac{s}{\sqrt{n}}}
$$

$$
Z = \frac{25.2 - 24}{\frac{1.5}{\sqrt{40}}}
$$

$Z = 5.059644256$

---

4. Con este valor se puede concretar las afirmaciones anteriores

$Z_{calculado}$ el Z que se calcula

$Z_{critico}$ es el Z que surge de la tabla

Si $Z_{calculado}$ es $\gt$ $Z_{critico}$ R $H_0$

$5.059644256 \gt 1.645$ R $H_0$

---

5. Concluir

> Con una confianza del 95% podemos concluir que el rendimiento del nuevo motor es mayor a $24 km/lt$

### Intervalo de confianza

$\mu = \bar{x} \pm (\frac{Z_{\frac{\alpha}{2}}}{2} * \frac{s}{\sqrt{n}})$

$\alpha = 0.05$

$\frac{\alpha}{2} = 0.025$

$z_\frac{\alpha}{2} = Z0.025 = -1.96$

$z_{1 - \frac{\alpha}{2}} = Z0.975 = 1.96$

$\mu = 25.2 \pm (1.96 * frac{1.5}{\sqrt{40}})$

$\mu = 25.2 \pm 0.4648$

$\mu = (24.535; 25.4648) \rightarrow$ Intervalor para el parametro poblacional

$\mu$ no contiene a $24 km/lt$ R $H_0$

---

### Ejemplo

Un inspector de calidad vista una planta de empacado para verificar que el peso del articulo sea el indicado en la etiqueta. La empresa asegura que el contenido de cada caja es de $750g$ (Gramos), con una desviación estandar de $5g$. Se seleccionan $100$ cajas al azar y el resultado fue de $748g$. Con estos resultados y usando un $\alpha$ del $5\%$ podemos concluir que el articulo se esta llenando por debajo de lo incluido en la etiqueta.

1. Se plantea la hipotesis

$H_0: \mu \geq 750$

$H_1: \mu \lt 750$

Nota: $H_1$ siempre lleva el peso de la prueba

2. Se determina el nivel de confianza

$\alpha: 0.05$

3. Se calcula la probabilidad

$Z = \frac{748 - 750}{\frac{5}{\sqrt{100}}}$

$Z = -4$

4. Afirmaciones con el Z

$Z_{calculado} = -4$

Este valor se calcula con la inversa de $\alpha$

```
=DISTR.NORM.ESTAND.INV(0,05)
```

$Z_{critico} = -1.644853627$

Si $Z_{calculado}$ es $\lt$ $Z_{critico}$ R $H_0$

$-4 \lt -1.645$

5. Conclusión

Con una confinanza del $95\%$ podemos concluir que el contenido es menor a $750g$

### Intervalo de confianza

$\mu = 750 \pm (\frac{1.96 * 5}{100})$

$\mu = 748 \pm 0.98$

$\mu = (748.02 ; 748.98)$

El intervalo no contiene el promedio $\mu = 750$, por lo tanto se rechaza $H_0$

---

### Ejemplo
Se quiere probar si existe discriminación salarial en cuanto al valor devengando hombres y mujeres, una muestra de hombres y mujeres con más de 5 años de experiencia entregó los siguientes resultados:

| Hombres            | Mujeres            |
| ------------------ | ------------------ |
| $n_1 = 44$         | $n_2 = 32$         |
| $\bar{x}_1 = 9.25$ | $\bar{x}_2 = 8.90$ |
| $S_1 = 1.00$       | $S_2 = 0.8$        |

Usando un $\alpha$ de $5\%$ podemos decir que existe diferencia en cuanto al valor devegado

### Solución

> 1 serán los hombres y 2 serán las mujeres

$$
H_0: \mu_1 - \mu_2 = 0
$$

$$
H_1: \mu_1 - \mu_2 \neq 0
$$

$\alpha = 0.05$

$$
Z = \frac{(\bar{x}_1 - \bar{x}_2) - (\mu_1 - \mu_2)}{\sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}}
$$

Pero $\mu_1 - \mu_2 = 0$

$$
Z = \frac{(\bar{x}_1 - \bar{x}_2) - 0}{\sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}}
$$

$$
Z = \frac{(\bar{x}_1 - \bar{x}_2)}{\sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}}
$$

Usando esta formula:


$$
Z = \frac{(9.25 - 8.90)}{\sqrt{\frac{1^2}{44} + \frac{0.8^2}{32}}}
$$

$Z = 1.693$

---

Si $Z_{calculado} \lt Z_{critico}$ o $Z_{calculado} \gt Z_{critico}$ R $H_0$

$1.93 \gt 1.96 \rightarrow$ Esto es falso, por tanto se rechaza $H_0$

---

Por tanto se concluye que no existe suficiente evidencia estadistica para rechazar $H_0$. Por lo tanto no se puede decir exista diferencia entre ambos salarios