# jun 16 Web services
## Enterprise Application Integration (EAI)
  * The use of a middleware as a layer for compatability between components
  *  But these have limitation in Business to business use cases
      *  Who will implement the middleware
      *  Is the data secure
      *  Complexity
  *  Better way than EAI -> web services
### SOAP
    * Use of XML for msg transfer
    
### WSDL ->  Web Services Description Language.
### UDDI

#### The above there are part of first gen Web services

## SOAP 
It is a defined format in xml to invoke an operation
![image](https://github.com/ronitwilson/system-design/assets/9934360/9295cef5-edee-41d4-a80a-60031e7026c9)


### types of SOAP
  * Document type soap -> somthing like sending the feild of a form
  * RPC SOAP -> call a remote service

### SOAP working
SOAP messages are sent over transport protocol.  example HTTP 

##### image 
![image](https://github.com/ronitwilson/system-design/assets/9934360/9123d819-eb78-43b2-811f-6896f98289e3)

### SOAP Message patterns
    * Request-response and a variant called Solicit-response
    * One-way
    * Notification

### Disadvantage 
Main disadvantage overhead with xml headings etc


## WSDL
Web Service Description Language (WSDL) is a standard used to describe the interface of a web service. This helps SOAP messages find services, and understand how to interact with services.

  * WSDL descriptions are machine-readable
  * This allows service descripter to generate machine readable code to interface with service automaitcally (binding)

 ### WSDL 2.0 parts
   *  Types -> discribe the datatype
   *  Interfaces -> what operation can be performed

## **Service Publication and Discovery (UDDI)**

Web services need to be published and discovered. Developers need to be able to find services to build apps, and there needs to be a way to get people to use these created services.
The first framework for publishing was **Universal Description, Discovery, and Integration (UDDI)**

### UDDI General working
* UDDI allows service providers to publish their services to a UDDI registry.
* Once they are published, potential service requesters can search the registry and discover the service they need.
* Once the service that the service requester wants to use is found, the service requester can bind to it using the WSDL description
* Once bind is done the service requester can invoke

#### UDDI image
![image](https://github.com/ronitwilson/system-design/assets/9934360/22e3e3c1-15fe-409d-b5fd-8bb3fa222ba9)

#### UDDI Publishing
* White pages -> overview business name
* Yello pages -> more info contains info about service
* Green pages -> contains technical details

## Service Composition BPEL - Business Process Execution Language (BPEL)
Composing services involves invoking services in a certain order and handling exceptions that may arise. 
* Basic services often have low-level, basic functionality.
* This functionality can be combined into higher level functionality with Business Process Execution Language (BPEL)
    * Lower-level details of inter-service communication are dealt with by protocols such as SOAP and WSDL
### Cordination
Coordination is when a process coordinates the activities of two or more services.


## Rest 
* URI
* Using HTTP header to specify format
  *   Content type/accept
* Using Query in URL
* Using Ofset and filtering in URL
* Versioning APIs
* HTTP status codes

### Microservices
Service oriented architecture
#### Advantages
* Each service can be autonomous
* Easy to scal some parts
* Services can be updated seperately
#### Disadvantages
* Complex
* the limitation of being a distributed system
    * Some centralized management of all microservices will be required
    * Database consistency needs to be maintained
    * Testing is complex
* Crucial service failing may be a bottlenect
* overhead in services communicating to one another
