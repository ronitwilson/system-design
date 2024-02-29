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
