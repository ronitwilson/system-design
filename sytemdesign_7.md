# Service oriented Architecture
* We can make use of other's laready built services
* The flow is asyncchronus

## Two main classification
### Services on Internet
* example flight price service
### Services on large orgs
* example the service department may provide a service to know about support costs in the software.

## Service Principles
* Modular and loosley cuples
* Platform and language independent
* Self describing  -> exmaple **WSDL web service description language**
* Self-Advertising -> example **Universal description Discovery and Integration (UDDI)**

## Service oriented architecture example
![image](https://github.com/ronitwilson/system-design/assets/9934360/08eb6c61-1716-49b9-8862-1a0cd8904034)


## HTTP
### HTTP 1.1 -> URI and URL 
![image](https://github.com/ronitwilson/system-design/assets/9934360/1e523431-fe7f-45aa-b4d9-34fbacc2f82d)

### Client server model

### Request model
![image](https://github.com/ronitwilson/system-design/assets/9934360/cd21cc87-2624-4dec-b638-a6c78fd38560)

### Respnse  model
![image](https://github.com/ronitwilson/system-design/assets/9934360/c527de2f-f693-47fc-85ee-b77992b510f5)

### URI encoding
* We can't use some charecter like spaces which is encoded like %02 etc

### HTTP methods
* GET POST PUT DELETE MODIFY

### example request response
![image](https://github.com/ronitwilson/system-design/assets/9934360/7543fc98-1e53-4eaf-8a7c-b4d5724f4e5e)

## RPC
  * The client and server are on different machine/ different virtual instance of same machine
  * address space between client and server is different

### IDL - Interface language definiton
  * IT is the specification for remote procedure calls
#### example architecture
![image](https://github.com/ronitwilson/system-design/assets/61230302/41803a97-a8eb-45da-ab9f-c5a44ec326ca)
### Client stub
  * establish the connection
  * Format the data to standardized structure
  * Send the remote procedure call
  * reveive the server stub response
### Server stub
  * invoke the desired procedure 

### Interface Headers
* Tells the client what procedures are remotely accessible
* TellsThe actual procedure that is being invoked on server
* Tells the procedure call that is invoked b broadcaset\

### Steps during the rpc call
  * Client component invokes the procedure
  * Client stub marshalls the parameters
  * Message is sent to server
  * The server stub receives and unmarshalls the message
  * The server executes the procedure
  * The result is sent back to server stub
  * the result is given to client stub
  * the client stub unmarshall and process the results

## Object Brokers
RPCs with the class/object based approach is called  Object brokers

#### CORBA 
The most common object broker architecture is the **Common Object Request Broker Architecture (CORBA)**

#### Object request broker
  * Provides object interoperability.
  * A obj declares its interfaces before it can be accessed by client or sever through the broker
  * Broker is responsible for marshalling and unmarshalling

#### CORBA services
  * services provided by the middleware to objects 

#### CORBA facilities
  * high level function as document management

#### CORBA architecture 
Insert picture here..

#### CORBA IDL
SImilar the IDL at the RPC , but supports inheritance and polymorphism.

#### Static and Dynamic Interoperability
  * **Static binding** occurs when the client stub is created. The service that is used for static binding to a broker is handled by the IDL. **When the IDL compiler generates the stub, it will be statically bound to the broker** that the IDL compiler belongs to.
  * **Dynamic binding **is also specified in CORBA. It allows clients to dynamically search for new objects using service discovery

#### CORBA facilities
