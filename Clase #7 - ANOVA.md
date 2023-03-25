# Análisis de varianza (ANOVA)

Es una tecnica que permite comprar más de 2 medias, en este caso más de 2 poblaciones, donde

$H_0: \mu_1 \geq \mu_2$
$H_1: \mu_1 \lt \mu_2$ Izquierda

$H_0: \mu_1 \leq \mu_2$
$H_1: \mu_1 \gt \mu_2$ Derecha

## Prueba de hipotesis

$H_0: \mu_1 = \mu_2 = \mu_3 = \mu_4 = ... = \mu_n$
$H_1: \mu_1 \neq \mu_2 \neq \mu_3 \neq \mu_4 \neq ... \neq \mu_n$

$H_0: \mu_i = \mu_j$ Estadisticamente iguales
$H_1: \mu_i \neq \mu_j$ Estadisticamente diferentes

Para hacer esto se puede usar:

- Anova de un factor completamente aleatorio en Excel o SPSS

- Anova por bloques en: SPSS

El analisis de varianza sirve para comparar varios grupos en una variable cuantitiva, la cual está dividida en varios tratamientos que evalúan la variable de interes

> Esto sirve para hacer pruebas de hipotesis, pero no puede decir cual es mayor que cual, solo dice si hay o no una diferencia

## Supuestos del anova

- Las poblaciones (Distribuciones de probabilidad de la variable dependiente correspondiente a cada factor), son normales.

- Las $k$ muestras sobre las que se aplican son independientes.

- Las poblaciones tiene todas igual varianza (homoscedasticidad).

### Formualas para los tratamientos

Donde:

- $sctr$ suma de cuadrados de los tratamientos
- $n_j$ tamaño de muestra del tratamiento $j$
- $x_j$ es media del tratamiento $j$
- $\bar{\bar{x}}$ es la media de todos los datos/observaciones
- $cmtr$ cuadrado medio de los tratamientos
- $k$ número de tratamientos
- $\bar{x}$ es la media del tratamiento
- $sce$ suma del cuadrado del error
- $cme$ cuadrado medio del error
- $s_j^2$ varianza del tratamiento $j$
- $n_T$ número total de observacuines
- $F$ distribución de probabilidad de $F$ de ficha

$$sctr = \sum_{j=1}^k(n_j) * (\bar{x}_j - \bar{\bar{x}})^2$$

$$cmtr = \frac{sctr}{k-1}$$

$$\bar{x}=\sum_{i=1}^j(\frac{x_{i1} + x_{i2} + ... + x_{ij}}{n_i})$$

$$sce = \sum_{j=1}^k(n_j-1)*S_j^2$$

$$cme = \frac{sce}{n_T-k}$$

$$F = \frac{cmtr}{cme}$$

## Ejemplo propuesto

- Para estudiar el efecto de la temperatura en el rendimiento de un proceso quimico, se produjeron 5 lotes con cada uno de los 3 tratamientos. Los resultados se presentan a continuación-

- De la tabla para el analisis de varianza. Use un alfa del 5% para probar si la temperatura afecta el rendimiento del proceso

| 50°C | 60°C | 70°C |
| ---- | ---- | ---- |
| 34   | 30   | 23   |
| 24   | 31   | 28   |
| 36   | 34   | 28   |
| 39   | 23   | 30   |
| 32   | 27   | 31   |

Hagamos el primer calculo a mano, luego en excel y finalmente calculamos todo con excel

Para calcula la media de 50°C podemos sumar los valores y dividir entre el número de valores:

$\bar{x}_{50} = \frac{34+24+36+29+32}{5}$

$\bar{x}_{50} = 33$

Ahora para calcular la varianza

$S_{50}^2=\frac{(34-33)^2+(24-33)^2+(36-33)^2+(29-33)^2+(32-33)^2}{5}$

$S_{50}^2=\frac{1+81+9+36+1}{5}$

$S_{50}^2=\frac{128}{5}$

$S_{50}^2=25.6$

> VAR.P divide sobre n mientras que VAR.S divide sobre n-1

Confirmamos con

```
VAR.P(33)
```

En valor con la función nos da 25.6

Ahora calculamos los demás con excel

| Medida   | 50°C | 60°C | 70°C |
| -------- | ---- | ---- | ---- |
| Media    | 33   | 29   | 28   |
| Varianza | 25.6 | 14   | 7.6  |

1. Plantenado las hipotesis:

$H_0: \mu_1 = \mu_2 = \mu_3$

$H_1: \mu_1 \neq \mu_2 \neq \mu_3$

2. Planteamos el alpa:

$\alpha = 0.05$

Ahora calculamos la media de medias:

> Este es el promedio de las medias

$\bar{\bar{x}} = 30$

Ahora calculamos el sctr:

$$sctr = \sum_{j=1}^k(n_j) * (\bar{x}_j - \bar{\bar{x}})^2$$

$sctr = 5*(33-30)^25*(29-30)^2+5*(28-30)^2$

$sctr = 48+5+20$

$sctr = 70$

Ahora calculamos el sce:

$$sce = \sum_{j=1}^k(n_j-1)*S_j^2$$

$sce = 4*25.6+4+14+4*7.6$

$sce = 102.4 + 56 + 30.4$

$sce = 188.8$

3. Calculamos el estadistico de prueba:

Para calcular el $F_{critico}$

```
INV.F.CD(alpha, 2, 12)
```

$cmtr = \frac{70}{3-1} = 35$

$cme = \frac{188.8}{12} = 15.73$

$F = \frac{35}{15.73} = 2.22$

$F_{calculado} > F_{critico}$

$F_{critico} = F(2.22, 0.05) = 3.89$

$2.22 > 3.89$ No apruebo la hipotesis $H_0$

## Intervalo de confianza

Donde:

- $t$ de student; para calcular el valor de t se puede usar
```
DISTR.T.INV(2 * alpha; valor)
```
- $S$ desviación de la varianza del error

$$\mu = \bar{x}_i \pm t_{\frac{\alpha}{2}} * \frac{S}{\sqrt{n_j}}$$

$$S = \sqrt{cme}$$

## Retomando el ejemplo anterior

Intervalor para 50°C se puede calcula con:

$$\mu = \bar{x}_i \pm t_{\frac{\alpha}{2}} * \frac{S}{\sqrt{n_j}}$$


Primero calculamos la $S$

$$S = \sqrt{cme}$$

$S = \sqrt{15.73}$

$S = 3.97$

Para calcular el $t_{\frac{\alpha}{2}}$

$t_{\frac{\alpha}{2}} = 2.17884$

El intervalor para 50°C será: $33 \pm 2.17884 * (\frac{3.97}{\sqrt{5}})$

Con esto podemos calcular todos los demás intervalos

---

El intervalor °50C: $33 \pm 3.8649$

El intervalo °50C = $(29.1351 ; 36.8649)$

---

El intervalor °60C: $29 \pm 3.8649$

El intervalo °60C = $(25.1351 ; 32.8649)$

---

El intervalor °70C: $28 \pm 3.8649$

El intervalo °70C = $(24.1351 ; 31.8649)$

> Si el valor resultante es menor que alpha la hipotesis nula se rechaza