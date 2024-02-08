#29-01-2024
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
### Factory Method Pattern
* Option of using a **factory object** patter (not the actual fatory method)
 *  ![image](https://github.com/ronitwilson/system-design/assets/9934360/ce79f5a1-d33f-412a-8378-4872b00dfc6c)
 *  Note there is KnifeFactory which creates the necessary knife obj
* Acutal factory Mehtod pattern
 * ![image](https://github.com/ronitwilson/system-design/assets/9934360/366b2ec7-f488-4988-a7bf-5b029db57bba)
 * ![image](https://github.com/ronitwilson/system-design/assets/9934360/5b570343-16f1-40a6-926d-80d712681659)

## 8-02-2024
### Facade Pattern
* provide simplified interface for client to interact with a subsystem
* a wrapper class which encapsulates a subsystem in order to hide the subsystem complexity
* Steps
 *  Design the interface
 *  Implement the interface with one or more classes
 *  Create the facade class & wrap the class that implements the interface
 *  use facade class to access the subsystem
*  ![image](https://github.com/ronitwilson/system-design/assets/9934360/a91c2e7f-7e06-4f47-a57c-6b7f8f123880)

