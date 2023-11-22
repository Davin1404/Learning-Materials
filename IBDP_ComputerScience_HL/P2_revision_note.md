# Paper2 Revision Note

# Class and Object
An ***object*** is an abstract entity and its components are data and actions.  

| Terms | Definitions |
| --- | --- |
| Constructor | A special kind of method, which is only declared once, that is called when an object is instantiated so that it initializes its data with specific values. Method name is same as the class name. |
| Accessor | A special kind of method that is called in order to read a specific data value of an object. Use the prefix “get” in the method name. |  

As the variables are declared as ***private*** in order protect data from accidental changes or from outside the object; 

They cannot be accessed directly from outside this class;

Therefore, ***public*** accessor methods are needed to ***permit access***; 

| Terms | Definitions |
| --- | --- |
| Mutator | special kind of method that is called in order to modify a private(hidden) variable in an object or class. Use the prefix “set” in the method name. |
| Signature | The methods name and all of its parameters and the types of these parameters. |
| Return value | Value that is passed back, returned, to the code that called the specific method.  |
| Identifier | The unique name of a program element |
| Object reference (pointer) | A reference is a variable whose value points to the location of an object (in memory) |
| Libraries | There consist of pre-written code, classes, procedures, methods etc. that programmers can use to add more functionality to their programs without having to rewrite the equivalent code.  |

##

#### Advantages of using libraries: 

Saves development time;  
Since classes and their methods do not need to be rewritten;

Promotes abstraction;  
Because reusable code exists that functions without knowledge of internal working;

Libraries contain error-free code;  
Because it has been used and tested for many times;

Promotes efficiency and organization;  
As code will be shorter and easier to read;

Familiarity with libraries;  
Allow for easier maintenance or modification;

##

### Modifier
| Terms | Definitions |
|---|---|
| Public | Unlimited access. |
| Protected | Allows access to variable from within the package in which they are created. |
| Final | Prevents variables from being modified. |
| Static | Refers to variables that act on the class as a ***whole***. |

##
#### Static  
Static means it is the same for all instances of the class;  
because it is contained in the class rather than in an instance of the class/object / it is defined 
at the class level;

Static means that less memory is taken up;  
as only 1 memory allocation it created for all instances rather than 1 per instance;  

|Static variables|Static methods|
|---|---|
|Static variable is a class variable not re-declared in each object; The values are the ***same*** for all objects;|Are class methods (not object methods); Are ***independent*** of the objects in the class;|

##

#### Distinguish between a class and an instantiation.  
* A class is the blueprint of an object which does not occupy any memory in a program. ***Do not occupy any memory in a program***.  

* An instantiation is the creation of an actual object which ***occupies enough memory to accommodate the object’s data and actions***.   

##

#### Define the relationships between object, objects’ data and objects’ actions.  

An object is thus an abstract entity that describes the data that this entity has (properties or attributes) and the actions that this entity can perform (methods).   

##

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

##

### Features
* Polymorphism  
* Encapsulation 
* Inheritance 

##

### Advantages  
* Re-use object;    

  * Which will speed up development.  
* Work can be ***split up*** across the sub-topics;  
  * Which will speed up development.  
* Sub-groups can re-use objects;  
  * Without having to re-program.  
* Quicker to test;  
  * As each module is small and independent;

##

### Disadvantages  
* Unsuitable for ***minor projects***;  

  * Since OOP increase complexity for little gain.  
* OOP programs are larger than other programs;  
  * Add therefore slower.  
* OOP programs take ***more effort*** to construct
  * Because of the decomposition needed to achieve abstraction.  

##

### Advantgaes of using ***modularity***
* Faster development;  

  * Because different programming teams can work on ***different modules***.  
* Easier to debug;  
  * Because the ***smaller modules*** will have ***fewer mistakes*** than one big program;  
* Easier to update (in the future);
  * Because it is easier to ***update a module*** than the full program.  

##

>#### N15 (d) In relation to the Doctor object, outline the need for extended character sets as used by modern programming languages.  
>
>Different languages use different characters, which are not included in the basic 8-bit ***ASCII*** character set; 
> 
>Extended character sets (like ***Unicode***) include all possible characters from all languages;  
>
>For example, the doctor’s name could not be spelled correctly in ***ASCII***;  

##

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

##

# Polymorphism (OOP's features)
### Definition 
*(empty)*

##

### Characteristics
Each method is defined within its own class.  
Each method is called within an object of that class.  
Therefore the compiler (allow program) knows which method to use.  

##

### ***Overload***  
* The constructors have ***different parameter sets*** (or equivalent);  

* ***Compiler*** can differentiate between the two;  

* The compiler will execute the constructor whose ***parameter set matches*** the arguments in the constructor call;  

##

### ***Override***  
* Allows for subclasses to ***alter any superclasses actions*** and make them ***specific to their needs***;  

* Method overrding ***redefines a method*** from the inherited class;  

##

### Advantages of using ***Polymorphism***  
* Polymorphism allows an external program to use the same method actions on all subclasses;

* By allowing overridden functions in child classes to add only the code that is needed for the unique processing of that sub-class;

* In this example, the `getWeight()` method returns the weight of each piece of `RollingStock` . In the case of a wagon, the additional computation needed to add the weight of the cargo is added;

##

>#### M19 15, (c) outline how method overriding can help to create the new class FinalsOnlyEvent
>* Method overriding redefines a method from the inherited class;
>
>* The constructor could only instantiate the finals object;
>
>* The method `addSwimmers()` could fill finals directly;
>
>* The method `fillFinals()` could do nothing;

##

>#### M18 15(b) with reference to the two methods with the same name in the Points class, explain the OOP features that makes it possible to successfully implement either of these methods.
>Overloading;  
>The constructor methods have a different type of parameters;  
>During method calling, compiler will determine which of these methods is selected;  
>By matching up with the parameters;  

##

### Disadvantages of using ***Polymorphism***  
*(empty)*

##

# Encapsulation (OOP'sfeatures)  
### Definition  
* Encapsulation places ***all attributes and methods*** that relate to a ***particular*** object;  

* Encapsulation allows to make instance variable and method of a class ***private*** to that class. So that the main program ***cannot directly access*** the data in an object;  

##

### Characteristics

By using private for variables Data can be protected from accidental changes or from outside the object; ***accessor*** and ***mutator*** method are in the place in order that other classes will access.  

The class combines data and methods; So as to reuse the code for multiple dates.


##

### Advantages of using ***Encapsulation***  
* Encapsulation places all ***attributes*** and ***methods*** that relate to a ***particular*** object;
  
  * For example, Payment class includes attributes such as the food and drink arrays and method such as `calculateBill()`;
  
  * This provides a clearer view of view/understanding of each section of the problem;
  
  * Which can lead to more efficient programming (faster and less errors);  

* Encapsulations ***protects*** the values of the data stored within the object;  
  
  * From ***accidental changes*** made by other classes;  
  
  * For example, quantity in the FoorItem class cannot be altered through another variable called quantity in another class; 
 
  * This allows programmers to select any variable names they wish on choice of variable names; 

##

### Disadvantages of using ***Encapsulation***  
*(empty)*

##

# Inheritance  (OOP’s features) (“is a”)
### Definition
* A ***new class*** is ***derived*** from an ***existing class***.  

* The new class inherits ***all properties and method*** of the other class;   

* The derived class is called a subclass, and the original is called a superclass.  

##

### Advantages of using ***Inheritance***  
* It promotes code reuse;  
  
  * Because the superclass holds common data and actions that are ***shared*** by all newly developed classes;  

* It reduces the amount of coding;  
  
  * By allowing sub-classes to ***inherit the methods***;  

* It reduces maintenance overhead;  
  
  * Because you only have to ***update the superclass***;  

* It allows extensibility 
  * that specific types of check-outs can be created which reduces development time, costs and testing. 

##

### Disadvantages of using ***Inheritance***  
*(empty)*

##

# Aggregation (“has a”)
### Definition 
*(empty)*

### Advantages of using ***Aggregation***  
* Aggregation allows code ***reuse and reduce amount of coding*** as the code for the (e.g., in M19 the Swimmer object) object has ***already existed***.  

* Aggregation allows for the ***better organization*** of objects as the variables of the aggregated data will be kept in the class in which it belongs.


### Disadvantages of using ***Aggregation***  
* Aggregation increases ***dependencies*** that a change in the owner class (e.g., in M19 the Swimmer class) could have an unexpected consequence for the subclass (e.g., in M19 the Race class);

* Using aggregation can lead to ***more complex code***; when accessing functions of the aggregated object;

##

# Dependencies (“uses a”)
### Definition 
*(empty)*  

##

### Advantages of using ***Dependencies***  
*(empty)*  

##

### Disadvantages of using ***Dependencies***  
* Dependencies when one object uses another object, the first object depends on the second, since it cannot function without it. Whenever the first object needs to be used, the second object will be used as well.  

* Dependencies are ***directional***, in that an object can depend on another object, but the second object does not necessarily need to depend on the first object as well.   

* For example, if object A depends on object B, it does not necessarily mean that B also depends on A. 


##

>#### The reasons for keeping dependencies to a minimum
>
>Changes in one class in a dependency will affect the other classes in this dependency;  
>This may cause programs using the second class not to function;
>
>Reduce maintenance overheads;  
>As a programmer editing one class would not have to be concerned with other classes;

##

>#### Outline two reasons why the use of multiple programming teams in different locations may be problematic when developing an integrated software solution.
>   
>i.	Teams may be located in different countries; therefore, they may have communication issues with each other due to different languages or different time zones;  
>
>ii.	Inability to discuss face-to-face which reduces efficiency;  
>
>iii.	Problems with different conventions (e.g., data format);  
>
>iv. Managing the teams in different locations may be problematic;
>
>v.	Teams may not collaborate well due to personality issues;
>
>vi.	Development time might increase;

##

>#### N19 17, (f) explain the importance of using coding style and naming conventions when programming
>i.	Indentation/use of white space  
>ii.	Annotations   
>iii.	Meaningful identifiers   
>iv.	Capitalization conventions  
>
>i.	Helps reading and understanding;  
>ii.	For easer maintenance and extension;    
>iii.	For better team-work, collaboration and development;
>iv.	To help with de-bugging;   

>#### Describe one feature of modern programming languages that allow the wide range of students’ names to be represented correctly.  
>	
>Modern programming languages use Unicode; which uses more bits than ASCII; This allows the use of non-Latin languages.  

---

# Data Structure

# Stack

### Definition
FILO (first in last out) data structure.  

>#### Applications:  
>The system stack stores return data of interrupted processes; The last interrupted process is the first to resume.  

# Queue
### Definition
FIFO (first in first out) data structure, only allowss addition at the end and removal from the front.  

### Advantages of using "***Queue***"
*(empty)*

### Disadvantages of using "***Queue***"
* This is not sufficient in scenarios that elements can ***change freely***;  
* Because it is a ***FIFO data structure*** / only allows addition at the end and removal from the front;
* It has no ***fixed length*** which could lead to ***unmanageable***;

# ArrayList 

### Definition
*(empty)*

### Advantages of using "***ArrayList***"
* Memory space for the exact number of objects can be assigned.
    
* There is no need to determine ArrayList size.  

### Disadvantages of using "***ArrayList***"
* Using a ***fixed*** amount of memory is inefficient;  
  * as it will ***re-size*** itself when more entries are required.  

* ***Overflow*** is a problem;  
  * as there is a ***fixed*** amounts of element allowed.  

# LinkedList

* Java-specific data structure  

* Doubly-linked list (although sometimes referred to as a singly-linked list on the exam)
* Each piece of data is stored in a node, with pointers
* Located non-contiguously in memory - addresses of nodes are spread out across RAM and nodes only linked by pointers
* Ideal for frequent insertion or deletion of elements, or when the size of the list is unknown
* Ideal Use Cases
  * Implementing a Queue - front of the queue is represented by the head of the Linked List, and the rear of the queue is represented by the tail of the Linked List.  

  * Implementing a Stack - top of the stack is represented by the head of the Linked List, and the bottom of the stack is represented by the tail of the Linked List
  * Large Data Sets (due to dynamic memory allocation)

|Pros|Cons|
|---|---|
|***Dynamic Size*** - Unlike arrays, linked lists can grow or shrink in size|***Access Time*** - Finding a specific value in a linked list takes longer than in an array|
|***Easy Insertion and Deletion*** - easy to insert and delete elements from linked list; simply invovlves changing points of adjacent nodes|***Extra memory overhead*** - pointers are utilized, which take up more memory than a single array element|  
|***Efficient memory usage*** - memory is only allocated for elements in the linked list unlike arrays|***Complexity*** - linked lists can be more difficult to implement and debug than simple data structures like arrays|
|***Versatility*** - can be used to implement other data structures like stacks and queues||

### Replace a data structure to ***LinkedList***
* Modify the class to have a “next” member variable (next element pointer);  
  
* Modify the first class to have a “first” member variable (begin element pointer);  
* Modify the `add()` and `remove()` methods to implement the linked list;

### Code Example
#### Example 1: Create and initialize LinkedList
```
LinkedList<Student> studentList = new LinkedList<>();
Student jamesObject = new Student("John Doe", 20, "Computer Science",85);
Student janeObject = new Student("Jane Smith", 21, "Mathematics",90); 

// Add 5 Student objects to the list

studentList.add(jamesObject);
studentList.add(janeObject);
studentList.add(new Student("Bob Johnson", 19, "Physics", 92));
studentList.add(new Student("Alice Brown", 22, "Chemistry", 88));
studentList.add(new Student("Charlie Lee", 18, "Biology", 87));
```

#### Example 2 : Display Contents of Linked List
```
public void displayStudentInfo(LinkedList<Student> studentList) {
    int index = 0;
    while(index < studentList.size()) {
        Student currentStudent = studentList.get(index);
        System.out.println(currentStudent.getName() + " "+
        currentStudent.getGrade());
        index++;
    }
}
```

#### Example 3: Transfer Contents of an Array to a Linked List
```
public LinkedList<Student> arrayToLinkedList(Student[] studentArray){
    LinkedList<Student> studentList = new LinkedList<>();
    for(int i = 0; i < studentArray.length; i++) {
        studentList.addLast(studentArray[i]);
    }
    return studentList;
}
```

#### Example 4: Transfer Contents of a LinkedList to an Array
```
public Student[] linkedListToArray(LinkedList<Student> studentList) {
    Student[] studentArray = new Student[studentList.size()];
    int studentArrayIndex = 0;
    while(studentArrayIndex < studentList.size()) {
        studentArray[studentArrayIndex] =
            studentList.get(studentArrayIndex);
        studentArrayIndex++;
    }
    return studentArray;
}
```

#### Example 5: Transfer Contents of a LinkedList to an Array (Using an Iterator)
```
public Student[] iteratorlinkedListToArray(LinkedList<Student>studentList){
    Student[] studentArray = new Student[studentList.size()];
    int studentArrayIndex = 0;
    ListIterator<Student> studentIterator =
        studentList.listIterator();
    while (studentIterator.hasNext()) {
        studentArray[studentArrayIndex] = studentIterator.next();
        studentArrayIndex++;
    }
    return studentArray;
}
```

#### Example 6: Find the Maximum Value of An Attribute in a LinkedList of Objects
```
public int findMaximum(LinkedList<Student> studentList) {
    int maximum = studentList.getFirst().getGrade();
    ListIterator<Student> studentIterator =
        studentList.listIterator();
    while(studentIterator.hasNext()) {
        Student currentStudent = studentIterator.next();
        int currentGrade = currentStudent.getGrade();
        if(currentGrade > maximum) {
            maximum = currentGrade;
        }
    }
    return maximum;
}
```

#### Example 7: Remove an Object Based on Some Criteria
```
public boolean removeByName(LinkedList<Student> studentList, Stringname){
    int index = 0;
    while(index < studentList.size()) {
    Student currentStudent = studentList.get(index);
        if (currentStudent.getName() == name) {
            studentList.remove(index);
            return true;
        }
    }
    return false;
}
```

# Binary Tree

### Definition
*(empty)*

### Advantages of using "***Binary Tree***"
* Binary search is ***much faster*** than *sequential search*;  
  
* Because it reduces the search space by half in each time;


### Disadvantages of using "***Binary Tree***"
* Binary search is not ***applicable*** to ***unsorted*** data sets;  

  * Because the data must be sorted first which adds to computational cost; 

* It can be difficult to manipulate pointers or references in a binary tree; 

  * Which makes it more difficult to add or delete objects in a binary tree;

>#### M19 17, (b) outline one reason why a linked list may be more suitable than a binary tree in this particular situation 
>* The ease of which pointers or references can be manipulated in a linked list;   
>* Allows easier addition/deletion of objects (compared to a binary tree);  
>* It can be difficult to manipulate pointers or references in a binary tree; 
>* Which makes it more difficult to add or delete objects in a binary tree;

>#### N17 18, (c) Explain how a binary tree structure would allow a more efficient search for the Item object.
>The pl array/Item objects could be read into a binary tree;

> * And placed in order of the item code;
> * (Successive) comparisons between the search item and tree item will reduce the search space by a half (each time);
> * Which results in a faster search than a linear search/ `Olog(n)` is better than `O(n)`;
> * As a linear search might have to loop through the whole list;

## Recursive
### Definition 
When a method calls on itself;  
With a changing parameter;  
There is a base (terminating) case;  

The solution repeats the same algorithm;  
With a changing parameter set;  
Until a terminating case is reached; 

> #### M19 17, (b) outline one reason why the use of a recursive method may be inappropriate for linked lists
>* For a *large* linked list, this would require a *large number* of recursive calls which may cause ***stack overflow***;
>* A linked list only allows for sequential access; Therefore, using recursion ***would not*** lead to any gains in ***efficiency***;

>#### N17 19, (b) without writing code, describe the recursive method palindrome() that returns whether or not a word is a palindrome;
>* The index of last character <= index of the first character; 
>* Otherwise, the first and last letters will be compared; 
>* Returns false if they are not equal; 
>* If they are equal, ***calls the method again***; 
>* With, as its parameter, the word stripped of its first and last letters (can use indices);





