## Chapter 7 Classes

### 7.1 
- Encapsulation
    - separate how the class is implemented and what the class can do by its users
    - users have no access to the class member data nor how its operations are defined. Users can only use the functions that are in the class (provide input and expect the class function will work properly and produce a desired outcome)

- member functions
    - when we call a member function, we do so on behalf of an object (an instance of the class is an object. the class itself is not an object, it is a datatype - a blueprint that is used to create objects, which are called instances). 
    - inside a member function, we can refer directly to the members of the object (the instance of the class) on which the function is called. NO need for a member access operator since there is assumed an implicit reference through *this*. 
    - minor side note: const member functions may read, but not write to the data members of the object on which it is called.
        - it is added after the function paramemters, before the body. 
    - member function can be defined (NOT declared) outside of the class function, but must use a scope operator :: to indicate that the function defined is a member function of certain class. 
    
- constructors
    - initialize the data members of a class object. 
    - if no constructor is defined, then the compiler will generate a default constrctor 
        - it will default initialize all members
    - there can be multiple constructors (same as overloading the same function with different parameters)
- struct vs class
    - default access level for struct is public
    - default access level for class is private
    
