[[NODE_特性]]

###  **Interface Inheritance** : Implements

**

When a class is a hyponym of an interface, we used implements.

**

Every variable in Java has a “compile-time type”, a.k.a. “static type”.
编译时
- This is the type specified at declaration. Never changes!
Variables also have a “run-time type”, a.k.a. “dynamic type”.
运行时
- This is the type specified at instantiation (e.g. when using new).
- Equal to the type of the object being pointed at.

**Static vs. Dynamic Type** Every variable in Java has a static type. This is the type specified when the variable is declared, and is checked at compile time. Every variable also has a dynamic type; this type is specified when the variable is instantiated, and is checked at runtime.


**Method Overloading** In Java, methods in a class can have the same name, but different parameters. For example, a `Math` class can have an `add(int a, int b)` method and an `add(float a, float b)` method as well. The Java compiler is smart enough to choose the correct method depending on the parameters that you pass in. Methods with the same name but different parameters are said to be overloaded.

**Method Overriding** For each method in class A inherit from Interface B that we also defined in Interface B, we will add an `@Override` right above the method signature. 

**Interface Inheritance** Formally, we say that subclasses inherit from the superclass. Interfaces contain all the method signatures, and each subclass must implement every single signature; think of it as a contract. In addition, relationships can span multiple generations. For example, C can inherit from B, which can inherit from A.

**Default Methods** Interfaces can have default methods. We define this via:

**Dynamic Method Selection** The rule is, if we have a static type `X`, and a dynamic type `Y`, then if `Y` overrides the method from `X`, then on runtime, we use the method in `Y` instead. 


### Implementation Inheritance: Extends

**

When a class is a hyponym of a class, we used extends.

**



It‘s impossible in Java : 

```java
@Override
public String toString() {
    return super.super.toString();
}
```


why:
	It violates encapsulation.You shouldn't be able to bypass the parent class's behaviour.