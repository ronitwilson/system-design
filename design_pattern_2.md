# 21-02-2024
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

