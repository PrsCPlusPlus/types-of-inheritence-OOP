# **Types_of_Inheritance**

## **THEORY**
After using the concept of inheritance, you can use code reusability to increase the program’s efficiency and it also makes the code clean. The diagrammatic illustration above shows how you can combine three redundant classes having common features into one class whose members can be inherited by the other derived classes.

- **Single Inheritance in C++**

The inheritance in which a single derived class is inherited from a single base class is known as the Single Inheritance. It is the simplest among all the types of inheritance since it does not include any kind of inheritance combination or different levels of inheritance. The child class can inherit all the members of the base class according to the visibility mode (i.e., private, protected, and public) that is specified during the inheritance. However, it is optional to define the visibility mode during the inheritance. If you do not define it, it sets the visibility mode to private by default.

![image](https://github.com/Purvansha022609/Inheritance/assets/139473344/009687e9-e1f2-4c50-b683-0bc63a2a28e9)

- Syntax to Implement Single Inheritance in C++

The following syntax can be used to achieve Single Inheritance in C++:

class base_class_1

{

    // class definition

};

class derived_class: visibility_mode base_class_1

{

    // class definition

};

- **Multiple Inheritance**

Multiple Inheritance is the concept of inheritance in C++ by which we can inherit data members and member functions from multiple(more than one) base/parent class(es) so that the derived class can have properties from more than one parent class.


![inheitance](https://github.com/Purvansha022609/Inheritance/assets/139473344/57d078dd-e8a6-4836-a03b-f6300071b338)

- *Syntax of Multiple Inheritance in C++*
  
class BaseClass1

{  
    // Data members of BaseClass1.
    
    // Member functions of BaseClass1.
}  

class BaseClass2

{  
    // Data members of BaseClass2.
    
    // Member functions of BaseClass2.
}  

// Multiple inheritance

class DerivedClass: public BaseClass1, public BaseClass2

{
    // Data members of DerivedClass.
    
    // Member functions of DerivedClass.
}  

- **Multilevel Inheritance**
  
In C++ programming, not only you can derive a class from the base class but you can also derive a class from the derived class. This form of inheritance is known as multilevel inheritance.

![image](https://github.com/Purvansha022609/Inheritance/assets/139473344/924e54c2-b33c-4cbf-a8a5-f8a5ce3fbb62)


class A

{ 

... .. ... 

};

class B: public A 

{

... .. ...

};
class C: public B

{

... ... ...

};
Here, class B is derived from the base class A and the class C is derived from the derived class B.

- **Hierarchical Inheritance**

If more than one class is inherited from the base class, it's known as hierarchical inheritance. In hierarchical inheritance, all features that are common in child classes are included in the base class.

For example, Physics, Chemistry, Biology are derived from Science class. Similarly, Dog, Cat, Horse are derived from Animal class.

![image](https://github.com/Purvansha022609/Inheritance/assets/139473344/e093d725-818f-48b6-8348-87562744ce3c)


- *Syntax of Hierarchical Inheritance*
  
class base_class

{

     ... .. ...
     
}

class first_derived_class: public base_class

{

     ... .. ...
     
}

class second_derived_class: public base_class

{
     ... .. ...
}

class third_derived_class: public base_class 

{

     ... .. ...
     
}

## **ALGORITHM**

- **Single Inheritance Algorithm**:

1.Start

2.Define a base class (parent class) with member variables and member functions. This class represents the common properties and behaviors that will be inherited by the derived class.

3.Define a derived class (child class) that publicly inherits from the base class. This is done using the public access specifier when declaring the inheritance relationship.

4.Add additional member variables and member functions to the derived class as needed. These can be specific to the derived class and can extend or modify the behavior inherited from the base class.

5.Create objects of both the base class and the derived class in the program.

6.Use the objects to access member variables and member functions of both the base and derived classes.

7.End

- **Multiple Inheritance Algorithm**:

1.Start

2.Define multiple base classes (parent classes) with member variables and member functions. Each base class represents a specific set of properties and behaviors.

3.Define a derived class (child class) that publicly inherits from multiple base classes. This is done using a comma-separated list of base classes in the derived class declaration.

4.Add additional member variables and member functions to the derived class as needed. These can be specific to the derived class and can extend or modify the behavior inherited from the base classes.

5.Create objects of both the base classes and the derived class in the program.

6.Use the objects to access member variables and member functions of both the base classes and the derived class.

7.Resolve any ambiguities that may arise due to the inheritance of multiple base classes, especially when two or more base classes have member functions or variables with the same name.

8.End

- **Multilevel Inheritance Algorithm**:

1.Start

2.Define a base class (parent class) with member variables and member functions. This class represents the initial set of properties and behaviors.

3.Define a first-level derived class (child class) that publicly inherits from the base class. This derived class may add or modify properties and behaviors.

4.Define a second-level derived class (grandchild class) that publicly inherits from the first-level derived class. This creates a multilevel inheritance chain.

5.Add additional member variables and member functions to the second-level derived class as needed. These can be specific to the second-level derived class and can extend or modify the behavior inherited from the first-level derived class and the base class.

6.Create objects of the base class, the first-level derived class, and the second-level derived class in the program.

7.Use the objects to access member variables and member functions of all classes involved in the multilevel inheritance chain.

8.End

- **Hierarchical Inheritance Algorithm**:

1.Start

2.Define a base class (parent class) with member variables and member functions. This class represents the common properties and behaviors that will be inherited by multiple derived classes.

3.Define multiple derived classes (child classes), each of which publicly inherits from the same base class. These derived classes will form separate branches of the hierarchy.

4.Add additional member variables and member functions to each derived class as needed. These can be specific to each derived class and can extend or modify the behavior inherited from the base class.

5.Create objects of the base class and multiple derived classes in the program.

6.Use the objects to access member variables and member functions of both the base class and the derived classes.

6.End

## **OUTPUT**

- **Single Inheritance Algorithm**:


![image](https://github.com/RitvikArora22070123094/Types_of_Inheritance/assets/139522395/5596a5e8-6f37-4624-817d-272545bdbf77)



- **Multiple Inheritance**

![image](https://github.com/RitvikArora22070123094/Types_of_Inheritance/assets/139522395/bac7e4de-d512-41cc-affa-66abbe8bacac)


- **Multilevel Inheritance Algorithm**:

![image](https://github.com/RitvikArora22070123094/Types_of_Inheritance/assets/139522395/a5ca182a-53b5-4029-ab11-4075d7ee30f6)


  
- **Hierarchical Inheritance Algorithm**:

![exp14_4](https://github.com/Purvansha022609/Inheritance/assets/139473344/3ad54089-a77c-4beb-9d6e-0a322db553f0)
