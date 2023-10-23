# Topic 11 Probability

## Discrete Random Variable X

### Expectation and Variance
For a ***discrete random*** variable $X$.  
$$E(X)=\Sigma \space xP(X=x)$$
$$Var(X)=E(X^2)-[E(X)]^2$$

## Discrete Continuous Variable X

### Expectation and Variance
For a ***continuous random*** variable $X$.  
$$E(X)=\int_{-\infty}^{\infty} xf(x)\space dx$$
$$Var(X)=\int_{-\infty}^{\infty} x^2f(x)\space dx-(\int_{-\infty}^{\infty} xf(x)\; dx)^2$$

## Binomial Distribution
### Probability Density Function
Proporties:
* The function is non-negative, $f(x) \ge 0$.  
*  The total area contained between the graph and the horizontal axis is 1. 
$$P(a < x\le b)=\int_{a}^{b} f(x)\space dx$$
$$\int_{-\infty}^{\infty} f(x)\space dx=1$$
* GDC keywords: `binomPdf(n,p,x)`  , `binomCdf(n,p,q,x)`

### Expectation and Variance
For $X \sim B(n,P)$
$$E(X)=np$$
$$Var(X)=np(1-p)$$
 


