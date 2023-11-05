# Probability Distribution 
## 1. Discrete Probaility Distribution 
### 1.1 Cumulative Distribution Function (CDF)
The cumulative distribution function of a random variable $X$ expresses the probability that $X$ does not exceed the value $x$ as a function of $x$.  
$$F(x)=P(X\le x)=\sum _{y:y\le x}p(y)\tag{1}$$

### 1.2 Expected Value
For expected value $\mu$ :
$$\mu = E(X)=\sum \space xP(X=x)\tag{2}$$

### 1.3 Variance and standard deviation 
For variance:
$$Var(X)=\sum (x-\mu)^2P(X=x)=\sum x^2 P(X=x)-\mu^2\tag{3}$$  
$$Var(X)=E(X^2)-[E(X)]^2\tag{4}$$
For standard deviation $\sigma$ :
$$\sigma = \sqrt{Var(X)}\tag{5}$$

##

## 2. Binomial Distribution 
A sequence of several ***independent*** trials with ***equal*** probabilities.  

$$X \sim B(n,p)\tag{1}$$
### 2.1 The cumulative binomial distribution function 
[Cumulative Distribution Function for discrete random variables](#11-cumulative-distribution-function-cdf)



### 2.2 Mean (Expected value)
For mean $\mu$ :
$$\mu = E(X)=np\tag{2}$$

### 2.3 Variance and Standard Deviation
For variance:
$$Var(X)=npq=np(1-p)\tag{3}$$
For standard deviation $\sigma$ :
$$\sigma = \sqrt{Var(X)}=\sqrt{npq}\tag{4}$$


## 3. Continuous Distribution 
### 3.1 Probability Density Function (PDF)
#### Proporties:
* For a ***continuous random*** variable, a function can be used to model probabilities

$$P(a < X \le b)=\int_{a}^{b} f_{\text{pdf}}(x)\space dx \tag{1}$$  

* The function is non-negative for all values of $X$ 

$$f_{\text{pdf}}(x) \ge 0 \tag{2}$$   

*  The total area contained between the graph and the horizontal axis is 1. 

$$\int_{a}^{b} f_{\text{pdf}}(x)\space dx+\int_{b}^{c} f_{\text{pdf}}(x)\space dx+...=1$$  

$$\therefore\int_{0}^{\infty} f_{\text{pdf}}(x)\space dx=1\tag{3}$$

#### Tricks:  

$$P(X > a)=1-P(X \le a)=\int_{0}^{a}f_{\text{pdf}}(x)dx\tag{4}$$


#### GDC keywords:
1. `binomPdf(n,p,x)`  


### 3.2 Cumulative Distribution Function (CDF)
[Cumulative Distribution Function for discrete random variables](#11-cumulative-distribution-function-cdf)
#### GDC keyword: 
1.  `invNorm(area,m,SD)`

### 3.3 Mode 
For mode $M_o$ :
$$\text{when }\frac{df_{\text{pdf}}(x)}{dx}=0$$
$$M_o =x\tag{5}$$

### 3.4 Mean (Expected value)
* [Expected value for discrete distribution](#12-expected-value)  

For mean $\mu$ :
$$\mu = E(X)=\int xf_{\text{pdf}}(x)dx\tag{6}$$

### 3.5 Median
For median $m$ :  
* Half of the area under PDF lies to the left of m, thus the median $m$ satisfies.  
* ⚠️When there is ***MORE*** than one part in PDF, we need to consider ***the interval*** in which the value of $m$ lies.  
$$\int_{-\infty}^{m}f_{\text{pdf}}(x)dx=0.5\tag{7}$$

### 3.6 Percentile
For percentile $k$ :  
* The $k$ th percentile is defined as the value $n$ of the random variable such that $k\space \text{percent}$ of the values of $X$ are less than or equal to $n$, thus the $k$ th percentile satisfies:  

$$\int_{-\infty}^{n}f_{\text{pdf}}(x)dx=k\space\text{percent}\tag{8}$$ 


### 3.7 Variance and Standard Deviation
For variance:
$$Var(X)=\int x^2f_{\text{pdf}}(x)dx-\mu^2\tag{9}$$
For Standard Deviation $\sigma$ :
$$\sigma = \sqrt{Var(X)}\tag{10}$$

### 3.8 IQR  
For IQR:  

$$\text{IQR}=Q_3-Q_1\tag{11}$$  

* The $Q_1$ satisfies:  
$$\int _{-\infty}^{Q_1}f_{\text{pdf}}(x)=\frac{1}{4}\tag{12}$$  

* The $Q_3$ satisfies:  
$$\int _{-\infty}^{Q_3}f_{\text{pdf}}(x)=\frac{3}{4}\tag{13}$$  

##

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
 $$Z=\frac{X-\mu}{\sigma}$$
 $$\therefore Z\sim N(0,1^2)\tag{2}$$
##
Derivation: 
$$X\sim N(\mu,\sigma^2)$$
$$\text{Let} \space Z=\frac{X-\mu}{\sigma}$$
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

### 4.4 IQR
For IQR:  

$$\text{IQR}=Q_3-Q_1\tag{7}$$  

* The $Q_1$ satisfies:  

$$\int_{-\infty}^{Q_1}f_{\text{N}}(x)=\frac{1}{4}\tag{8}$$  

* Using GDC keywords `normCdf(a,b,m,SD)`, `invNorm(area,m,SD)`:  

$$\therefore\text{normCDF}(-\infty ,Q_1,\mu ,\sigma)=\frac{1}{4}$$  

$$\therefore Q_1=\text{invNorm}(\frac{1}{4},\mu ,\sigma)\tag{9}$$  

* In standard normal distribution:  

$$\therefore Q_1=\text{invNorm}(\frac{1}{4},0 ,1)\tag{10}$$ 

* The $Q_3$ satisfies:  

$$\int_{-\infty}^{Q_3}f_{\text{N}}(x)=\frac{3}{4}\tag{11}$$  

* Using GDC keywords `normCdf(a,b,m,SD)`, `invNorm(area,m,SD)`:  

$$\therefore\text{normCDF}(-\infty ,Q_3,\mu ,\sigma)=\frac{3}{4}$$

$$\therefore Q_3=\text{invNorm}(\frac{3}{4},\mu ,\sigma)\tag{12}$$  

* In standard normal distribution:  

$$\therefore Q_3=\text{invNorm}(\frac{3}{4},0 ,1)\tag{13}$$ 

##

## Average
$$S = x_1+x_2+...+x_n$$  

$$S \sim N(n\mu,n\sigma^2)$$

$$\overline{X}=\frac{x_1 + x_2 + ... + x_n}{n}$$  

$$\overline{X}\sim N(\mu,\frac{\sigma^2}{n})$$  

$$E(\overline{X})=E(\frac{x_1 + x_2 + ... + x_n}{n})=\frac{1}{n}E(x_1 + x_2 + ... + x_n)$$  

$$=\frac{1}{n}n\mu=\mu$$  

$$Var(\overline{X})=Var(\frac{x_1 + x_2 + ... + x_n}{n})=\frac{1}{n^2}Var(x_1 + x_2 + ... + x_n)$$  

$$=\frac{1}{n^2}n\sigma^2=\frac{\sigma^2}{n}$$