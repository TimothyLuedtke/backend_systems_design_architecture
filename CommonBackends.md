# Commonly used architecures

- Monolith
- Distributed (service-oriented)
- Serverless

## Monolith

- **Definition**: A monolithic architecture is a traditional unified model for designing software where the different components of the application are combined into a single program from a single platform.

- **Overview**: Thi architecture is simple to develop, test, and deploy. It is also easy to scale vertically by adding more resources to the server. However, it can be difficult to scale horizontally, and the entire application needs to be redeployed when changes are made.

### **Pros of Monoliths**

- **Simplicity**: Easier to develop, est and deploy due to the unified system.

- **Efficiency**: Since all the functionalities are interconected, it can be more efficient in terms of inter-process communication.

### **Cons of Monoliths**

- **Limited Scalability**: Scaling specific functions of a system is not possible. The entire system needs to be scaled.

- **Lack of Flexibility**: Changes to a single component can require the entire system to be redeployed.

- **Complexity**: The system can become too complex and hard to manage as the application grows.

### **Use Cases of Monoliths**

- **Small-scale applications**: Given its simplicity, monolithic architecture is ideal for small-scale applications or startups where the application's scope is clear and unlikely to drastically change or scale.

- **Applications with simple, well-defined business processes**: Monolithic architecture can be beneficial in scenarios where the business processes are simple and unlikely to require significant changes or additions.

- **Applications where high performance is critical**: Since all functionalities are interconnected, a monolithic architecture can provide faster inter-process communication compared to other architectures.

## Distributed (Service-Oriented)

- **Definition**: Generic services and/or microservices architecture is a method of developing software systems that are loosely coupled and independently deployable smaller sevices, which run in their own processes.

- **Overview**: This architecture allows for continuous delivery and deployment of large, complex applications. It also enhances an organization's capability to innovate and reduces the time to market for new features.

### Distributed (Generic Services)

- **Definition**: **Generic services** often refers to a component of an application that provides a specific functionality or service. These services are typically designed to be reusable across multiple applications.

- **Overview**: **Generic services** can be used to provide common functionality across multiple applications, reducing the need for duplicate code and improving maintainability.

### Distributed (Microservices)

- **Definition**: **Microservices** are a variant of the service-oriented architecture (SOA) structural style that arranges an application as a collection of loosely coupled services.

- **Overview**: **Microservices** are designed to be small, focused, and independently deployable services that work with other "services" using protocols such as HTTP/REST or messaging queues to provide the functionality of a larger application. This architecture allows for greater flexibility, scalability, and resilience compared to monolithic architectures.

### **Pros of Distributed Systems**

- **Independent Development**: Each service can be developed independently by a team that is focused on that service.

- **Independent Deployment**: Services can be deployed independently.

- **Fault Isolation**: A process failure should not bring the entire system down.

- **Mixed Technology Stack**: Different services can use different technologies.

### **Cons of Distributed Systems**

- **Distributed System Complexity**: Developers must deal with the additional complexity of creating a distributed system.

- **Development and Testing**: Writing and testing applications is more difficult due to it being distributed system.

- **Data Management**: Managing data consistency can be challenging.
