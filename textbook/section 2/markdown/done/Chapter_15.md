# Chapter 15 Software reuse:
## 15.1 The reuse landscape
## 15.2 Application frameworks
## 15.3 Software product lines
## 15.4 Application system reuse

---

#### **Note:** Images excluded due to time constraints

---

### 15.1 The Reuse Landscape

#### Overview
- Software **reuse** has evolved over the past 20 years, offering various techniques to support different levels and types of reuse. The choice of reuse technique depends on several key factors, including system requirements, development team expertise, and the software's criticality.

#### Types of Reuse Techniques

1. **Application Frameworks**: Collections of classes adapted and extended to create systems.
2. **Architectural Patterns**: Standard software architectures used as application bases.
3. **Component-based Software Engineering**: Systems developed by integrating standard components.
4. **Configurable Application Systems**: Domain-specific systems designed for specific customer needs.
5. **Design Patterns**: Generic abstractions represented as patterns.
6. **ERP Systems**: Large-scale systems configured for an organization.
7. **Legacy System Wrapping**: Legacy systems accessed through defined interfaces.
8. **Model-driven Engineering**: Code generated from domain and implementation-independent models.
9. **Program Generators**: Systems generated from user-supplied models.
10. **Program Libraries**: Class and function libraries for common abstractions.
11. **Service-oriented Systems**: Systems developed by linking shared services.
12. **Software Product Lines**: Applications adapted around a common architecture for different customers.
13. **Systems of Systems**: Integration of two or more distributed systems to create a new system.

#### Key Factors for Planning Reuse

1. **Development Schedule**: For rapid development, reusing complete systems is preferable.
2. **Software Lifetime**: For long-lifetime systems, focus on maintainability and long-term implications.
3. **Team Expertise**: Reuse technologies are complex; focus on areas where the team has expertise.
4. **Software Criticality**: For critical systems requiring certification, having source code access is crucial.
5. **Application Domain**: In domains like manufacturing and medical systems, generic products can often be configured for local needs.
6. **Platform Compatibility**: Some components or systems may be platform-specific.

#### Generator-based Reuse
- **Generator-based reuse** embeds domain-specific solutions into automated tools, allowing users to create new systems effectively.

#### Managerial Considerations
- The decision to reuse often hinges more on **managerial willingness** than technical feasibility. Managers may prefer known risks of development over unknown risks of reuse. To promote reuse, it may be necessary to introduce a company-wide reuse program.

---

### 15.2 Application Frameworks

#### Overview
- **Application frameworks** are larger-grain abstractions in object-oriented development that support design reuse and class reuse. They provide a skeleton architecture and reusable components for a family of related applications.

#### Characteristics of Frameworks
1. **Language-Specific**: Implemented in object-oriented programming languages like Java, C#, C++, Ruby, and Python.
2. **Extensibility**: Can incorporate other frameworks and can be extended using features like inheritance and polymorphism.

#### Types of Frameworks
1. **Web Application Frameworks (WAFs)**: These are the most widely used and are usually based on the Model-View-Controller (MVC) Composite pattern.
2. **System Infrastructure Frameworks**: Support the development of system infrastructures like communications and user interfaces.
3. **Middleware Integration Frameworks**: Support component communication and information exchange (e.g., Microsoft’s .NET, Enterprise Java Beans).
4. **Enterprise Application Frameworks**: Concerned with specific application domains but have been largely superseded by software product lines.

#### Components in Web Application Frameworks (WAFs)
1. **Security**: Classes for user authentication and access control.
2. **Dynamic Web Pages**: Classes for defining web page templates.
3. **Database Integration**: Abstract interface to different databases.
4. **Session Management**: Classes for creating and managing user sessions.
5. **User Interaction**: Support for AJAX and/or HTML5, device-independent interfaces.

#### Implementation Considerations
- **Inversion of Control**: Framework objects control the flow, invoking “hook methods” in response to events, which are then linked to user-provided functionality.
- **Callbacks**: Methods that are called in response to events recognized by the framework.

#### Challenges and Limitations
- **Complexity**: Frameworks are inherently complex and require time to learn.
- **Evaluation**: Difficult and expensive to evaluate and choose the most appropriate framework.
- **Debugging**: More challenging due to the complexity and interactions between framework methods.

### 15.3 Software Product Lines

#### Overview
- **Software Product Lines** are sets of applications with a common architecture and shared components, adapted for specific customer requirements. They are effective for supporting multiple similar systems, thus enabling high levels of code and test reuse.

#### Core Elements of a Product Line
1. **Core Components**: Infrastructure support that usually remains unchanged.
2. **Configurable Components**: Can be modified and configured for new applications.
3. **Specialized Components**: Domain-specific elements that may be replaced in new instances.

#### Development Process
1. **Elicit Stakeholder Requirements**: Use an existing system to gather requirements.
2. **Select Closest-Fit System**: Choose an existing product closest to the new requirements.
3. **Renegotiate Requirements**: Make adjustments based on planning and new details.
4. **Adapt Existing System**: Develop new modules and adapt existing ones.
5. **Deliver New Product**: Document its features for future reuse and perform any deployment-time configurations.

#### Types of Specialization
1. **Platform Specialization**: Adapt for different operating systems.
2. **Environment Specialization**: Adapt for different hardware and peripherals.
3. **Functional Specialization**: Adapt for specific customer needs.
4. **Process Specialization**: Adapt to specific business processes.

#### Configuration Stages
1. **Design-Time Configuration**: Modification of the core product line for creating new systems.
2. **Deployment-Time Configuration**: A generic system is specialized at the time of deployment using configuration data.

#### Comparison with Application Frameworks
1. **Object-Oriented Features**: Frameworks rely on inheritance and polymorphism; product lines may not.
2. **Domain-Specificity**: Frameworks are usually general; product lines are often domain-specific.
3. **Hardware Support**: Product lines often support hardware interfacing; frameworks usually don't.
4. **Ownership**: Product lines are usually owned by the same organization and adapted from the closest family member.

#### Challenges and Considerations
- **Balance between Reuse and Customization**: Striking a balance can lead to quicker delivery and lower costs.
- **Reconfiguration Complexity**: Deployment-time configuration can be complex and time-consuming.

#### Tools and Support
- Software tools like configuration planning tools may support the complex process of deployment-time configuration.

---

### 15.4 Application System Reuse

#### Overview
- **Application System Products** are software systems adapted for multiple customers without changing the source code. Also known as COTS (Commercial Off-the-Shelf System) products, they are designed for general use and thus have high reuse potential.

#### Advantages of Application System Reuse
1. **Rapid Deployment**: Faster rollout of reliable systems.
2. **Transparency**: Easier to judge suitability due to existing implementations.
3. **Reduced Risks**: Mitigates some development risks.
4. **Resource Efficiency**: Businesses can focus on core activities.
5. **Technology Updates**: Simplified, as they are the vendor's responsibility.

#### Challenges and Risks
1. **Adapting Requirements**: May necessitate changes to existing business processes.
2. **System Assumptions**: Businesses might need to adapt to the system's underlying assumptions.
3. **System Selection**: Difficult due to poor documentation, wrong choices can be costly.
4. **Lack of Local Expertise**: Dependence on vendor or external consultants.
5. **Vendor Control**: Risks related to vendor business stability or changes.

#### Types of Application Systems
1. **Individual Systems**: Single-vendor generic applications tailored to customer needs.
2. **Integrated Systems**: Combination of functionalities from multiple vendors to create a new system.

#### Focus Areas in Development
- **Individual Systems**: Focus is on **system configuration**.
- **Integrated Systems**: Focus is on **system integration**.

#### Maintenance Responsibility
- **Individual Systems**: Vendor is responsible for maintenance.
- **Integrated Systems**: System owner is responsible for maintenance.

#### Platform Provision
- **Individual Systems**: Vendor provides the platform.
- **Integrated Systems**: System owner provides the platform.

#### Summary of Differences
- **Individual Systems** are based on a generic solution and standardized processes, while **Integrated Systems** offer flexible solutions for customer processes.
  
#### Application System Integration
- Further discussion on integration is mentioned to be covered in Section 15.4.2.


#### 15.4.1 Configurable application systems 


#### 15.4.2 Integrated application systems 

Integrated application systems include two or more application systems or, sometimes, legacy systems. You may use this approach when no single application system meets all of your needs or when you wish to integrate a new application system with systems that you are already using. The component systems may interact through their APIs or service interfaces if these are defined. Alternatively, they may be composed by connecting the output of one system to the input of another or by updating the databases used by the applications. To develop integrated application systems, you have to make a number of design choices: 1. Which individual application systems offer the most appropriate functionality? Typically, several system products will be available, which can be combined in different ways. If you don’t already have experience with a particular application system, it can be difficult to decide which product is the most suitable. 2. How will data be exchanged? Different systems normally use unique data structures and formats. You have to write adaptors that convert from one representation to another. These adaptors are runtime systems that operate alongside the constituent application systems. 3. What features of a product will actually be used? Individual application systems may include more functionality than you need, and functionality may be duplicated across different products. You have to decide which features in what product are most appropriate for your requirements. If possible, you should also deny access to unused functionality because this can interfere with normal system operation. 458    Chapter 15  ■  Software reuse Client Web browser Email system Server E-commerce Ordering and Adaptor system invoicing system Figure 15.14 An Email system Adaptor integrated procurement system Consider the following scenario as an illustration of application system integration. A large organization intends to develop a procurement system that allows staff to place orders from their desk. By introducing this system across the organization, the company estimates that it can save $5 million per year. By centralizing buying, the new procurement system can ensure that orders are always made from suppliers who offer the best prices and should reduce the administration associated with orders. As with manual systems, the system involves choosing the goods available from a supplier, creating an order, having the order approved, sending the order to a supplier, receiving the goods, and confirming that payment should be made. The company has a legacy ordering system that is used by a central procurement office. This order processing software is integrated with an existing invoicing and delivery system. To create the new ordering system, the legacy system is integrated with a web-based e-commerce platform and an email system that handles communications with users. The structure of the final procurement system is shown in Figure 15.14. This procurement system should be a client–server system with standard web browsing and email systems used on the client. On the server, the e-commerce platform has to integrate with the existing ordering system through an adaptor. The e-commerce system has its own format for orders, confirmations of delivery, and so forth, and these have to be converted into the format used by the ordering system. The e-commerce system uses the email system to send notifications to users, but the ordering system was never designed for this purpose. Therefore, another adaptor has to be written to convert the notifications from the ordering system into email messages. Months, sometimes years, of implementation effort can be saved, and the time to develop and deploy a system can be drastically reduced by integrating existing application systems. The procurement system described above was implemented and deployed in a very large company in nine months. It had originally been estimated that it would take three years to develop a procurement system in Java that could be integrated with the legacy ordering system. 15.4  ■  Application system reuse    459 Service wrapper Application system Figure 15.15 Application wrapping Services Services Application system integration can be simplified if a service-oriented approach is used. Essentially, a service-oriented approach means allowing access to the application system’s functionality through a standard service interface, with a service for each discrete unit of functionality. Some applications may offer a service interface, but sometimes this service interface has to be implemented by the system integrator. Essentially, you have to program a wrapper that hides the application and provides externally visible services (Figure 15.15). This approach is particularly valuable for legacy systems that have to be integrated with newer application systems. In principle, integrating application systems is the same as integrating any other component. You have to understand the system interfaces and use them exclusively to communicate with the software; you have to trade off specific requirements against rapid development and reuse; and you have to design a system architecture that allows the application systems to operate together. However, the fact that these products are usually large systems in their own right, and are often sold as separate standalone systems, introduces additional problems. Boehm and Abts (Boehm and Abts 1999) highlight four important system integration problems: 1. Lack of control over functionality and performance Although the published interface of a product may appear to offer the required facilities, the system may not be properly implemented or may perform poorly. The product may have hidden operations that interfere with its use in a specific situation. Fixing these problems may be a priority for the system integrator but may not be of real concern for the product vendor. Users may simply have to find workarounds to problems if they wish to reuse the application system. 2. Problems with system interoperability It is sometimes difficult to get individual application systems to work together because each system embeds its own assumptions about how it will be used. Garlan et al. (Garlan, Allen, and Ockerbloom 1995), reporting on their experience integrating four application systems, found that three of these products were event-based but that each used a different model of events. Each system assumed that it had exclusive access to the event queue. As a consequence, integration was very difficult. The project 460    Chapter 15  ■  Software reuse required five times as much effort as originally predicted. The schedule was extended to two years rather than the predicted six months. In a retrospective analysis of their work 10 years later, Garlan et al. (Garlan, Allen, and Ockerbloom 2009) concluded that the integration problems that they discovered had not been solved. Torchiano and Morisio (Torchiano and Morisio 2004) found that lack of compliance with standards in many application systems meant that integration was more difficult than anticipated. 3. No control over system evolution Vendors of application systems make their own decisions on system changes, in response to market pressures. For PC products in particular, new versions are often produced frequently and may not be compatible with all previous versions. New versions may have additional unwanted functionality, and previous versions may become unavailable and unsupported. 4. Support from system vendors The level of support available from system vendors varies widely. Vendor support is particularly important when problems arise as developers do not have access to the source code and detailed documentation of the system. While vendors may commit to providing support, changing market and economic circumstances may make it difficult for them to deliver this commitment. For example, a system vendor may decide to discontinue a product because of limited demand, or they may be taken over by another company that does not wish to support the products that have been acquired. Boehm and Abts reckon that, in many cases, the cost of system maintenance and evolution may be greater for integrated application systems. The above difficulties are life-cycle problems; they don’t just affect the initial development of the system. The further removed the people involved in the system maintenance become from the original system developers, the more likely it is that difficulties will arise with the integrated system. K e y P o i n t s ■ There are many different ways to reuse software. These range from the reuse of classes and methods in libraries to the reuse of complete application systems. ■ The advantages of software reuse are lower costs, faster software development, and lower risks. System dependability is increased. Specialists can be used more effectively by concentrating their expertise on the design of reusable components. ■ Application frameworks are collections of concrete and abstract objects that are designed for reuse through specialization and the addition of new objects. They usually incorporate good design practice through design patterns. Chapter 15  ■  Website    461 ■ Software product lines are related applications that are developed from one or more base applications. A generic system is adapted and specialized to meet specific requirements for functionality, target platform, or operational configuration. ■ Application system reuse is concerned with the reuse of largescale, off-the-shelf systems. These provide a lot of functionality, and their reuse can radically reduce costs and development time. Systems may be developed by configuring a single, generic application system or by integrating two or more application systems. ■ Potential problems with application system reuse include lack of control over functionality, performance, and system evolution; the need for support from external vendors; and difficulties in ensuring that systems can interoperate.