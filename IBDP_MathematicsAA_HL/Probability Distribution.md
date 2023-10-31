# Probability Distribution 
## 1. Discrete Probaility Distribution 
## 2. Binomial Distribution 
## 3. Continuous Distribution 
### 3.1 Probability Density Function (PDF)
#### Proporties:

$$P(a <X\le b)=\int_{a}^{b} f_{\text{pdf}}(x)\space dx \tag{1}$$  

* The function is non-negative  

$$f_{\text{pdf}}(x) \ge 0 \tag{2}$$   

*  The total area contained between the graph and the horizontal axis is 1. 

$$\int_{a}^{b} f_{\text{pdf}}(x)\space dx+\int_{b}^{c} f_{\text{pdf}}(x)\space dx+...=1$$  

$$\therefore\int_{0}^{\infty} f_{\text{pdf}}(x)\space dx=1\tag{3}$$

#### Tricks: 
$$P(X>a)=1-P(X<a)=\int _{0}^{a}f_{\text{pdf}}(x)dx\tag{4}$$

#### GDC keywords:
1. `binomPdf(n,p,x)`  


### 3.2 Cumulative Distribution Function (CDF)
### 3.3 Measures of Center, Position, and Spread of a Continuous Distribution
#### 3.3.1 Mode 
For mode $M_o$ :
$$\text{when }\frac{df_{\text{pdf}}(x)}{dx}=0$$
$$M_o =x$$

#### 3.3.2 Mean (Expectation)
For mean $\mu$ :
$$\mu = E(X)=\int xf_{\text{pdf}}(x)dx$$

#### 3.3.3 Median
For median $m$ :  
* Half of the area under PDF lies to the left of m, thus the median $m$ satisfies
$$\int_{-\infty}^{m}f_{\text{pdf}}(x)dx=0.5$$

#### 3.3.4 Percentile
For percentile $k$ :  
* The $k$ th percentile is defined as the value $n$ of the random variable such that $k\%$ of the values of $X$ are less than or equal to $n$, thus the $k$ th percentile satisfies
$$\int _{-\infty}^{n}f_{pdf}(x)dx=k\%$$

## 4. Normal Distribution 
### 4.1 Normal Probability Density Function 
A bell-shaped density curve that is ***symmetric*** about the mean $\mu$. Its variability is measured by $\sigma$.  
$$X\sim N(\mu,\sigma^2)\tag{1}$$

GDC keyword: 
1.  `normCdf(a,b,m,SD)`  
2.  `invNorm(area,m,SD)`

### 4.2 Standard Normal Disctribution (Z~distribution ) 
* For the standard normal distribution (Z~distribution), ***the graph is symmetrical along the y-axis***. 
* It has a mean $\mu$ of $0$ and a standard deviation $\sigma$ of 1 (variance $\sigma^2$).   
* Therefore, if $\mu$ or $\sigma$ is unkown, we can convert normal variable $X$ into standard variable $Z$.  
 $$\therefore Z\sim N(0,1^2)\tag{2}$$

##
Derivation: 
$$X\sim N(\mu,\sigma^2)$$
$$Let \space Z=\frac{X-\mu}{\sigma}$$
$$\therefore Z\sim N(\mu_z,\sigma_z)$$
$$\because \mu_z=E(Z)=E(\frac{X-\mu}{\sigma})=\frac{1}{\sigma}(E(X)-\mu)=\frac{1}{\sigma}(\mu -\mu)=0$$
$$\because \sigma_z=Var(Z)=Var(\frac{X-\mu}{\sigma})=\frac{1}{\sigma^2}Var(X-\mu)$$
$$=\frac{1}{\sigma^2}Var(X-0)=\frac{1}{\sigma^2}Var(X)=\frac{1}{\sigma^2}\sigma^2=1$$
$$\therefore Z\sim N(0,1^2)$$
##



### 4.3 The Expectation and Variance Algebra
The expectation algebra of one random variable:  
$$E(aX+b) = aE(X)+b\tag{3}$$
$$Var(aX+b)=a^2Var(X)\tag{4}$$

Linear combinations of two or more **Independent** random variables:  
$$E(a_1X_1+a_2X_2+...+a_nX_n) $$
$$= a_1E(X_1)+a_2E(X_2)+...+a_nE(X_n)\tag{5}$$
$$Var(a_1X_1+a_2X_2+...+a_nX_n)$$
$$=a_1^2Var(X_1)+a_2^2Var(X_2)+...+a_n^2Var(X_n)\tag{6}$$
> What is "Independent"?  
> e.g. Weights of 6 diffierent apples are independent random variables. 

The linear combination of two **independent** random variables that having ***normally*** distributed random variables also has a ***normal distribution***. 