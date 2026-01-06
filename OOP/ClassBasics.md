**Fundamentals of OOP**

**"Class"**
-> UserDefined datatype (an OOP construct), that can be used to encapsulate data and task/functions which operate on the data. \
-> 'function new()' is called the 'constructor' and is automatically called upon object creation. \
-> 'this' is used to refer to the current class. Normally used within the class to refer to its own properties/methods. \

**"Class Constructor"** \
-> 'new()' is called class constructor and is the way to initialize the class variables with some values. \
-> No return type and is non-blocking. \

**"Parameterized Class"** \
-> Much easier to write generic class which can be instantiated in multiple ways to achieve different array size or datatypes. 
-> With parameterized class they can be overridden during class instantiation. 
-> We can also pass parameterize the datatypes which can be overridden in the class.  

"this" \
-> Refers to class properties, parameters and methods of the current instance. \
-> It can be used only within non-static methods, constraints and covergroups. \

"Static" \
-> Static Variable - When a variable is declared as static, that variable will be the only copy in all class instances. \
-> Static Function - Follows scoping and access rules, but the only difference is it can be called outside the class even without class instantiation. It can be called using ":: Scope Operator". \

"Copy" \
-> Shallow Copy - new() All the variables are copied across integers, strings, instance handles. \
-> Deep Copy - copy() Everything (including the nested objects) is copied and typically custom code is required for this purpose. \

"Cast" \
-> Syntax(Dynamic Cast) - $cast \
-> Used when we have different data type variables where ordinary assignment wont be valid. \
-> It can be called in functions(returns 1 if cast is legal) and tasks(assign source expression to target variable, if fails produces a runtime error) also. \
-> Syntax(Static Cast) - '() \
-> Enforces type safety, it doesnt allow casting between incompitible data types. (Evaluated at compile Time) \
-> 


1. Inheritance
   -> Using the properties/ methods of a class in another function/task to perform further operations in the function or task is called inheritence. \
   -> This allows developers to add new properties and methods to new class while maintaining the original class members. (Modification done without touching the old class) \
   -> Syntax to use the class is 'super' and using 'extend' while we declare the class. \

2. Abstract/Virtual Class
   -> Useful when we have to create child classes. \
   -> Useful to enforce testcase developers to always extend a base class to another class for their needs.
   -> Syntax - virtual class <class_name>

3. Polymorphism
   -> Allows the use of a variable of the base class type to hold subclass objects and to reference the methods of those subclasses directly from the subclass. \
   -> It allows child class to have different definition than its parent class method is virtual in nature. \
   -> Virtual methods -  which enable all child classes to override the method with a different definition, but the prototyping returning type and argument shall remain constant. 
   
