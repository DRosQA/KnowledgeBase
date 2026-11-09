(The idea that...)

## Encapsulation
…every object should manage its own state, and not let others manage it directly.

ex. Pizza(MenuItem) has its own properties of price and name, and methods to change them, but doesn't expose them directly outside so that outside code has to change them according to rules defined in Pizza

## Inheritance
…classes should share information the have in common, inheriting from a template where possible, and specializing down the line. 

ex. Pizza is a MenuItem

## Composition
…where possible, objects should be built from smaller, separate objects (components), instead of everything belonging to one giant class.

ex. MenuCombo class contains components for Pizza(MenuItem) and Drink(MenuItem)

## Abstraction
…details of implementation should be hidden inside classes, and only relevant info/data should be exposed. 
In OOP, not entirely related to [[oop elements|abstract class and abstract method]].

ex. Pizza(MenuItem) only exposes price, and doesn't show how its calculated outside, because things that just want to know the price don't care about taxes and retail margins

## Polymorphism
…values should be accessible in different ways so that they can be reused more. Often achieved by sharing an access way at a base level via inheritance, method overloading, or using a generic/base class instead of specific one in implementation.

ex. int and float are polymorphic because both are **numbers** and can both use math operators.
ex. int and "2".ToInt() are polymorphic ad hoc, because both can use math operators
ex. Pizza(MenuItem) and Drink(MenuItem) are polymorphic because both can use order_from_menu()

See also [[general concepts|duck typing]]