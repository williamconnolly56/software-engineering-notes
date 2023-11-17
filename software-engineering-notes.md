# **Monolithic software architecture**


## *Key characteristics*


- Single Codebase - The entire application is developed, built, and deployed from a single codebase.
- Tight Integration - Components of the application are tightly coupled and share the same memory space.
- Single Deployment Unit - The entire application is deployed as a single unit.


## *Advantages*


- Simplicity - Can be simpler to develop and understand.
- Ease of deployment - Often less complex than deploying a distributed system.
- Performance -  All components are tightly integrated and communication between them is more efficient compared to distributed systems.
- Development speed -  Enables faster development in the early stages of a project as focus can be on building features and not managing the communication between distributed components.


## *Disadvantages*


- Development bottlenecks - Multiple developers working on the same codebase may lead to conflicts, and coordinating changes can be complex.
- Technology stack - A single technology stack is used for the entire system so If new technologies need to be incorporated, it may require significant refactoring.
- Fault tolerance - If one part of the application fails, it can bring down the entire system.
- Scaling - It can be challenging to scale individual components independently. If a specific feature or module requires more resources, scaling the entire monolith might be necessary.


## *Application - Minimum Viable Products (MVPs)*


A monolithic architecture can enable rapid development and deployment of MVPs. It simplifies the development process and helps to quickly validate concepts before possibly transitioning to a more complex architecture. As the application and its requirements grow, more modular and scalable architectures like microservices might become preferable to address evolving needs.


## *Software architectures comparison*


| Characteristic | Monolithic | Microservices |
| -------- | ------- | ------- |
| Architecture | All components are tightly integrated into a single codebase. | Different functionalities are broken down into independent self-contained units (microservices) with their own codebases and databases. |
| Scalability | Typically scaled by replicating the entire application. Relatively inflexible when scaling individual components independently. | Enables granular scalability by independently scaling specific microservices. |
| Development and deployment  | Easier to develop and deploy initially. Changes may require redeploying the entire application. | Allows independent development and deployment of microservices. |
| Technology stack | Typically uses a single technology stack for the entire application. Changing to a new technology often involves significant refactoring.| Permits the use of different technologies for different microservices. |
| Fault isolation | Limited fault isolation; a failure in one component may affect the entire system. | Improved fault isolation; a failure in one microservice does not necessarily impact others. |
| Team structure | Coordination is required when multiple developers are working on the same codebase. | Facilitates larger teams as each microservice can be developed and maintained independently. |
| Communication between components | Components communicate directly within the application code. | Communication often occurs via APIs, HTTP, or message queues. |
| Resource utilization | Resource allocation is uniform for all components which may be suboptimal. | Enables more efficient resource utilization. |


## *Diagram*


![monolithic](https://github.com/williamconnolly56/software-engineering-notes/assets/146080335/c277f40e-9c95-4c09-ab0c-383ab22d6f35)


## References


- https://www.techtarget.com/whatis/definition/monolithic-architecture 
- https://www.atlassian.com/microservices/microservices-architecture/microservices-vs-monolith 
- https://microservices.io/patterns/monolithic.html 
- https://www.openlegacy.com/blog/monolithic-application 
- https://medium.com/koderlabs/introduction-to-monolithic-architecture-and-microservices-architecture-b211a5955c63 
- https://www.geeksforgeeks.org/monolithic-architecture/ 

