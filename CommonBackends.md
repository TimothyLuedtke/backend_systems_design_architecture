# Commonly used architecures

- Monolith
- Distributed (service-oriented)
- Serverless

## Table of Contents

- [Monolith](#monolith)
  - [Pros of Monoliths](#pros-of-monoliths)
  - [Cons of Monoliths](#cons-of-monoliths)
  - [Use Cases of Monoliths](#use-cases-of-monoliths)
- [Distributed (Service-Oriented)](#distributed-service-oriented)
  - [Distributed (Generic Services)](#distributed-generic-services)
  - [Distributed (Microservices)](#distributed-microservices)
  - [Pros of Distributed Systems](#pros-of-distributed-systems)
  - [Cons of Distributed Systems](#cons-of-distributed-systems)
  - [Use Cases of Distributed Systems](#use-cases-of-distributed-systems)
- [Serverless](#serverless)
  - [Pros of Serverless](#pros-of-serverless)
  - [Cons of Serverless](#cons-of-serverless)
  - [Use Cases of Serverless](#use-cases-of-serverless)

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

### **Use Cases of Distributed Systems**

- **E-commerce platforms**: They often need to handle high volumes of transactions and user interactions, which can be efficiently managed through independent micoservices.

- **Social media platforms**: The various functionalities like posting, messaging, and notofications can be divided into separate microservices.

- **Streaming services**: Microservices can help handle
the heavy load and deliver smooth streaming experience.

- **Online gaming platforms**: They can use microservices to manage game logic, player data, and real-time multiplayer interactions separately.

- **Large-scale IoT systems**: Each device or sensor type can be managed by a dedicated microservice.

## Serverless

- **Definition**: Serverless architcecture refers to applications that significantly depend on third-party services(Backend-as-a-Service or BaaS) or on custom code that's run in ephemeral containers(Function-as-a-Service or FaaS).

- **Overview**: Serverless architectures, the app logic is still run on servers, but all the serber management is done by the cloud provider. This allows developers to focus on writing code without worrying about the underlying infrastructure.

### **Pros of Serverless**

- **No Server Management**: Developers do not need to worry about server provisioning, scaling, or maintenance.

- **Cost-Effective**: You only pay for the time your code is running, which can be more cost-effective than traditional server-based architectures.

- **Automated Scaling**: Serverless architectures can automatically scale to meet demand.

### **Cons of Serverless**

- **Expensive for Long-Running Applications**: For applications that run for long periods of time, serverless can be more expensive than traditional server-based architectures.

- **Testing**: Testing serverless applications can be more challenging than traditional server-based applications due to the reliability on the internet.

- **Troubleshooting and Debugging**: Debugging serverless applications can be more challenging due to the distributed nature of the architecture.

### **Use Cases of Serverless**

- **Real-time File Processing**: Serverless functions can be triggered by file uploads to process the files in real-time. *Ex: Image resizing, PDF generation.*

- **Real-time Stream Processing**: Perform real-time analytics on streaming data from sources like IoT devices or social media feeds. *Ex: Processing and analyzing data from sensors.*

- **Extract, Transform, Load (ETL) Jobs**: Serverless functions can be used to process and transform data from one format to another. *Ex: Extracting data from a database, transforming it, and loading it into a data warehouse.*

- **Websites and Web Applications**: Serverless architectures can be used to host static websites or dynamic web applications. *Ex: Hosting a blog, portfolio, or e-commerce site.*

- **Scheduled Tasks**: Serverless functions can be scheduled to run at specific times to perform tasks like data backups or cleanup.
