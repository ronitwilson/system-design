![image](https://github.com/ronitwilson/system-design/assets/9934360/e6466f5d-dea0-494b-b502-c6da105ff52d)# 17-apr
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

## Client Server n-Tier 
* Normally each tier runs on a seperate machine
### client/server 2 tier architecture
* request response model
    * Don't need to worry where the request comes from
    * ![image](https://github.com/ronitwilson/system-design/assets/9934360/813c802e-a43d-4e2e-9413-0c21cc0f11f1)
    * can be scaled more easily
    * but server acts as a central point of failure
    * centralization of computing power and functionality
### 3 tier architecture 
![image](https://github.com/ronitwilson/system-design/assets/9934360/efae2046-dc82-4cbc-8ab3-7227dd9cded2)


# Interpreter Based systems
* Users can write scripts macros, rules that access & compose the basic feature of system in new ways
* Example a component called interpreter is built into the system
    * eg Excel can do run time calulations
* With interpreter end users can add functionality to system & extend existing functionality
    * By composing pre existing function in a specific order to create something new

# State Transition system
*  A state transition system is a concept used to describe the behavior of a system
### Example of state transistio system
![image](https://github.com/ronitwilson/system-design/assets/9934360/180dd56f-1421-43b0-8b79-43f1fdf2bfc7)
### Uses
* Helps determince when important system events/resources are used
* Help understand how parallel process multithreading etc work
* Help identify deadlocks

# Pipe and filter systems
* Very much relateable to the **chain of responsibilty pattern**
### Diagram
![image](https://github.com/ronitwilson/system-design/assets/9934360/45134706-a6cc-42fe-91fd-1d28818c9084)

### Advantages
    * Loose and flexible coupling
    * Filters can be treated as black boxes
    * Reusability,Filters can be reused
    
### Disdvantages  
    * Reduced performance
    * Every filter must parse the input and then perform transformation and then send the data
    * Filters may get overloaded with too much data
    * not suitable for interactive applications as data transfers and transformations take time


# Implicit Invocation systems
* functions are not in direct communication with each other
## Event Based
* **Event bus** and **Event generators** and **Event consumers**
* can be related to observer event pattern
* generators don't need to know about the consumers
* consumers can be **triggered asynchronously**
* Need to **handle race conditions**
  * Use of a Semaphore (use of a key)
* We can predict the **order of the events**
### example event based system  
![image](https://github.com/ronitwilson/system-design/assets/9934360/7a7fcced-0f5d-4ea4-99ae-657fd8e42251)

### Publish subscribe system are also very similar
* This is like a subsystem of event based system
* Note that the components only publish and subscirbe
  * In the event based system, they only create events and handle events
* Note we cant modify a published message
  * Solution would be to have a correction message

# Process Control Systems
* There are feedback loops
* 4 main parts
    * Sensor
    * controller
    * actuator
    * process
* There are closed loop systems
    * The simple one with no external input
* Foreward loop systems
    * The closed loop + external input at the controller logic
### images
![image](https://github.com/ronitwilson/system-design/assets/9934360/7cfba647-c8fc-4c08-bde0-f848d737ef3a)
![image](https://github.com/ronitwilson/system-design/assets/9934360/ad8db9e7-ccfa-42de-a328-01080922cb6b)

