# Paper2 Revision Note

# Class and Object
An ***object*** is an abstract entity and its components are data and actions.  

| Terms | Definitions |
| --- | --- |
| Constructor | A special kind of method, which is only declared once, that is called when an object is instantiated so that it initializes its data with specific values. Method name is same as the class name. |
| Accessor | A special kind of method that is called in order to read a specific data value of an object. Use the prefix “get” in the method name. |
>As the variables are declared as ***private*** in order protect data from accidental changes or from outside the object; 
>
>They cannot be accessed directly from outside this class;
>
>Therefore, ***public*** accessor methods are needed to ***permit access***; 

| Terms | Definitions |
| --- | --- |
| Mutator | special kind of method that is called in order to modify a private(hidden) variable in an object or class. Use the prefix “set” in the method name. |
| Signature | The methods name and all of its parameters and the types of these parameters. |
| Return value | Value that is passed back, returned, to the code that called the specific method.  |
| Identifier | The unique name of a program element |
| Object reference (pointer) | A reference is a variable whose value points to the location of an object (in memory) |
| Libraries | There consist of pre-written code, classes, procedures, methods etc. that programmers can use to add more functionality to their programs without having to rewrite the equivalent code.  |

>#### Advantages of using libraries: 
>
>Saves development time;  
>Since classes and their methods do not need to be rewritten;
>
>Promotes abstraction;  
>Because reusable code exists that functions without knowledge of internal working;
>
>Libraries contain error-free code;  
>Because it has been used and tested for many times;
>
>Promotes efficiency and organization;  
>As code will be shorter and easier to read;
>
>Familiarity with libraries;  
>Allow for easier maintenance or modification;

### Modifier
| Terms | Definitions |
|---|---|
| Public | Unlimited access. |
| Protected | Allows access to variable from within the package in which they are created. |
| Final | Prevents variables from being modified. |
| Static | Refers to variables that act on the class as a ***whole***. |

>#### Distinguish between a class and an instantiation.  
>
>A class is the blueprint of an object which does not occupy any memory in a program.
>
>An instantiation is the creation of an actual object which occupies enough memory to accommodate the object’s data and actions 

>#### M16 17, (c) discuss how the use of library classes simplifies the construction of the methods in parts(a) and (b) (asking for ArrayList)
>Can use the ArrayList library class; 
>
>Do not have to declare the size of the array; 
>
>Because the ArrayList automatically resizes itself; 
>
>Do not need to identify the index; 
>
>Because library class auto increments for you; 
>
>Could have used “sort list” instead of finding the correct place to insert object; 


---

# Object Oriented Programming (OOP)
### Definition
 A computer programming model that organizes software design around data, or ***objects***, rather than functions and logic. 

### Features
* Polymorphism  
* Encapsulation 
* Inheritance 

### Advantages  
* Re-use object;    
  * Which will speed up development.  
* Work can be ***split up*** across the sub-topics;  
  * Which will speed up development.  
* Sub-groups can re-use objects;  
  * Without having to re-program.  
* Quicker to test;  
  * As each module is small and independent;

### Disadvantages  
* Unsuitable for ***minor projects***;  
  * Since OOP increase complexity for little gain.  
* OOP programs are larger than other programs;  
  * Add therefore slower.  
* OOP programs take ***more effort*** to construct
  * Because of the decomposition needed to achieve abstraction.  

### Advantgaes of using ***modularity***
* Faster development;  
  * Because different programming teams can work on ***different modules***.  
* Easier to debug;  
  * Because the ***smaller modules*** will have ***fewer mistakes*** than one big program;  
* Easier to update (in the future);
  * Because it is easier to ***update a module*** than the full program.  

>#### M16 16, the company wished to update this OOP program and sell it to other hotels. They hire a programmer to make appropriate changes to the program
>(a)	Outline the responsibilities that the programmer has when updating the program.
>* Thorough testing;
>* Cite sources;
>* Update documentation;
>
>(b)	Discuss the features of modern programming languages that enable the program to be sold in other countries 
>* Unicode;
>* International character sets;
>* Changes are straightforward;

## Polymorphism (OOP's features)
### Definition 
*(empty)*

### ***Overload***  
The constructors have ***different parameter sets*** (or equivalent);  

***Compiler*** can differentiate between the two;  

The compiler will execute the constructor whose ***parameter set matches*** the arguments in the constructor call;  

### ***Override***  
Allows for subclasses to ***alter any superclasses actions*** and make them ***specific to their needs***;  

Method overrding ***redefines a method*** from the inherited class;  

### Advantages of using ***Polymorphism***  
Polymorphism allows an external program to use the same method actions on all subclasses;

By allowing overridden functions in child classes to add only the code that is needed for the unique processing of that sub-class;

In this example, the `getWeight()` method returns the weight of each piece of `RollingStock` . In the case of a wagon, the additional computation needed to add the weight of the cargo is added;

>#### M19 15, (c) outline how method overriding can help to create the new class FinalsOnlyEvent
>* Method overriding redefines a method from the inherited class;
>
>* The constructor could only instantiate the finals object;
>
>* The method `addSwimmers()` could fill finals directly;
>
>* The method `fillFinals()` could do nothing;

>#### M18 15(b) with reference to the two methods with the same name in the Points class, explain the OOP features that makes it possible to successfully implement either of these methods.
>Overloading;  
>The constructor methods have a different type of parameters;  
>During method calling, compiler will determine which of these methods is selected;  
>By matching up with the parameters;  

### Disadvantages of using ***Polymorphism***  
*(empty)*

## Encapsulation (OOP'sfeatures)  
### Definition  
Encapsulation places ***all attributes and methods*** that relate to a ***particular object;  

Encapsulation allows to make instance variable and method of a class ***private*** to that class;  

So that the main program ***cannot directly access*** the data in an object;  

### Advantages of using ***Encapsulation***  
Encapsulation places all attributes and methods that relate to a particular object;
For example, Payment class includes attributes such as the food and drink arrays and method such as `calculateBill()`;
This provides a clearer view of view/understanding of each section of the problem;
Which can lead to more efficient programming (faster and less errors);  

Encapsulations ***protects*** the values of the data stored within the object;  
From ***accidental changes*** made by other classes;  
For example, quantity in the FoorItem class cannot be altered through another variable called quantity in another class;  
This allows programmers to select any variable names they wish on choice of variable names; 

### Disadvantages of using ***Encapsulation***  
*(empty)*

## Inheritance  (OOP’s features) (“is a”)
### Definition
A ***new class*** is ***derived*** from an ***existing class***.  

The new class inherits ***all properties and method*** of the other class;   

The derived class is called a subclass, and the original is called a superclass.  

### Advantages of using ***Inheritance***  
It promotes code reuse;  
Because the superclass holds common data and actions that are ***shared*** by all newly developed classes;  

It reduces the amount of coding;  
By allowing sub-classes to ***inherit the methods***;  

It reduces maintenance overhead;  
Because you only have to ***update the superclass***;  

It allows extensibility that specific types of check-outs can be created which reduces development time, costs and testing. 

### Disadvantages of using ***Inheritance***  
*(empty)*

## Aggregation (“has a”)
### Definition 

### Advantages of using ***Aggregation***  
Aggregation allows code ***reuse and reduce amount of coding*** as the code for the (e.g., in M19 the Swimmer object) object has ***already existed***.  

Aggregation allows for the ***better organization*** of objects as the variables of the aggregated data will be kept in the class in which it belongs.


### Disadvantages of using ***Aggregation***  
Aggregation increases ***dependencies*** that a change in the owner class (e.g., in M19 the Swimmer class) could have an unexpected consequence for the subclass (e.g., in M19 the Race class);

Using aggregation can lead to more complex code; when accessing functions of the aggregated object;




---
