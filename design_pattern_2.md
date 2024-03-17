# 21-02-2024
## Behavioural Pattern
## Template Method Pattern
* Best used when we generalize 2 classes into a superclass
* so that some implementation specifics can be deffered to subclasses
* It encourages the use of abstract base class and abstract methods
* ![image](https://github.com/ronitwilson/system-design/assets/9934360/83532533-c194-4e48-b04b-fbaa71418457)

## Chain of Responsibility Pattern
* The client object request is passed to a chain of handlers
  * If the handler can process the requests ends with this handler
  * If the handler cannot handle the request, the request  is sent to the next handler in chain
* It is similar to exception handling in Java
* Remember how the carpc software in cubanops works
  * The File wathcer handler -> uploader handler -> archive manager handler
* ![image](https://github.com/ronitwilson/system-design/assets/9934360/1dc9509b-d921-47a9-bf6b-87fb3bdc9e0e)

## State Machine Pattern
* Remember there are states and triggers
* ![image](https://github.com/ronitwilson/system-design/assets/9934360/3ec23feb-a527-4b58-9890-f2fd86745c9a)

## Command Pattern
* The command pattern creates a command object  betwen sender and reciver
* The invoker is a object that invokes the command objects
* Uses
 * Store and schedule different requests
 * Allows commands to be undone and redone
 * Allows commands to ve seperated from the UI
![image](https://github.com/ronitwilson/system-design/assets/9934360/a536f873-7502-47d9-8277-139d71eda64f)

## Observer Pattern
* **Observers** rely on the **subject** to inform them of changes to the state of the subject
* There is Subject superclass -> keeps list of all observers
* There is a Observer interface with a method that can be notified
![image](https://github.com/ronitwilson/system-design/assets/9934360/a0dd9033-6ce6-4ada-9a4f-1e8ff86e8c33)


## Model view Controller Pattern
* Model can be considered like data or state
* View is the interface
* Uses the controller to modify the model
![image](https://github.com/ronitwilson/system-design/assets/9934360/559dd2ed-bf56-49a7-a934-53e67680500d)

## Mediator design pattern
*  Mediator pattern, you will add an object that will talk to all of these other objects and coordinate their activities.
*  The Mediator allows for loose coupling between colleagues. Since each of these colleagues only communicates with the mediator, they can be reused more easily.
*  On the other hand, the mediator can quickly become very large.
![image](https://github.com/ronitwilson/system-design/assets/9934360/3404356e-8e48-409f-8b4e-a0ec88d2874e)
![image](https://github.com/ronitwilson/system-design/assets/9934360/ec7a104d-afa1-46da-9834-fc995a52f33b)

