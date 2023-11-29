# B.3 Fluids and Fluids dynamics
## B.3.1 Static fluids - density and pressure 
### Density - a property of matter
The mass per unit volume of a substance.  
$$\text{density}=\frac{\text{mass}}{\text{volume}}\tag{1}$$  
$$\rho = \frac{m}{V}$$

##

### Pressure
The normal force acting per unit cross-sectional area  
$$\text{pressure}=\frac{\text{normal force}}{\text{cross-sectional area}}\tag{2}$$  
$$P=\frac{F}{A}$$  

##

### Hydrostatic Pressure in a Fluid  
$$P=\rho gh\tag{3}$$  
$$h=\text{depth}$$
$$g=\text{Gravitational field strength}$$  

⚠️Total pressure $P$ at depth $h$:
$$P=\rho gh+p_0\tag{4}$$  
$$p_0=\text{Atmospheric pressure}$$

##

### U tube
$$h_1 \rho _1=h_2 \rho_2 \tag{5}$$  

![uTude](/IBDP_Physics_HL/Topic%20B%20Engineering/image/uTube.png)  

##

### Pascal'ss principle  
The pressure applied at one point in an enclosed fluid under equilibrium conditions is transmitted equally to all parts of the fluid.  

$$p_1=\frac{F_1}{A_1}=\frac{F_2}{A_2}\tag{6}$$  

$$P_1 = \text{Pressure throughout fluid}$$

![pascal](/IBDP_Physics_HL/Topic%20B%20Engineering/image/PascalPrinciple.png)  

## B.3.2 Archimedes' principle  
For an object wholly or partially immersed in a fluid, there will be an upward buoyancy force (upthrust) acting on the object which is equal to the weight of fluid that the object displaces.   

$$B=\rho _f V_f g\tag{7}$$  
$$B = \text{Buoyancy (upthrust) force}$$
$$V_f = \text{Volume of fluid that the object displaces}$$  

#### ⚠️The origin of the buoyancy force:   
Pressure in a liquid increases with depth, so pressure at bottom of bubble greater than pressure at top.  

##

## B.3.3 Fluid dynamics  
### An ideal fluid  
An ideal fluid offers ***no resistance*** either to a solid moving through it or it moving through or around a solid object.   

* ***Non-viscous***
  * Does not exert forces on other fluids.  
* ***Laminar*** flow
  * Fluid velocity of a point in the fluid is constant.  
* ***Incompressible*** 
  * The fluid cannot be compressed and so density is constant throughout.  

##

### Streamline (or laminar) flow  
#### Streamline 
The paths taken by particles within a fluid.  

#### ⚠️The continuity equation  
$$Av=\text{constant}\tag{8}$$  
$$A=\text{Cross-section area}$$  
$$v=\text{velocity of the fluid}$$

$$\text{voume flow rate: } Av$$
$$\text{Unit: }\text{m}^3\text{s}^{-1}$$

![TCE](/IBDP_Physics_HL/Topic%20B%20Engineering/image/maxresdefault.jpg) 

##

### The Bernoulli equation 
$$\frac{1}{2} \rho v^2+\rho gh+P=\text{constant}\tag{9}$$

##

## B.3.4 Applications of the Bernoulli equation 

### Airfoil
⚠️***Height*** constant⚠️ as we assume that airfoil is very thin.  

Find lift force.  

$$\frac{1}{2}\rho v_1^2+\sout{\rho g z_1}+P_1=\frac{1}{2}\rho v_2^2+\sout{\rho g z_2} +P_2$$  

$$\frac{1}{2}\rho (v_1^2-v_2^2)=P_2-P_1$$  

$$\because F_{\text{lift}}=\Delta P\times A$$  

$$\therefore F_{\text{lift}}=\frac{1}{2}\rho (v_1^2-v_2^2)\times A\tag{ANS}$$  

![airfoil](/IBDP_Physics_HL/Topic%20B%20Engineering/image/airfoil.jpg)

##

### Venturi tubes  
⚠️***Height*** constant⚠️

Find pressure / height difference.  

$$\frac{1}{2}\rho v_1^2+\sout{\rho g z_1}+P_1=\frac{1}{2}\rho v_2^2+\sout{\rho g z_2} +P_2$$  

$$\frac{1}{2}\rho v_1^2+P_1=\frac{1}{2}\rho v_2^2+P_2$$  

$$\frac{1}{2}\rho (v_1^2-v_2^2)=P_2-P_1$$  

$$\frac{1}{2}\rho (v_1^2-v_2^2)=\rho g \Delta h $$  

$$\rho g \Delta h=\text{hydrostatic pressure}$$

$$\Delta h = \frac{1}{2g}(v_1^2-v_2^2)\tag{ANS}$$  

![vTubes](/IBDP_Physics_HL/Topic%20B%20Engineering/image/2560px-Venturi5.png) 

##

### Pitot static tubes
**Function**: measuring the velocity of a fluid of density $\rho$.  
⚠️***Height*** constant⚠️  
⚠️***Final velocity*** $=0$⚠️    

$$\frac{1}{2}\rho v_x^2+\sout{\rho g z_x}+P_x=\frac{1}{2}\rho v_y^2+\sout{\rho g z_y} +P_y$$  

$$\frac{1}{2}\rho v_x^2 = P_y-P_x$$  

$$\frac{1}{2}\rho v_x^2 = \rho g \Delta h$$

$$v_x=\pm \sqrt{2g\Delta h}\tag{ANS}$$  

![pitot](/IBDP_Physics_HL/Topic%20B%20Engineering/image/pitot.png)

##

### Flow out of a container  

⚠️***Pressure*** is constant: as container has **constant** radius.⚠️  
⚠️***Initial velocity*** = 0⚠️  
⚠️$P_x=P_y=P_0$ ⚠️ as two points are open to atmosphere, ***they will be both at atmosphere pressure***  

$$\frac{1}{2}\rho v_x^2 + \rho gh_x = \frac{1}{2}\rho v_y^2 + \rho gh_y$$  

$$\rho g(h_x-h_y)=\frac{1}{2}\rho v_y^2$$  

$$v_y=\sqrt{2gh_x}\tag{ANS}$$  

![flow](/IBDP_Physics_HL/Topic%20B%20Engineering/image/Flow.png)

##

## B.3.5 Stokes' law and viscosity  
### Viscosity  
The viscosity $\eta$ of fluids is highly temperature dependent.  
It has the units $\text{Pas}$

* For ***liquids***, ***less*** viscous at higher temperature  
* For ***gases***, ***more*** viscous at higher temperature.  

### Stokes' law

$$F_d=6\pi \eta rv\tag{10}$$  

##
$$r=\text{Radius of the sphere}$$  

$$v=\text{Speed of the sphere}$$  

$$\eta = \text{a constant, coefficient of viscosity, unit (Pas)}$$  
##

### Terminal speed 

$$6\pi \eta rv_t+\frac{4}{3}\pi r^3 \rho g=mg$$  

$$\therefore 6\pi \eta rv_t+\frac{4}{3}\pi r^3 \rho g=\frac{4}{3}\pi r^3\sigma g$$  

$$\therefore v_t = \frac{2r^2g(\sigma-\rho)}{9\eta} \tag{11}$$  

##
$$v_t = \text{Ball's terminal speed}$$  

$$\rho = \text{The density of fluid}$$  

$$\sigma = \text{The density of the ball}$$  
##

assumption 1: sphere  
assumption 2: laminen flow  

## B.3.6 Laminnar flow and turbulent flow  

|Laminar Flow|Turbulent Flow|
|---|---|
|The velocity of the fluid is constant any point in the fluid.  |The velocity is not constant.|  

![Turbulent fow](/IBDP_Physics_HL/Topic%20B%20Engineering/image/Turbulent.png)  

### Reynolds number
Reynolds number $R$ can be used to predict whether the flow is great enough to become turbulent.  

$$R=\frac{vr\rho}{\eta} \tag{12}$$  

|after the calculation|conclusion|
|---|---|
|$R<1000$|Laminar flow|
|$R>1000$|It does not mean that the flow will be turbulent because there is a transition stage between the fluid being laminar or turbulent|
|$R>2000$|Turbulent flow|


##
$$v=\text{velocity}$$  

$$r=\text{radius of the pipe}$$  

$$\rho = \text{Density of the liquid}$$

$$\eta = \text{Viscosity of the liquid}$$  
##
