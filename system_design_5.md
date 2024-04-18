# 17-apr
## Abstract Data types Use of Obect Oriented Programming
* Recall Object oriented principles
  * Abstraction -> simplify a concept
  * Encapsulation -> bundle data and functions
  * Decomposition -> break a whole into smaller part
  * Generalization -> factor out conceptual commonalities
* Identify data and put them in classes wich is the abstract data type
* Use of structural and behavioural design patterns

## Procedural programming paradigm
* break up the overall functionality of system into main program and subroutines
* Focus is on the data and behaviour of the function and how data moves through them
* Suited for **computation focused**
* Functions are like black box given an input will always have sme output (no state)
![image](https://github.com/ronitwilson/system-design/assets/9934360/2192fe8e-2b1a-4999-8b5d-97c6229837e9)
![image](https://github.com/ronitwilson/system-design/assets/9934360/764e3a91-c06b-4fa8-b464-b859dc7c2873)

## Repository Based Systems Data Centric software architecture
* Databases
* Two main componenents
  * Central Data
    * Component which stores and serve data
  * Data accessors
    * that makes queries and transactions against the information stored
* **Data accessors are sepertated from one another and communicate only through the data component**
* Data integrity and Data Persistence
  * Achived useing DBs
* Charectors of data accessors
  *  share set of data while able to operate independently
  *  Data accessors need not interact with each other
  *  data accessor contains all the business rules required to perform its functions
* advantages of data centric architecture over oops
  * Increased support of data intergrity, data backup, data restoration
  * easy to scale the data storage
  * reduce the need to  transfer the data a lot
* disadvantages
  * Heavily reliant on central data component
  * diffultt to change the existing data schema
  * Data accessors are dependent on what gets stored in the database. New data accessors need to build around the existing data schema

## Layered architecture
* components in a layer only interact with components in adjacent layers
* It allows for **separation of concerns**
    * Many layered systems are split into “presentation,” “logic,” and “data” layers.
    * I can think of the mvc architecture
* Os of a computer is an example of layered system
![image](https://github.com/ronitwilson/system-design/assets/9934360/3131fbd2-7845-418b-8e64-2da59a241cd2)
* Disadvantages
    * There is **overhead**
    * A layer can talk to another only through the ajacent layer
* There are variations possible
    * make room for a top layer to talk to a lower one
    * But it is about trade offs coupling vs flexibility etc
![image](https://github.com/ronitwilson/system-design/assets/9934360/0e2bddc1-8ec0-472a-9e33-f403e6cb5e8a)


