describes a reusable solution to a commonly needed behavior.
Those from "Design Patterns" book are listed first.
## Creational
About how to create objects
### Factory method
Provide an way for creating a **single** object, but let subclasses decide which class to instantiate. Provides [[oop concepts|polymorphism]] to object creation, not only object use.

Use the Factory Method pattern when
- a class can't anticipate the class of objects it must create
- a class wants its subclasses to specify the objects it creates
- classes delegate responsibility to one of several helper subclasses, and you want to localize the knowledge of which helper subclass is the delegate
Use simple constructors otherwise.

ex. a constructor for MenuItem, not for every item separately, so that calling code doesn't have to know what specific MenuItem it wants to create. 
#### abstract factory method
Provide an way for creating **families** of related or dependent objects without specifying their concrete classes by encapsulating a group of individual factories that have a common theme without specifying their specific classes. 

### Singleton
Ensure a class has only one instance, and provide a global point of access to it. The pattern is useful when exactly one object is needed to coordinate actions across a system.
### Builder
Separate the construction of a complex object from its representation, allowing the same construction process to create various representations.
### Prototype
Specify the kinds of objects to create using a prototypical instance, and create new objects from the 'skeleton' of an existing object, thus boosting performance and keeping memory footprints to a minimum.
### Dependency Injection
A class accepts the objects it requires from an injector instead of creating the objects directly.
Dependency injection aims to separate the concerns of constructing objects and using them, leading to loosely coupled programs.

In statically typed languages using dependency injection means that a client only needs to declare the interfaces of the services it uses, rather than their concrete implementations, making it easier to change which services are used at runtime without recompiling.
### Object pool
Avoid expensive acquisition and release of resources by recycling objects that are no longer in use.

## Structural
about how to organize objects intro structures
### Adapter

### Bridge 

### Composite

### Decorator

### Facade

### Flyweight

### Proxy
### Delegation


## Behavioral
about how to communicate between objects
### Chain of responsibility 
delegates commands to a chain of processing objects.
### Command
creates objects that encapsulate actions and parameters.
### Interpreter
implements a specialized language.
### Iterator
accesses the elements of an object sequentially without exposing its underlying representation.
### Mediator
allows loose coupling between classes by being the only class that has detailed knowledge of their methods.
### Memento
provides the ability to restore an object to its previous state (undo).
### Observer
is a publish/subscribe pattern, which allows a number of observer objects to see an event.
### State
allows an object to alter its behavior when its internal state changes.
### Strategy 
allows one of a family of algorithms to be selected on-the-fly at runtime.
### Template method 
defines the skeleton of an algorithm as an abstract class, allowing its subclasses to provide concrete behavior.
### Visitor
separates an algorithm from an object structure by moving the hierarchy of methods into one object.
### Null object 
Avoid null references by providing a default object.
### Servant 
Define common functionality for a group of classes. The servant pattern is also frequently called helper class or utility class implementation for a given set of classes. The helper classes generally have no objects hence they have all static methods that act upon different kinds of class objects.


## Concurrency
about how to handle concurrent processing