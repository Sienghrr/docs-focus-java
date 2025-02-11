			Java Basic Docs

*Introdution:
Variable: in java cannot start with number , it must start with character. and if you want to start your variable with symbol , you only can use  $ or _
but it is not common to start the variable name with symbol. The common start with character.

Naming Convention: if your variable name have only one word then all lowercase , but if your variable name have two words or more then the first word all lowercase and the second word capital the first letter and the rest of it go with lowercase. ex: student , studentName ,dateOfBirth...

*Keywords:

break  : is used to exit loop.
continue : is used to skip line or something in loop.
return : is used to exit function.
super : is used when we want to call parent method in the subclass.
final(variable) : when we want to make it as const variable.
final(method) : when we want our method cannot override.
final(class): when we want our class cannot extends.
static(variable) : it mean class variable .

*Array:

if you want to define the maximum size of that array:
	int[] a = new int [your size here];
	double[] b = new double [your size here];

if you to initialize it:
	int[] a = {1,2,34,5,6}; or
	int[] a = new int []{1};

*Function:

	When you first create function the fields inside () called Parameters, and when you call function the fields inside () called Arguments.

There are two types of function :
void function : is used when you do not want to return the value .
return function : is used when we want to take the result of that function to do with something else.

*Class and object:

	Every class in java programming is inherit from class object.
Class : is a blue-print of the object. fiends and methods in the class , we called it 'Member of the class'.
Object: is the instance or the result that come from the class. and we can use "member of the class" by access through object.field or method.

Access Modifier : private, public , protected , default.

default : can access only the class itself or in the same package.
public: can access every where.
private : can only access only the class itself.
protected: can access in the class , package and subclass.

Method Overloading: it mean in the simple way , when you create the same function name , but have different datatype.
VarArg : it mean that you have parameters in the function as array.
	how to use vararg : datatype... then datatypeName.
	some rules you need to know if you want to use vararg :
	    - in one function you can only have one vararg.
	    - vararg must be the last parameter in the function.

*Constructor:
	
	Constructor is similar to class , but constructor is call immediately when the object of the class is initialize. Constructor have the same name as class but the key different is constructor have no return type.
	There are 3 types of constructor in java programming: NoArg-Constructor , parameterized constructor and default constructor.

NoArg-Constructor: is the constructor that have no parameter inside the ();
Parameterized Constructor: is the constructor that have parameter one or more inside the ();
Default Constructor: is the constructor that create by the java compiler and the structure of default constructor is exactly the same as NoArg-Constructor. the key different is NoArg-Constructor we need to create it by ourselves , but default constructor is create by java compiler automatically.


	Rule how to create and use Constructor:
	-Constructor cannot be an abstract or static or final declaration.
	-Constructor can overload but cannot overridden
	-if you want to call constructor in other constructor , you just use keyword  "this(args)" and it must be the first statement.

*Inheritance:

	Inheritance is a key feature of OOP concept that allow us to create new classes from existed class. And the new class that create from the old one we called it subclass or child class or derived class. And the old class we called it super class or parent class or base class.
	
	In order to perform inheritance , we use keyword "extends".

- Subclass can access every fields and methods of parent class , except that in parent class that field or method declare as a private field or method .
- Parent class cannot access the fields or methods of subclass.

	When we put @overridden on the method it mean that we want to tell the compiler that we want to modify that method of parent class.
	Here are some rules of java overriding:
	-Both the parent class and subclass must have the same method name , same return type and the same parameter list.
	-We cannot override the method declared as final and static.

	sort notice: if this - other (asc) and if other - this (desc)

	
	Why inheritance ?
	- we use inheritance because we want our code reusability , it simply mean that we take the code in parent class to use in subclass instead of writing the same code many times.
	- method overriding is known as runtime polymorphism . so we can get polymorphism through inheritance.

*Abstraction:
	Abstraction is a key feature of oop concept and it allows us to hide some information and show only the information we need to show.
	In order to get abstraction we need to use abstract class and abstract method.

	- abstract class: cannot create object.
	- abstract method : do not need body.
	- we use abstract keyword to create abstract method and abstract class.

To implement feature of abstract class , we inherit subclasses from it and create object of the subclass.
-  A subclass must override all the abstract methods of abstract class. if the subclass is declared as abstract, so that not necessary.

*Interface in java:
	 Interface is a fully abstract class.it includes a group of abstract methods(methods without the body) .
	 - we use interface keyword to create an interface.
	 - implicit = automatically
	 - explicit = need to define

In interface is implicit it mean that our method in the interface although we do not declare as public , it is public.although we do not declare as abstract, it is abstract.
	example for variable in interface:
		int version = 1; = public static final int version =1;

	- the same as abstract class we cannot create object from interface.
	- To use interface other classes must implement it and we use implements keyword to implement an interface
and comma(,) for multiple interfaces.

+ Advantages of interface
- similar to abstract class , interface help us to achieve abstraction in java.
- Interface provides specifications that a class (which implement it) must follow.
- interfaces are also use to achieve multiple inheritance in java.
- if you want to create method that have body in interface , you can achieve that by using default , static and private keyword.
- if you want to extends and also implement , you must extends first and then implements.
 






































