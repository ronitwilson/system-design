# 29-01-2024
## Design patterns overview
* There are about 23 famous design patterns
### Gang of four
* Creational patterns -> example we make a copy of object, instead of creating each time
* Structural patterhn -> How objects relate to each other
  * Think about terms
    * Decomposistion
    * Generalization
    * Association, Aggregation, Compsition, inheritance, interface
* Behavioural patterns -> how they work together to obtain a goal

## 8-02-2024
### Singleton Pattern (Creational)
* only one object will be alive..
* Constructor is private
* getInstance object

## 8-02-2024
### Factory Method Pattern (Creational)
* Option of using a **factory object** patter (not the actual fatory method)
 *  ![image](https://github.com/ronitwilson/system-design/assets/9934360/ce79f5a1-d33f-412a-8378-4872b00dfc6c)
 *  Note there is KnifeFactory which creates the necessary knife obj
* Acutal factory Mehtod pattern
 *  ![image](https://github.com/ronitwilson/system-design/assets/9934360/366b2ec7-f488-4988-a7bf-5b029db57bba)
 *  ![image](https://github.com/ronitwilson/system-design/assets/9934360/5b570343-16f1-40a6-926d-80d712681659)

## 8-02-2024
### Facade Pattern (Structural)
* provide simplified interface for client to interact with a subsystem
* a wrapper class which encapsulates a subsystem in order to hide the subsystem complexity
*  ![image](https://github.com/ronitwilson/system-design/assets/9934360/a91c2e7f-7e06-4f47-a57c-6b7f8f123880)
* **Steps**
 *  Design the interface
 *  Implement the interface with one or more classes
 *  Create the facade class & wrap the class that implements the interface
 *  use facade class to access the subsystem

## 8-02-2024
### Adapter Pattern (Structural)
* ![image](https://github.com/ronitwilson/system-design/assets/9934360/39b7a1a6-3a27-4312-ad70-6b6ba0164a7c)
* **Steps**
 * Design the target interface
 * Implement the target interface with the adapter class
 * send request from cline to adapter using the target interface
* ![image](https://github.com/ronitwilson/system-design/assets/9934360/282a20e3-dc93-416a-beb9-098455134cdb)

## 8-02-2024
### Composite Pattern (Structural)
* To compose nested structures of objects.
* To deal with classes for these objects uniformly.
* ![image](https://github.com/ronitwilson/system-design/assets/9934360/b13c128c-ef05-4eb4-908b-12f07affdc88)

* An abstract class can be used instead of an interface.
* Notice how the composite class holds a array of composite objects.
* ![image](https://github.com/ronitwilson/system-design/assets/9934360/ba048bbe-9d98-487d-9039-ea8a98467d03)




