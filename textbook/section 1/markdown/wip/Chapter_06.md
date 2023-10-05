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






### 6.2 Architectural Views






### 6.3 Architectural patterns

#### 6.3.1 Layered Architecture

#### 6.3.2 Repository Architecture

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