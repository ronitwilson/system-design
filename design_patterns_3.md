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
 
# 5-apr-2024
##  Anti patterns and code smells
* **too many comment**s is not good
* **Do not repeat yourself**
* **Long methods** are more complex and hence not a good patern
* **Large classes** are not good
 *  Classes should have a explicit purpose
*** Data class too many** is not good
 * These are too small classes with only getter and setter
* **Data clumps** -> groups of data always occuring together but not in the same class
* Logn Parameter list -> have a prameter object
* **Divergent change** it occurs when you have to change a clas in many different ways for different reasons
 * classes are too large and complex
* **Shotgun Surgery** occurs when a change needs to be made to one requirement but numerous classes all over the design need to be touched to make that change
* **Feature envy** -> a methods is more interested in the details of a class other than the one it is in
 *  chances are the method is in the wrong class
*  **Inappropriate intimacy** 2 classes depend too much on one another
 *  classes are circular dependent
 *  It can be a necessarily
 *  Methods can be factored out so that both classes use a third class
*  **Message chains**  wehn we are chaining objecs to reach a particular methods
 *  breaks law of demeter
*  **Primitive Obsession** we we use built in types too much 
*  **Switch statements** if there are too many swithc statements scattered throught a program
 *  Possible use of polymorphism
*  **Speculative Generality** when you make the super class too general speculating about the future
 *  Use Just in time design
*  **Refused Request** sub class inherits somethigns but does not need it
