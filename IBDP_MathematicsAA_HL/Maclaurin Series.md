# Maclaurin series
$$f(x)=f(0)+xf'(0)+\frac{x^2}{2!}f''(0)+\frac{x^3}{3!}f'''(0)+...$$

$$\text{e.g. Find the Maclaurin seris for } \ln(1+\text{sin}(x))$$  
$$f(0)=\ln(1+\text{sin}(0))=0  $$  
$$f'(0)=\frac{\text{cos}(0)}{1+\text{sin}(0)}=1 $$  
$$f''(0)=-\frac{1}{1+\text{sin}(0)}=-1  $$  
$$f'''(0)=\frac{\text{cos}(0)}{(1+\text{sin}(0))^2}=1 $$  
$$f^{(4)}(0)=...$$  
$$\therefore \ln (1+\text{sin}(x))=x-\frac{x^2}{2!}+\frac{x^3}{3!}+...\tag{ANS}$$  

## Tricks  

*Some derivation that appeared in the previous homework:*  

$$\text{Find the Maclaurin seris for } \ln(1-\text{sin}(x))$$  

$$\ln(1-\text{sin}(x))=\ln[1+(-\text{sin}(x))]$$  

$$=\ln(1+\text{sin}(-x))$$  

$$\therefore =0+(-x)-\frac{(-x)^2}{2!}+\frac{(-x)^3}{3!}+...$$  

$$\therefore \ln(1-\text{sin}(x)) =-x-\frac{x^2}{2!}-\frac{x^3}{3!}+...\tag{ANS}$$  

##

$$\text{Find the Maclaurin seris for } \ln(\text{cos}(x))$$  

$$\because \ln(1+\text{sin}(x))+\ln(1-\text{sin}(x))=\ln[(1+\text{sin}(x))(1-\text{sin}(x))]$$  

$$=\ln(1^2-\text{sin}^2(x))=\ln(\text{cos}^2(x))=2\ln(\text{cos}(x))$$  

$$\therefore \ln(\text{cos}(x))=\frac{1}{2}[\ln(1+\text{sin}(x))+\ln(1-\text{sin}(x))]$$  

$$=\frac{1}{2}[(x-\frac{x^2}{2!}+\frac{x^3}{3!}+...)+(-x-\frac{x^2}{2!}-\frac{x^3}{3!}+...)]$$  

$$\therefore \ln(\text{cos}(x))=-\frac{1}{2}x^2-\frac{1}{12}x^4+...\tag{ANS}$$    

##

$$\text{Find the Maclaurin seris for } \text{tan}(x)$$  

$$\because \frac{\text{d}}{\text{d}x}[\ln(\text{cos}(x))]=\frac{1}{\text{cos}(x)}(-\text{sin}(x))=-\tan(x)$$  

$$\therefore \tan(x)=-\frac{\text{d}}{\text{d}x}[\ln(\text{cos}(x))] =-\frac{\text{d}}{\text{d}x}(-\frac{1}{2}x^2-\frac{1}{12}x^4+...)$$  

$$\therefore \tan(x)=x+\frac{1}{3}x^3+...\tag{ANS}$$  

