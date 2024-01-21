# system-design

## Design Principles

## 20-Jan-2024
### Coupling Cohesion
* Coupling -> ideally classes should be loosely coupled, so that one obj can be exchnaged for another
* Cohesion -> ideally one class should do only one work..

 ### Information Hiding
 * encapsulation enables this, ex: the public functions are the interfaces what is the actual logic/attribute is hidden inside
 *  Acess modifiers: Public, Private,Protected, Package

 ### Conceptual Integrity
 * Creating consistent software -> even if multiple people work on the software, it would look like it was made from one mind
 * Naming convention like snail_case, Camel case etc
 * Have practices like PR reviews
 * Having interfaces for example help have integrity
 * Having desing practises, Having a clear architecture

 ### Generaliztion Principles
 #### Inheritance issues
 * Be carefull of inherting too much..
 * Follow + Liskov Substitution Principle:- subclass can replace a superclass if and only if, the subclass does not change the functionality of superclass
 * If inheritance does not suit the needs decomposition is an alternative (ex a smartphone si made by seperate phone and camer classes)
 * **overall goal** - reuseable flexible maintainable
  
 ### Modelling Behaviour
  #### Sequence diagrams
 * ![image](https://github.com/ronitwilson/system-design/assets/9934360/4ca9d520-d874-4de8-85d2-e8a29c26cd3c)

## 21-Jan-2024
### Modelling Behaviour
#### States
 * There is sometimes the entry activity
 * The do activity
 * The exit activity
 * It can be repesented like this (example of entry/do/exit state of vending machine)
  * ![image](https://github.com/ronitwilson/system-design/assets/9934360/094da18b-c1ce-4ddb-8a84-ca66a8c1f413)
### Model checking
 * We can use testing to make sure the software is fine as intended
 * How can reason about software
  * We can look at a program as a mathematical artifact
  * We can break down the complex system into smaller state
 * **In model checking we try to make sure system works in small cases (small world asumption)**
 * Not all software peices make sense to do model checking
 * The phases of model checking
  *  Modelling phase
  *  Running phase
  *  Analysis phase
