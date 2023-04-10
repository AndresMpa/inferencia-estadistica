# Ejemplo ANOVA

| Pintura 1 | Pintura 2 | Pintura 3 | Pintura 4 |
| --------- | --------- | --------- | --------- |
| 124       | 144       | 133       | 150       |
| 127       | 141       | 143       | 142       |
| 135       | 143       | 137       | 135       |
| 124       | 139       | 136       | 140       |
| 131       | 135       | 131       | 153       |

Probar la hipotesis que si el tiempo de secado depende del tipo de pintura. Usar un $\alpha$ del $5\%$

## Solución

$\bar{X}_p1 = \frac{124+127+135+124+131}{5}$
$\bar{X}_p1 = 128.2$

$\bar{X}_p2 = \frac{144+141+143+139+135}{5}$
$\bar{X}_p2 = 140.4$

$\bar{X}_p3 = \frac{133+143+137+136+131}{5}$
$\bar{X}_p3 = 136$

$\bar{X}_p4 = \frac{150+142+135+140+153}{5}$
$\bar{X}_p4 = 144$

$\bar{\bar{X}} = \frac{128.2+140.2+136+144}{5}$
$\bar{\bar{X}} = 137.15$

Ahora para calcular el $sctr$

$$sctr = \sum_{j=1}^k(n_j) * (\bar{x}_j - \bar{\bar{x}})^2$$

$sctr = 5*[(128.2 - 137.15)^2 + (140.4 - 137.15)^2 + (136 - 137.15)^2 + (144 - 137.15)^2]$

$sctr = 694.55$

$cmtr = \frac{694.55}{3}$

$cmtr = 231.56$

$sce = 4 * [22.7+12.8+21+54.5]$

$sce = 444$

$cme = \frac{444}{11}$

$cme = 27.95$

1. Hipotesis

$H_0: \mu_i = \mu_j$
$H_1: \mu_i \neq \mu_j$

2. Certeza:

$0.05$

3. Valor F

$F = \frac{231.5166}{8.343}$

4. Si $F_{calculado} \gt F_{critico}$

$F_{critico} = F(0.05; 3; 16) = 3.2389$

$8.346 \gt 3.2389$

5. Conclusión

$R.H_0$. Por tanto con un nivelde confianza del 95% podemos concluir que si existe diferencia en los tiempos de secado con respectoma la pintura

## Tabla nova

| Fuente       | suma de cuadrados | Grados de libertad | Cuadrados medios | Estadistico F                | F crititco | Valor P |
| ------------ | ----------------- | ------------------ | ---------------- | ---------------------------- | ---------- | ------- |
| Tratamientos | 694.55            | 3                  | 231.5166         | $F = \frac{231.5166}{27.75}$ | 3.2389     | 0.01442 |
| Error        | 444               | 16                 | 27.75            |                              |            |         |
| Total        | 1138.55           | 19                 |                  |                              |            |         |

$S = \sqrt{cme}$
$S = \sqrt{5.2678}$

$t_\frac{\alpha}{2} = t(0.025; 16) = 2.1199$