#Distribuciones muestrales para la diferencia de medias y propociones

---

No necesariamente ambas poblaciones deben ser iguales, ni ambos tamaños de muestra deben ser iguales

El estimador puntual

$\bar{x}_1 - \bar{x}_2$

Y debe cumplirse el teorema central del limite, o sea:

$\epsilon(\bar{x}_1 - \bar{x}_2 = \mu_1 - \mu_2)$

Y

$\sigma_{\bar{x}_1 - \bar{x}_2} = \sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}$

$Z = \frac{(\bar{x}_1 - \bar{x}_2) - \epsilon(\bar{x}_1 - \bar{x}_2)}{\sigma_{\bar{x}_1 - \bar{x}_2}}$

$Z = \frac{(\bar{x}_1 - \bar{x}_2) - \mu_1 - \mu_2}{\sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}}$

###Ejemplo:

1. En una poblacion A, la media poblaciones es de $30.5$ con una desviación de $5.4$; en una población B la media poblacional es $29.4$ con una varianza de $28.6$. Se pide:

   - Calcular la probabilidad de que al tomar una muestra de $40$ elementos de la población $1$ y una muestra de $50$ de la población $2$; esta sea mayor o igual a $1$ a favor de la población A.

   - Calcular la probabilidad de que la diferencia entre ambas no sobrepase $1.5$ unidades a favor de la población B

###Solución:

#####Datos:

$\mu_A = 30.5$

$n_A = 40$

$\sigma_A = 5.4$

$\mu_B = 29.4$

$n_B = 50$

$\sigma_B = 28.6$

Calcular la probabilidad de que al tomar una muestra de $40$ elementos de la población $1$ y una muestra de $50$ de la población $2$; esta sea mayor o igual a $1$ a favor de la población A.

$x_1 \geq x_2 + 1$

$P(\bar{x}_1 - \bar{x}_2 \geq 1)$

$z = \frac{1 - (30.5 - 29.4)}{\sqrt{\frac{5.4^2}{40} + \frac{28.6}{50}}}$

$z = -0.08767208838$

$P(z \geq  -0.08767208838)$

$1 - P(z \geq  -0.08767208838)$

$P(1 - 0.465068652)$

$P = 0.53650$

> Por tanto la probabilidad de que sea mayor o igual a $1$ a favor de la población A será de $53.65\%$

Calcular la probabilidad de que la diferencia entre ambas no sobrepase $1.5$ unidades a favor de la población B

$P(x_2 - x_1 \leq 1.5)$

$z = \frac{1.5 - (29.4 - 30.5)}{\sqrt{\frac{28.6}{50} + \frac{5.4^2}{40}}}$

$z = 2.367146386$

$P(z \geq 2.279474298)$

$P = 0.988680557$

Por tanto la probabilidad sería de $98.87\%$

$z = \frac{(\hat{p}_1 - \hat{p}_2) - (p_1 - p_2)}{\sqrt{\frac{p_1 * q_1}{n_1} + \frac{p_2 * q_2}{n_2}}}$

2. Un especialista en genética ha detectado que el $26\%$ de los hombres y el $24\%$ de las mujeres de cierta región del país tiene un leve desorden sanguíneo; si se toman muestras de $150$ hombres y $150$ mujeres, determine la probabilidad de que la diferencia muestral de proporciones que tienen ese leve desorden sanguíneo sea de:

   - Menos de $0.035$ a favor de los hombres.
   - Entre $0.01$ y $0.04$ a favor de los hombres.

#####Datos:

$P_{hombres} = 0.26$
$Q_{hombres} = 0.74$
$n_{hombres} = 150$

$P_{mujeres} = 0.24$
$Q_{mujeres} = 0.76$
$n_{mujeres} = 150$

Menos de $0.035$ a favor de los hombres.

$P(\hat{p}_{hombres} - \hat{p}_{mujeres} \leq 0.035)$

$z = \frac{(\hat{p}_{hombres} - \hat{p}_{mujeres}) - (p_{hombres} - p_{mujeres})}{\sqrt{\frac{p_{hombres} * q_{hombres}}{n_{hombres}} + \frac{p_{mujeres} * q_{mujeres}}{n_{mujeres}}}}$

$z = \frac{0.035 - (0.26 - 0.24)}{\sqrt{\frac{0.26 * 0.74}{150} + \frac{0.24 * 0.76}{150}}}$

$z = 0.3$

$P(\hat{P}_{hombres} - \hat{P}_{mujeres} \leq 0.035)$

$P(z \leq 0.3)$

$P = 0.6179$

Por tanto la probabilidad es de $61.79$

Entre $0.01$ y $0.04$ a favor de los hombres.

$P(0.01 \leq \hat{p}_{hombres} - \hat{p}_{mujeres} \leq 0.04)$

$z = \frac{(\hat{p}_{hombres} - \hat{p}_{mujeres}) - (p_{hombres} - p_{mujeres})}{\sqrt{\frac{p_{hombres} * q_{hombres}}{n_{hombres}} + \frac{p_{mujeres} * q_{mujeres}}{n_{mujeres}}}}$

$z_1 = \frac{0.04 - (0.26 - 0.24)}{\sqrt{\frac{0.26 * 0.74}{150} + \frac{0.24 * 0.76}{150}}}$

$z_1 = \frac{0.02}{\sqrt{0.0358 + 0.03487}}$

$z_1 = 0.075223370503$

$z_2 = \frac{0.01 - (0.26 - 0.24)}{\sqrt{\frac{0.26 * 0.74}{150} + \frac{0.24 * 0.76}{150}}}$

$z_2 = \frac{-0.01}{0.04998666489}$

$z_2 = -0.2000533547$

