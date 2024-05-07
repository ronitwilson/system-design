
# Architecuteal Trade offs
## Quality Attributes
* System architectues **are not inherently good or bad**
* It is about meeting the requirements
### a table on some attributes
![image](https://github.com/ronitwilson/system-design/assets/9934360/d3277e0c-5f0f-4ee7-bdea-3a92135458c1)
![image](https://github.com/ronitwilson/system-design/assets/9934360/a6e398d9-6ab0-4705-822e-9511126677ad)
![image](https://github.com/ronitwilson/system-design/assets/9934360/97726100-8799-4db2-8c62-76454d590786)
### other points
* A a good practice to try to minimize complexity of design
* It is important to have detailed and up-to-date docu
### Design porcess guide lines
* Recognise the important quality attribs and prioritize them
    * Trade-offs should be noted
* involve a tech lead in design process
    * will help **identify any implementations that can pose a challenge**
* Taking a design approaches from perspective of diff stake holders

### Analyzing and Evaluatiing an Architecture
### General procedure
![image](https://github.com/ronitwilson/system-design/assets/9934360/6cba2457-8db6-491f-8389-8b6996bbcf49)


### Explainations
![image](https://github.com/ronitwilson/system-design/assets/9934360/ce711afb-84b4-469d-9b68-35e5c3c40243)

### Notes
* In the context of analyzing and evaluating architecture, you should focus on situations that are outside of the normal execution path

## Architecute trade-off Analysis (ATMAM Architecute trade-off Analysis Method)
### Participands
* Evaluation Team
    * Designers - involved with arch design, anayzing system requirement
    * Peers - part ofproject but not involved in design process
    * Outsiders - no involment in project but should have experience in analyzing architecute 
 * Project decision makers
 * Architecure stake holders
### high level picture
![image](https://github.com/ronitwilson/system-design/assets/9934360/f299c824-7d37-4e8a-a0ee-d156d8bdf5b8)

### ATAM process
#### Present the ATAM
#### Pressent the business drivers
#### Present the architecute
* both current and expected state of architecute
#### Identify the architecutral approaches
* analyse the architectural patterns used in the system
#### create a quality attribute tree
* get the achitecture significant requirement (ASR)
![image](https://github.com/ronitwilson/system-design/assets/9934360/9241387d-d2d0-4385-9950-ffaefd3367df)
#### Analyze the architectural approaches
* This allows for the identification and documentation of risk and non-risk **scenarios, sensitivity points, and trade-offs**
* Connection between business drivers and system arrchitecutes
#### Brainstorm and prioritize scenarios
#### Re-analuze the arch approaches
#### Present the result

# Relationship to Org structure 7 may
## Conway's Law
* Software  will tend to take a form that is congruous to the organization that produced it
    * knowledge of Conway’s Law should result in planning development teams around the desired architecture
    * For example, if you are building a web application using the n-Tier architecture, you could
        * have one team for the data backend,
        * one team for the application logic layer
        *  one for the presentation tier.
## Product Line and Product families
### Product lines have several advantages
* product lines help reduce development cost per product
* similar user experience across products in the product line
* reduce time to market of the newer producets in the product line
* having only less products in product line is not a good idea
#### Product line flow chart 
![image](https://github.com/ronitwilson/system-design/assets/9934360/98d36090-a432-42b9-ba63-60a4b9a02ba3)

### Teams in product line
* **Domain engineering** focus on the commanlities and variations (infrastructre for the pdl)
*  **Application engineering** focus on integrating the commanalities and variations n make the product
