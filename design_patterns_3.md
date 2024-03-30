# 26-03-204
## Liskov Sibstitution principle
* its about inheritence
*  a subclass is expected to have the same characteristics and behave in the same way.
*  If a class, S, is a subtype of a class, B, then S can be used to replace all instances of B without changing the behaviors of a program
*  Invariant conditions that exist in the base class, must also remain invariant in the subclass
*  Immutable characteristics of a base class must not be changed by the subclass

## Open/closed principle
* Open for extension
* Closed for modification
* Although the principle is called “closed”, it does not mean that changes cannot be made to a class during developmen
* 2 ways to be open for extension
  * inheritence of a superclass
  * implementation of abstract class
* option to use final keyword to close classes

# 30-03-204
## Dependency inversion principle
* based on cocepts coupling -> how strongly coupled a module is
* cohesion -> how clear it is the role of a module
* how easy it is to replace a dependency
 * how easy to replace one class with another
* High level modules should depend on high level generalizations and not on low level  
