# Chapter 6 Architectural Design

## 6.1 Architecture Design Decisions
## 6.2 Architectural Views
## 6.3 Architectural patterns
## 6.4 Application Architectural

---

### Architectural Design

1. **Definition and Role**: 
    - Architectural design is about designing the overall structure of a software system.
    - It links requirements engineering to design by identifying main structural components and their relationships.
    - The output is an architectural model that shows how the system's components communicate.

2. **In Agile Processes**: 
    - Early stages focus on architectural design.
    - Incremental development of architecture is not effective; refactoring architecture is expensive.

3. **Overlap with Requirements Engineering**: 
    - In practice, architectural design often overlaps with requirements engineering.
    - Main components may be identified during the requirements phase to facilitate discussions with stakeholders.

4. **Levels of Abstraction**: 
    - Architecture in the Small: Focuses on individual programs and their decomposition.
    - Architecture in the Large: Concerned with complex enterprise systems and their interconnections.

5. **Importance and Impact**: 
    - Affects performance, robustness, distributability, and maintainability.
    - Non-functional requirements significantly influence the architecture.

6. **Advantages of Explicit Architecture**: 
    1. Facilitates stakeholder communication.
    2. Aids in early-stage system analysis.
    3. Supports large-scale reuse through product-line architectures.

7. **Modeling Techniques**: 
    - Block diagrams are commonly used but are criticized for their lack of detail.
    - More rigorous architectural description languages exist but are not widely used due to their complexity and cost.

8. **Contradictions in Practice**: 
    - Architectural models serve two purposes:
        1. Encouraging discussions about system design for stakeholder communication and project planning.
        2. Documenting a fully fleshed-out architecture to facilitate system understanding and evolution.

Architectural design is a critical phase in the software development process, serving as the bridge between requirements and implementation. While it plays a significant role in influencing various system attributes, the ways in which architectural models are created and used can vary, often depending on project-specific needs and constraints.

![img_44.png](img_44.png)

### 6.1 Architecture Design Decisions

1. **Nature of Architectural Design**: 
    - Not a formulaic process; depends on the system, the architect's experience, and specific requirements.
    - Considered a series of decisions rather than a sequence of activities.

2. **Structural Decisions**: 
    - Architects make key structural decisions that impact both the system and its development.
    - These decisions often depend on the architect's knowledge, experience, and the domain of the application.

3. **Reuse and Domain Similarities**: 
    - Systems in the same domain often share architectural similarities.
    - Architects should identify what can be reused from existing architectures within the same or broader application classes.

4. **Distributed vs. Localized Systems**: 
    - The choice between a distributed and a localized architecture is crucial, especially for large systems.
    - This choice affects performance and reliability.

5. **Architectural Patterns and Styles**: 
    - Based on well-known patterns like client–server or layered architectures.
    - Patterns capture the essence of architectures used in different systems.

6. **Non-Functional Requirements and Architecture**: 
    - Architecture style should depend on non-functional requirements such as:
        1. Performance: Localize critical operations to reduce component communications.
        2. Security: Use layered structures with higher validation for innermost layers.
        3. Safety: Co-locate safety-related operations to simplify validation and provide fail-safes.
        4. Availability: Include redundant components for higher availability.
        5. Maintainability: Use fine-grained, self-contained components for easier changes.

7. **Potential Conflicts**: 
    - Trade-offs may be necessary when multiple non-functional requirements are important.
    - Different architectural patterns may be used for different parts of the system to balance conflicting requirements.

8. **Evaluation of Architectural Design**: 
    - Difficult to evaluate definitively, as the true test comes when the system is in use.
    - Comparing against reference architectures or generic patterns can provide some level of evaluation.

Architectural design is a complex and creative process that involves a series of crucial decisions. These decisions are influenced by various factors including the type of system, the architect's background, and specific functional and non-functional requirements. The chosen architecture profoundly affects the system's performance, security, and other attributes, necessitating careful consideration and sometimes trade-offs among conflicting requirements.

![img_45.png](img_45.png)

### 6.2 Architectural Views

1. **Purpose of Architectural Models**: 
    - Used for discussing software requirements or design.
    - Serve as documentation for detailed design and implementation.

2. **Multiple Views for Complexity**: 
    - A single diagram cannot capture all aspects of a system's architecture.
    - Multiple views are often needed for both design and documentation.

3. **Krutchen’s 4+1 View Model**: 
    - Krutchen suggests four fundamental architectural views linked through use cases:
        1. **Logical View**: Shows key abstractions as objects or object classes.
        2. **Process View**: Shows runtime composition of interacting processes.
        3. **Development View**: Shows software decomposition for development.
        4. **Physical View**: Shows distribution of software components across hardware.

4. **Hofmeister's Conceptual View**: 
    - Hofmeister et al. add a "Conceptual View" that serves as an abstract representation of the system.
    - Useful for decomposing high-level requirements and informing architectural decisions.

5. **Informality vs Formality in Notations**: 
    - UML often used informally for architecture description.
    - Some argue for more specialized Architectural Description Languages (ADLs), but these are less accessible to non-specialists.

6. **Agile Perspective on Documentation**: 
    - Detailed design documentation is often seen as unnecessary in agile methods.
    - Focus is on developing views useful for communication rather than complete documentation.

In summary, architectural views serve to capture different aspects of a system's design and are crucial for both discussion and documentation. While there are formal methods and notations, such as UML and ADLs, the industry often leans towards more informal, accessible representations, especially in agile environments. Different architects and methodologies propose various sets of views, but the emphasis is on capturing what is most useful for the project's specific needs.


![img_46.png](img_46.png)

### 6.3 Architectural patterns

1. **Introduction and Origin**: 
    - Patterns are stylized, reusable solutions in software engineering.
    - The concept gained traction with a book on object-oriented design patterns (Gamma et al. 1995).

2. **Other Types of Patterns**: 
    - Exist in organizational design, usability, cooperative interaction, and configuration management.

3. **Architectural Patterns vs Styles**: 
    - Initially proposed as "architectural styles" in the 1990s.
    - Detailed handbooks published on pattern-oriented software architecture.

4. **Definition and Utility**: 
    - Architectural patterns are abstract descriptions of tried and tested good practices.
    - They include information on when to use them and their strengths and weaknesses.

5. **Model-View-Controller (MVC) as an Example**: 
    - Commonly used for interaction management in web-based systems.
    - Descriptions often include pattern name, brief description, graphical model, and example usage.

6. **Graphical Representations**: 
    - Patterns can be illustrated from different views, like conceptual and runtime system architectures.

7. **Scope and Limitations**: 
    - Not all generic patterns can be described due to space limitations, but selected examples provide insights into good architectural design principles.

In summary, architectural patterns offer a formalized way to introduce tried and tested system organizations into new projects. These patterns can vary in type and application but generally include guidelines on when and how to use them. They are often visually represented to give both conceptual and practical insights into their structure and utility.

![img_49.png](img_49.png)

![img_48.png](img_48.png)

![img_47.png](img_47.png)

#### 6.3.1 Layered Architecture

1. **Fundamental Concepts**: 
    - Separation and independence are key to architectural design.
    - Allows for changes to be localized within the system.

2. **Layered Architecture Purpose**: 
    - Achieves separation and independence by organizing system functionality into separate layers.
    - Each layer relies only on the layer immediately beneath it.

3. **Advantages**:
    - **Incremental Development**: Allows for the incremental release of services as layers are developed.
    - **Changeability and Portability**: A new layer can replace an existing one without affecting the rest of the system, provided the interface remains the same.
    - **Localizing Dependencies**: Makes it easier to adapt to different operating systems or databases, as only machine-dependent layers need to be changed.

4. **Example Structure**: 
    - Four-layer example consists of:
        1. System support software layer (e.g., database and OS support).
        2. Application layer with application functionality and utility components.
        3. User interface management, authentication, and authorization layer.
        4. Top layer focused on user interface facilities.
    - The number of layers is arbitrary and can be adjusted as needed.

5. **Real-world Examples**: 
    - iLearn digital learning system and Mentcare system both employ a four-layer architecture following this pattern.

In summary, the Layered Architecture pattern organizes a system into separate, interdependent layers to achieve modularity, ease of development, and change resilience. This architecture is flexible, allowing for incremental development and adaptability to different technological platforms.

![img_52.png](img_52.png)

![img_51.png](img_51.png)

![img_50.png](img_50.png)

#### 6.3.2 Repository Architecture

1. **Core Concept**:
    - Focuses on how a set of interacting components can share data through a centralized database or repository.

2. **Applicability**: 
    - Suited for systems where data is generated by one component and used by another.
    - Examples include command and control systems, management information systems, CAD systems, and software development environments.

3. **Advantages**:
    - **Efficient Data Sharing**: Eliminates the need to transmit data explicitly between components.
    - **Version Control**: Can include features like versioning and rollback.

4. **Challenges**:
    - **Data Model Compromise**: All components must agree on a repository data model, which could be a limiting factor for integrating new components.
    - **Distribution Difficulty**: Logically centralized repositories can be technically challenging to distribute over multiple machines due to consistency and data duplication issues.

5. **Variations**:
    - **Passive Repository**: Control is managed by the components using the repository.
    - **Blackboard Model**: An alternative used in AI systems where the repository triggers components based on the availability of certain data.
  
In summary, the Repository Architecture pattern is useful for systems that require efficient sharing of large amounts of data between components. It comes with its own sets of advantages and challenges, including efficient data sharing but also potential difficulties with data model agreement and distribution. Various models like the passive repository and blackboard model offer different approaches to control and data availability.

![img_53.png](img_53.png)

![img_54.png](img_54.png)

#### 6.3.3 Client-Server Architecture

#### 6.3.4 Pipe and Filter Architecture









### 6.4 Application Architectural

#### 6.4.1 Transactional Processing Systems

#### 6.4.2 Information Systems

#### 6.4.3 Language Processing Systems

---

### Summary

- A software architecture is a description of how a software system is organized. Properties of a system such as performance, security, and availability are influenced by the architecture used.

- Architectural design decisions include decisions on the type of application, the distribution of the system, the architectural styles to be used, and the ways in which the architecture should be documented and evaluated.

- Architectures may be documented from several different perspectives or views. Possible views include a conceptual view, a logical view, a process view, a development view, and a physical view.

- Architectural patterns are a means of reusing knowledge about generic system architectures.

- They describe the architecture, explain when it may be used, and point out its advantages and disadvantages.

- Commonly used Architectural patterns include model-view-controller, layered architecture, repository, client–server, and pipe and filter.

- Generic models of application systems architectures help us understand the operation of applications, compare applications of the same type, validate application system designs, and assess large-scale components for reuse.

- Transaction processing systems are interactive systems that allow information in a database to be remotely accessed and modified by a number of users. Information systems and resource management systems are examples of transaction processing systems.

- Language processing systems are used to translate texts from one language into another and to carry out the instructions specified in the input language. They include a translator and an abstract machine that executes the generated language.

---