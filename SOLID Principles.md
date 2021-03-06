# SOLID Principles

#### _Single Responsibility_
There should never be more than one reason for a class to change. Essentially: a class should exist for one purpose only. If you create a class to represent a SalesOrder, you wouldn't want that class to save to the database and export an XML receipt.

Loose Coupling instead encourages objects that receive input from other objects not to have to know what the other object is doing. The other object's only responsibility is to return the correct data; it doesn't matter if the way it accesses that data changes if the objects are loosely coupled. 

#### _Open/Closed_
Software entities (classes, modules, functions, etc) should be open for extension, but closed for modification. By using abstraction--placing responsibility in derivative classes--you can create classes that do the same thing differently without changing the base functionality. 

If properties of the abstracted class need to be compared or organized together, another abstraction should handle this. This is the basis of the "keep all variables private" argument.

#### _Liskov Substitution_

Functions that point to or reference a base class must be able to use objects of derived classes without knowing it. 

#### _Dependency Inversion Principle_
Depend on abstractions, not on concretions. High-level modules should not depend on low-level modules. Both should depend upon abstractions. Abstractions should not depend upon details. Details should depend upon abstractions. 

#### _Interface Segregation Principle_
Clients should not be forced to depend upon interfaces they do not use. "When a client depends on a class that contains interface that they don't use, but that other clients do use, then that client will be affected by the changes those other clients force upon the class."