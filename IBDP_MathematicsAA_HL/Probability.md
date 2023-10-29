# Probability

$$E(aX+b) = aE(X)+b$$
$$Var(aX+b)=a^2Var(X)$$

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
1.  $P(a<X<b)={\tt normCdf}(a,b,\mu,\sigma)$
    1.  `normCdf(a,b,m,SD)`  
2.  `invNorm(area,m,SD)`

### Standard Normal Disctribution (Z~distribution ) 
* For the standard normal distribution (Z~distribution), ***the graph is symmetrical along the y-axis***. 
* It has a mean $\mu$ of $0$ and a standard deviation $\sigma$ of 1 (variance $\sigma^2$).   

Derivation: 
$$X\sim N(\mu,\sigma^2)$$
$$Let \space Z=\frac{X-\mu}{\sigma}$$
$$\therefore Z\sim N(\mu_z,\sigma_z)$$
$$\because \mu_z=E(Z)=E(\frac{X-\mu}{\sigma})=\frac{1}{\sigma}(E(X)-\mu)=\frac{1}{\sigma}(\mu -\mu)=0$$
$$\because \sigma_z=Var(Z)=Var(\frac{X-\mu}{\sigma})=\frac{1}{\sigma^2}Var(X-\mu)$$
$$=\frac{1}{\sigma^2}Var(X-0)=\frac{1}{\sigma^2}Var(X)=\frac{1}{\sigma^2}\sigma^2=1$$
$$\therefore Z\sim N(0,1^2)$$

* Therefore, if $\mu$ or $\sigma$ is unkown, we can convert normal variable $X$ into standard variable $Z$.  

### The Expectation and Variance Algebra
The expectation algebra of one random variable:  
$$E(aX+b) = aE(X)+b$$
$$Var(aX+b)=a^2Var(X)$$

Linear combinations of two or more **Independent** random variables:  
$$E(a_1X_1+a_2X_2+...+a_nX_n) $$
$$= a_1E(X_1)+a_2E(X_2)+...+a_nE(X_n)$$
$$Var(a_1X_1+a_2X_2+...+a_nX_n)$$
$$=a_1^2Var(X_1)+a_2^2Var(X_2)+...+a_n^2Var(X_n)$$
> What is "Independent"?  
> e.g. Weights of 6 diffierent apples are independent random variables. 

The linear combination of two **independent** random variables that having ***normally*** distributed random variables also has a ***normal distribution***. 