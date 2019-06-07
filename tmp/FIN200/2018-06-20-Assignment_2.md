---
layout: post
title:  "Assignment_2 Finance"
date:   2018-06-20 20:32:51 +0100
authors: Ty_Yiu
categories: FIN200 Uni 
---

### Business Statistics 

<div style="page-break-after: always;"></div>

## 8.57

### a)

| $\text{mean} _{\text{standard error}}$ | 1.195 |
| -------------------------------------- | ----- |
| $\circ_{\text{of freedom}}$            | 69    |
| $t_{value}$                            | 2.649 |
| Margin of error                        | 3.166 |
| $\text{limit}_{\text{upper}}$          | 48.17 |
| $\text{limit}_{\text{lower}}$          | 41.83 |

### b)

| $\hat{p}$                                   | 0.514  |
| ------------------------------------------- | ------ |
| $Z_{\text{value}}$                          | -1.96  |
| $\text{proportion}_{\text{standard error}}$ | 0.0597 |
| Margin of error                             | 0.1171 |
| $\text{limit}_{\text{upper}}$               | 0.3972 |
| $\text{limit}_{\text{lower}}$               | 0.6314 |

## 8.61

### a)

$$
\bar{X}\pm t * \frac{S}{\sqrt{n}}=21.34\pm1.995*\frac{9.22}{\sqrt{70}} 
$$

$$
\text{Inequality} = 19.14 \leq \alpha \leq 23.54
$$

### b)

$$
p \pm Z * \sqrt{\frac{p*(1-p)}{n}}= 0.3714\pm1.645*\sqrt{\frac{0.3714*(0.6286)}{70}}
$$

$$
\text{Inequality} = 0.2764 \leq \pi \leq 0.4664
$$

### c)

$$
n= \frac{Z^2*S^2}{e^2}=\frac{1.96^2*10^2}{1.5^2}=170.74 \approx 171
$$

### d)

$$
n= \frac{Z^2*\pi*(1-\pi)}{e^2}= \frac{1.645^2*0.5*(1-0.5)}{0.045^2}=334.08 \approx 334
$$

### e)

It should be chosen the larger sample (always consider outliers etc. for general scale), especially when intentionally multi-purposing a sample. 

## 8.65

### a)

$$
\bar{X}\pm t*\frac{S}{\sqrt{n}}=5.501\pm 2.68*\frac{0.106}{\sqrt{50}}
$$

$$
\text{Inequality} = 5.46 \leq \mu \leq 5.54
$$

### b)

5.5 grams is inside the 99% confidence interval and thus the mean tea bag weight can be claimed to be mean 5.5 grams.

### c)

A normal distribution of the weight of tea bags validates the assumption.

## 9.69

### a)

$$
H_0 : \pi = 0.5 \text{, thus } H_1 : \pi  \neq 0.5
$$

### b)

The probability of creating a Type $I$ error, is equal to the level of significance. Specifically, the web page visitors that prefer the new design over the old design could be deducted to be other than half, thus a type $I$ error.

A type $II$ error on the contrary describes accepting and relying on data which should not be relied upon. Specifically, the web page visitors may be far off half the sample, but it is persisted upon half probability.

### c)

The null hypothesis rejection in consideration of the $P$ value of 0.2, describes that there is a 20% probability of incorrectly concluding that the sample is not half.

### d)

Incorrect conclusions about half of the sample are significant and is thus a argument for a higher $\alpha$.

### e)

Raising $\alpha$ should be stimulating to re-evaluate the probability of making type $I$ errors.

### f)

When $P=0.12$ rejecting the null hypothesis should be considered. When $P=0.06$ most type $I$ error occurrence probabilities diminish.

## 9.73

### a)

$$
H_0 : \alpha \geq 100 \text{, thus }H_1:\alpha < 100
$$

If ($t_{Stat} < (-1.6657)$){	reject $H_0$	}
$$
t_{Stat} = \frac{\bar{X}-\mu}{\frac{S}{\sqrt{n}}} = \frac{93.7-100}{\frac{34.55}{\sqrt{75}}}=(-1.579)
$$
Since $t_{Stat}:(-1.579) > t_{\text{critical bound}} :(-1.6657)$	{	do not reject $H_0$	}

### b)

$H_0:\pi < 0.1$, thus at most 10 percent are incorrect.

$H_1:\pi > 0.1$, thus more than 10 percent are incorrect.

Thus, if ($Z_{Stat} > (1.645)$) {	reject $H_0$	}
$$
Z_{Stat}= \frac{p -\pi}{\sqrt{\frac{\pi*(1-\pi)}{n}}}= \frac{0.16-0.1}{\sqrt{\frac{0.1*(1-0.1)}{75}}}=1.73
$$
Since $Z_{Stat} :(1.73) $ > $ Z_{\text{critical bound}} : (1.645)$ {	reject $H_0$ 	}

### c)

You must assume a normal distributed random data set for the use of a t-test on population mean.

### d)

$H_0:\alpha \geq 100$, thus reimbursement is at least 100.

$H_1:\alpha < 100$, thus reimbursement is less than 100.

Thus, if ($t_{Stat} < (-1.6657)$)	{	reject $H_0$	}
$$
t_{Stat} = \frac{\bar{X}-\mu}{\frac{S}{\sqrt{n}}} = \frac{90-100}{\frac{34.55}{\sqrt{75}}}=-2.5066 \approx (-2.5)
$$
Since $t_{Stat} : (-2.5) < t_{\text{critical bound}}:(-1.6657)$	{	reject $H_0$ 	}

### e)

$H_0:\pi < 0.1$, thus at most 10 percent are incorrect.

$H_1:\pi > 0.1$, thus more than 10 percent are incorrect.

Thus, if ($Z_{Stat} > (1.645)$) {		reject $H_0$		}
$$
Z_{Stat}= \frac{p -\pi}{\sqrt{\frac{\pi*(1-\pi)}{n}}}= \frac{0.2-0.1}{\sqrt{\frac{0.1*(1-0.1)}{75}}}=2.89
$$
Since $Z_{Stat} :(2.89) $ > $ Z_{\text{critical bound}} : (1.645)$ {	reject $H_0$ 	}

## 10.77

### a)

If ($H_0:\ _1S^2 = \ _2S^2$) {	Population variances are equal	}

> $F_{Stat}$ = test for differences in variance

| Level of significance                             | 0.5     |
| ------------------------------------------------- | ------- |
| $\text{sample}S_1$                               | 20      |
| $\text{sample}\sigma_{\text{1}}$                 | 5.714   |
| $\text{sample}S_2$                               | 38      |
| $\text{sample}\sigma_{\text{1}}$                 | 5.406   |
| $\text{population 1} \circ_{\text{ of freedom}}$ | 19      |
| $\text{population 2} \circ_{\text{ of freedom}}$ | 37      |
| Upper critical value                              | 2.11685 |
| p                                                 | 0.749   |



If ($F_{Stat} > 2.1169$)	{	reject $H_0$		} 
$$
F_{Stat}= \frac{_1S^2}{_2S^2} = \frac{(5.7144)^2}{(5.4064)^2}= 1.1172 \approx 1.12
$$
Since $F_{Stat} :(1.12) $ < $ Z_{\text{ upper critical bound}} : (2.1169)$ {	do not reject $H_0$ 	}

### b)

Since there is no significant difference in the variances, use the *pooled variance test*

### c)

($H_0:\ \mu_1 = \mu_2$) ($H_1 : \ \alpha_1 \neq \alpha_2$)

| Level of significance                             | 0.05            |
| ------------------------------------------------- | --------------- |
| $\text{sample}S_1$                               | 20              |
| $\text{sample}\sigma_{\text{1}}$                 | 5.714           |
| $\text{sample}\mu_{\text{1}}$                    | 16.625          |
| $\text{sample}S_2$                               | 38              |
| $\text{sample}\sigma_{\text{1}}$                 | 5.406           |
| $\text{sample}\mu_{\text{2}}$                    | 11.026          |
| Upper critical value                              | 2.00324         |
| Lower critical value                              | (-2.00324)      |
| P                                                 | 0.000532        |
| $\text{population 1} \circ_{\text{ of freedom}}$ | 19              |
| $\text{population 2} \circ_{\text{ of freedom}}$ | 37              |
| $\sigma^2_{pooled}$                               | 30.391          |
| $\mu_2-\mu_1$                                     | $\approx$ 5.599 |
| $t_{Stat}$                                        | 3.676           |



If ($t_{Stat} < (-2.0032)$)	{	reject $H_0$		} 

Else If ($t_{Stat} > 2.0032$)	{	reject $H_0$		} 

Since $t_{Stat} :(3.676) $ > $ t_{\text{ upper critical bound}} : (2.00324)$ {		reject $H_0$ 	}

## 10.81

### a)

If ($H_0:\ _1S^2 = \ _2S^2$) {	Population variances are equal	}

| Level of significance                             | 0.05   |
| ------------------------------------------------- | ------ |
| $_\text{sample}S_1$                               | 500    |
| $_\text{sample}\sigma_{\text{1}}^2$               | 22500  |
| $_\text{sample}S_2$                               | 500    |
| $_\text{sample}\sigma_{\text{1}}^2$               | 6400   |
| $_\text{population 1} \circ_{\text{ of freedom}}$ | 499    |
| $_\text{population 2} \circ_{\text{ of freedom}}$ | 499    |
| Upper critical value                              | 1.1921 |
| P                                                 | 0      |



If (	null hypothesis	)	{	reject $H_0$		} 

Since $P :(0) $ < 0.05 {	 reject $H_0$ 	}

A separate variance test wouldn't run in the null error.

### b)

($H_0:\ \mu_1 = \mu_2$) ($H_1 : \ \alpha_1 \neq \alpha_2$)

| Level of significance                             | 0.05     |
| ------------------------------------------------- | -------- |
| $_\text{sample}S_1$                               | 500      |
| $_\text{sample}\sigma_{\text{1}}$                 | 150      |
| $_\text{sample}\mu_{\text{1}}$                    | 153      |
| $_\text{sample}S_2$                               | 500      |
| $_\text{sample}\sigma_{\text{1}}$                 | 80       |
| $_\text{sample}\mu_{\text{2}}$                    | 85       |
| Upper critical value                              | 1.963    |
| Lower critical value                              | (-1.963) |
| P                                                 | 0        |
| $_\text{population 1} \circ_{\text{ of freedom}}$ | 3340.84  |
| $_\text{population 2} \circ_{\text{ of freedom}}$ | 4.386    |
| $_\text{total} \circ_{\text{ of freedom}}$        | 761.626  |
| $error_{standard}$                                | 7.6      |
| $\mu_2-\mu_1$                                     | 68       |
| $t_{Stat}$                                        | 8.944    |



If (	null hypothesis	)	{	reject $H_0$		} 

Mean order value difference is evident.

### c)

$$
(\bar{X}_1-\bar{X_2})\pm t_\frac{\alpha}{2} *\sqrt{\frac{_1S^2}{n_1}+\frac{_2S^2}{n_2}}
$$

$$
(153 - 85) \pm 1.963 * \sqrt{\frac{150^2}{500}+\frac{80^2}{500}}
$$

$$
\text{Inequality}: 53.075 \leq \mu_1 - \mu_2 \leq 82.924
$$

## 12.73

### a)

|                    | Twitter activity | delta  |
| ------------------ | ---------------- | ------ |
| Coefficient        | 0.05             | 6808   |
| $error_{standard}$ | 0.0035           | 854.97 |
| $t_{Stat}$         | 14.253           | 7.963  |
| P                  | 0                | 0.0005 |

### b)

The mean receipts will increase by $\approx$ 0.05 for $\Delta$ twitter activity.

When $\text{activity}_\text{twitter}=0, mean receipts = 6,808.1$

### c)

$$
\hat{Y}=b_0+b_1*X
$$

$$
\hat{Y}= 6808+0.05*100,000 = 11,808
$$

### d)

The domain of the independent variable is less than 1mil. Thus, extrapolated predictions are unreliable and should be avoided to be deduced from twitter activity if greater than domain.

### e)

$r^2= 0.976$, thus 97.6% the two variations move correlated.

### f)

There is no evident pattern, however sample size may be increased for more reliable residual analysis.

### g)

t= 14.2532 & p= 0

Since $p < \alpha = 0.05, H_0$ should be rejected. 

Linear correlation evident.


$$
\text{Interval}: 6,790.94\leq Y_{\ X=100,000}  \leq 16,879.58
$$

### i)

Twitter activity is, as seen above, a useful indicator for initial movie box office weekends receipts. Though, the sample size should be significantly greater for actual reliance on the data.

## 12.81

### a)

|           | Lower 95% | Upper 95% | P value | t Stat | Coefficients | Standard Error |
| --------- | --------- | --------- | ------- | ------ | ------------ | -------------- |
| Intercept | 138.44    | 199.13    | 0.000   | 11.39  | 168.78       | 14.81          |
| ERA       | -30.53    | -14.90    | 0.000   | -5.957 | -22.72       | 3.812          |

Intercept & slope: $b_0=168.78, b_1= (-22.719)$

### b)

If ERA = 0, est. mean wins = 168.78. Thus, $+\Delta$ team ERA  = $-\Delta*22.719$ wins.

### c)

$$
\hat{Y} = b_0+ b_1 *X = 168.78 + 22.72 (4.5 ) = 66.54 \approx 67
$$

### d)

$r^2=0.559$, thus 55.9% of variation in wins is deductible from $\Delta$ ERA.

### e)

There are no evident patterns in the residual plot, except proximity. In a normal plot, there is a more evident patterns visible. 

### f)

$H_0: \beta_1=0$, $H_1: \beta_1\neq0$, p=0 

Thus, reject $H_0$.

### i)

$$
(-30.533) \leq \beta_{1} \leq (-14.906)
$$

### j)

E.g all teams that played Baseball, within limits of e.g. geography or time or league.

### k)

Runs scored, hits, walks allowed, foul-play, etc. could be other independent variables for consideration.

### l)

Evident significant positive correlation between ERA and wins recorded.

## 13.49

$$
\hat{Y} = (-3.888) + 1.449* X_1 + 1.462*X_2-0.19*(X_1*X_2)
$$

### a)

$$
\hat{Y} = (-3.888) + 1.449* 2 + 1.462*2-0.19*(2*2)= 1.174
$$

### b)

$$
\hat{Y} = (-3.888) + 1.449* 2 + 1.462*7-0.19*(2*7)=6.584
$$

### c)

$$
\hat{Y} = (-3.888) + 1.449* 7+ 1.462*2-0.19*(7*2)= 6.519
$$

### d)

$$
\hat{Y} = (-3.888) + 1.449* 7 + 1.462*7-0.19*(7*7)=7.179
$$

### e)

$$
\hat{Y} = (-3.888) + 1.449* X_1 + 1.462*2-0.19*(X_1*2)
$$

$$
-0.964 + 1.069*X_1
$$

Thus, 1.069 is the slope of $X_1$.

### f)

$$
\hat{Y} = (-3.888) + 1.449* X_1 + 1.462*7-0.19*(X_1*7)
$$

$$
6.346 + 0.119*X_1
$$

### g)

$$
\hat{Y} = (-3.888) + 1.449* 2 + 1.462*X_2-0.19*(2*X_2)
$$

$$
(-0.99) + 1.082*X_2
$$

### h)

$$
\hat{Y} = (-3.888) + 1.449* 7 + 1.462*X_2-0.19*(7*X_2)
$$

$$
6.255 + 0.132*X_2
$$

### i)

$X_1$ And $X_2$ are negatively correlated, thus $\Delta$ in $X_1 \or X_2$ simultaneous and *aequis partibus* attenuation.

## 13.51

### a)

|                    | Intercept  | Field goal % | Three point field % |
| ------------------ | ---------- | ------------ | ------------------- |
| Coefficients       | (-217.474) | 4.352        | 1.692               |
| $error_{standard}$ | 50.732     | 1.303        | 1.1023              |
| $t_{\text{stat}}$  | (-4.287)   | 3.34         | 1.535               |
| P                  | 0.0002     | 0.0025       | 0.136               |
| Upper 95%          | (-113.38)  | 7.026        | 3.954               |
| Lower 95%          | (-321.568) | 1.679        | (-0.57)             |

Thus, $\hat{Y}=-217.474+4.352*_{\text{field goal %}}X_1+1.692*_{\text{field goal %}}X_2$ 

### b)

Three-point goal, field goal % $\Delta 0.01$ Increases wins estimate by 4.352. Perperam, $\Delta$ three-point goal increases wins estimate buy 1.692.

### c)

$$
\hat{Y}= -217.474 + 4.352*45+1.692*37 = 40.97
$$

### d)

Normal plot nor residual plot point toward potential disobedience of assumptions made.

### e)

$H_0 : \beta_1=\beta_2=0$, $H_1:\text{ !all } \beta_j= 0 \text{ for } j=1,2$

|            | df   | ss       | ms       | f      |
| ---------- | ---- | -------- | -------- | ------ |
| residual   | 27   | 2438.439 | 90.313   |        |
| regression | 2    | 2397.562 | 1198.781 | 13.274 |
| $\cup$     | 29   | 4836     |          |        |

Thus, $F=\frac{MSR}{MSE}=\frac{1198.781}{90.313}=13.274$

Since $P: (0.0001) <0.05$ {		reject $H_0$		}

Evident significant correlation between wins and field goal % $|$ three-point goal %.

### f)

Since $P: (0.0001),$  if $(H_0)$ 	{		 $P(F_{stat}=13.274)=0.0001$		}

### g)

$$
r^2=\frac{SSR}{SST}=\frac{2397.562}{4836}=0.496
$$

Thus, three-point goal % $|$ field goal % determine 49.6% of the win variation.

### h)



$_{\text{adj.}}r^2 = 0.458$

### i)

$$
X_1:t_{\text{stat}}=\frac{b_1}{s_{b_1}}=3.34
$$

Since $P: (0.0025)<0.05$ {		reject $H_0$		}

$X_1$may be superposition to $X_2$. 
$$
X_2:t_{\text{stat}}=\frac{b_2}{s_{b_2}}=1.5351
$$
Since $P:(0.136)>0.05$ {		do not reject $H_0$		} 

Thus, $X_1$ is the variable to be included over $X_2$.

### j)

$X_1:P=0.0025, X_2 : P=0.136$

Since $P: (0.0025),$  if $(X_1)$ 	{		 $P(t_{stat}: \pm 3.34)=0.25$		}

Since $P: (0.136),$  if $(X_2)$ 	{		 $P(t_{stat}: \pm 1.535)=0.136$		}

### k)

The explanatory variable field goal % is really the useful variable for win predictions.

## 13.55

### a)

$$
\hat{Y}= 87.721 - 18.953*X_1 + 15.963*X_2
$$

,where $X_1=\text{ERA } \& \ X_2=\text{runs scored}$ 

### b)

Runs scored constant, $\Delta ERA$ decreases estimated wins by means of 18.953.

Perperam, constant ERA, increases estimated wins by means of 15.963.

### c)

$$
\hat{Y} = 87.721 - 18.953*4+15.963*4
$$

### d)

There do not seem to be any evident violations of stated assumptions, when observing normal probability and residual plot. The normal plot has a clear correlation, where residuals proxy.

### e)

$F_{\text{stat}}=102.282, P = 0$

Since $P < 0.05$ 	{		reject $H_0$		}

Evident correlation between ERA and runs scored.

### f)

A zero P value would eliminate a test statistic of 102.282 or higher, if there would be nor correlation between ERA and runs scored.

### g)

$r^2 = 0.883$

,thus 88.3% variation in wins can be deducted from the two explanatory variables ERA and runs scored.

### h)

$_\text{adj.}r^2 = 0.875$ 

### i)

$X_1: (t_{\text{stat}})= -9.273, P=0$ 	{	reject $H_0$		}

ERA is indicative and insightful for modulation. 

$X_2: (t_{\text{stat}})= 8.668, P=0$ 	{	reject $H_0$		}

Runs scored is indicative and insightful for modulation. 

Regression is optimal choice, due to multiple *insightful* and *independent* variables.

### j)

$X_1: P= (0) \ P(\text{away from 0})\approx 0$, runs scored constant

$X_2: P= (0) \ P(\text{away from 0})\approx 0$, ERA constant 

### k)

$$
(-23.146) \leq \beta_1 \leq (-14.759)
$$
