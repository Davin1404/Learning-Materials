# Topic 11 Probability

$$E(ax+b) = aE(x)+b$$
$$Var(ax+b)=a^2Var()$$

## Discrete Random Variable X

### Expectation and Variance
For a ***discrete random*** variable $X$.  
$$E(X)=\sum \space xP(X=x)$$
$$Var(X)=E(X^2)-[E(X)]^2$$

## Discrete Continuous Variable X

### Expectation and Variance
For a ***continuous random*** variable $X$.  
$$E(X)=\int_{-\infty}^{\infty} xf_{pdf}(x)\space dx$$
$$Var(X)=\int_{-\infty}^{\infty} x^2f_{pdf}(x)\space dx-(\int_{-\infty}^{\infty} xf_{pdf}(x)\; dx)^2$$

## Binomial Distribution
## Probability Density Function
#### Proporties:
* The function is non-negative, $f(x) \ge 0$.  
*  The total area contained between the graph and the horizontal axis is 1. 
$$P(a < x\le b)=\int_{a}^{b} f_{pdf}(x)\space dx$$
$$\int_{-\infty}^{\infty} f_{pdf}(x)\space dx=1$$
GDC keywords:
1. `binomPdf(n,p,x)`  
2. `binomCdf(n,p,q,x)`

### Expectation and Variance
For $X \sim B(n,P)$
$$E(X)=np$$
$$Var(X)=np(1-p)$$

### Mode 
For mode $\mu$:
$$when\space\frac{df_{pdf}(x)}{dx}=0$$
$$\mu =x$$

### Median and percentiles
Half of the area under PDF lies to the left of m, thus the median $m$ satisfies: 
$$\int_{-\infty}^{m}f_{pdf}(x)dx=0.5$$

### Stardard Deviation
$$S.D.=\int_{0}^{1}x^2f(x)dx-\mu^2$$


## Normal Distribution 
### Normal Probability Density Function 
A bell-shaped density curve that is symmetric about the mean $\mu$. Its variability is measured by $\sigma$.  

GDC keyword: 
1.  `normCdf(up,down,m,SD)`
2.  `invNorm(area,m,SD)`

### Standard Normal Disctribution (Z~distribution ) 
* For the standard normal distribution (Z~distribution), ***the graph is symmetrical along the y-axis***. 
* *It has a mean $\mu$ of $0$ and a standard deviation $\sigma$ of 1*.   

Derivation: 
$$X\sim N(\mu,\sigma)$$
$$Let \space Z=\frac{X-\mu}{\sigma}$$
$$\therefore Z\sim N(\mu,\sigma)$$
$$\because E(Z)=E(\frac{X-\mu}{\sigma})=\frac{1}{\sigma}(E(X)-\mu)=\frac{1}{\sigma}(\mu -\mu)=0$$
$$\because Var(Z)=Var(\frac{X-\mu}{\sigma})=\frac{1}{\sigma^2}Var(X-\mu)$$
$$=\frac{1}{\sigma^2}Var(X-0)=\frac{1}{\sigma^2}Var(X)=\frac{1}{\sigma^2}\sigma^2=1$$
$$\therefore Z\sim N(0,1^2)$$

* Therefore, if $\mu$ or $\sigma$ is unkown, we can convert normal variable $X$ into standard variable $Z$.  
