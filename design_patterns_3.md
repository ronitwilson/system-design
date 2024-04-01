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
* based on cocepts **coupling** -> how strongly coupled a module is
* **cohesion** -> how clear it is the role of a module
* how easy it is to replace a dependency
 * how easy to replace one class with another
* High level modules should depend on high level generalizations and not on low level details
![image](https://github.com/ronitwilson/system-design/assets/9934360/409e02e9-0240-4282-8022-f5e8cb0c4afb)
![image](https://github.com/ronitwilson/system-design/assets/9934360/ab8a1be8-c344-4459-ac70-47bd54084179)
* built against interfaces not concrete clases

## Composing Objects Principle
* another approach to inheritance
* works similar to the decorator patterns, where a object is worked on by other classes.
* using interface means all lengthy inherited child class has all the methods and attribs fo the super class
* will lose the benifit of code reuseablity which comes with inheritance
![image](https://github.com/ronitwilson/system-design/assets/9934360/6f028e9f-986e-43a7-b0aa-45916bf4761b)


## Interface Segregation Principle
* if there is a single interface which holds all the methods then all clients will have to implement all methods just to make theri dependency compile
* large interfaces should be split into smaller ones

# 1-apr-2024
## Principle of least knowledge
* classes should know and interact with as few classes as possible
* coupling is reduced
* Law of demeter
* 4 rules
 ![image](https://github.com/ronitwilson/system-design/assets/9934360/0c5fa8be-9b4c-48d0-b765-d5f46a4de68e)
* **reaching through** of methods needs to be prevented
 *  chain of methods calls to obj you should not know
 *  when you receive an object of unknown type
 
