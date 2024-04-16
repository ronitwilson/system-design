# April 5 2024
## Kruchten’s 4+1 View Model
### Logical view
### Process iew
### development view
### Physical view

# Apr 8 2024
## Logical view
* Functional requirements of a system
* Use of **class diagram** n **State diagrams**
* Helps to see database schemes
* can see how classes interact

## Process view
* Non functional requirements like **performance** and **availability**
* presents the process that corrospond to objects in  logical view, it assumes all methods are implemented it cares to define in what order and how to execute
* **activity diagram and sequence diagrams**

## Development  view
* Describes the hierachical software structure.
* It considers what **program lang to use libs toolset**
* concerned with the details of development
* Can also involve budgeting project management etc

## Physical view
* UML deployment diagram
* describes how elements in logical process and development view are mapped to different nodes


# Component Diagrams
* Can be used earlyon in design 
* Example of how a pizza in a menu shows the different ingredients but not its details
* identify the main objects used in the system, relebant libs and how the relationship between the components
![image](https://github.com/ronitwilson/system-design/assets/9934360/6b647bd1-a35f-4a22-a3a4-a0bc1e2be505)

# UML Package Diagram
* Defines the namespace
* it could include data, classes or even other packages
* Provides a high-level groupings of the system
* It has a import and access field
* Import is public the name is visible for further imports through the level package
* access is private imports, these are not known outside the user namespace
  ![image](https://github.com/ronitwilson/system-design/assets/9934360/61776e6a-d2e9-4323-83c3-9aeec749252e)
* Helps to understand namespaces

# UML Deployment Diagram
* Helps to understand all the files and executables involved and environments where they reside
* It deals with **artifacts**
  * they are physical result of deployment proces
  * eg excutalbe, libs assets
* 2 types of deployment diagram
  * specification-level diag
    * top level does not reference specific instance or nodes
  * instance level diag
    * can be used to show different deplyments like development, staging, production etc
* **Manifestation** is a relationship where an artifact is a physical realization of software component.
![image](https://github.com/ronitwilson/system-design/assets/9934360/1ee333c2-b629-4911-8d62-5b422f1fb339)
![image](https://github.com/ronitwilson/system-design/assets/9934360/39cc17be-053b-4061-81a0-2b3497e0b02c)

