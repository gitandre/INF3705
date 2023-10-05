# Chapter 3 Agile
## 3.1 Agile methods
## 3.2 Agile Development techniques
## 3.3 Agile Project Management
## 3.4 Scaling Agile Methods

---

### 3.1 Agile methods

#### Historical Context
- In the 1980s and 1990s, a plan-driven approach was popular, especially for large, complex systems.
- Such heavyweight approaches were found to be inefficient for small and medium-sized projects due to high overheads.

#### Emergence of Agile Methods
- Developed in the late 1990s as a response to dissatisfaction with heavyweight, plan-driven approaches.
- Focus on the software itself, minimizing design and documentation overheads.
- Suited for rapidly changing requirements and aims to deliver working software quickly.

#### Agile Manifesto Principles
1. **Customer Involvement**: Customers should be closely involved to provide and prioritize new system requirements.
2. **Embrace Change**: The system should be designed to accommodate changing requirements.
3. **Incremental Delivery**: Software should be developed and delivered in increments, based on customer-specified requirements.
4. **Maintain Simplicity**: Focus on simplicity in both the software and the development process.
5. **People, not Process**: Exploit the skills of the development team; avoid prescriptive processes.

#### Core Values (from Agile Manifesto)
- **Individuals and Interactions** over processes and tools
- **Working Software** over comprehensive documentation
- **Customer Collaboration** over contract negotiation
- **Responding to Change** over following a plan

#### Ideal Use-Cases for Agile Methods
1. **Product Development**: Particularly effective for small or medium-sized products for sale.
2. **Custom System Development**: Effective when the customer is committed to being involved and when there are few external stakeholders.

#### Communication and Team Structure
- Agile methods work well when there is continuous communication between stakeholders and the development team.
- Best suited for co-located teams where informal communication is effective.

#### Limitations
- Less suited for systems that are tightly integrated with other systems being developed simultaneously.
- Not ideal for situations requiring coordination of parallel development streams.

![img.png](img.png)

### 3.2 Agile Development techniques

#### Historical Background
- Extreme Programming (XP), coined by Kent Beck, significantly influenced the agile development culture.
- XP aimed to push recognized good practices like iterative development to "extreme" levels.

#### Core Concepts in XP
1. **Requirements as User Stories**: Requirements are expressed as scenarios or user stories implemented as tasks.
2. **Frequent Releases**: Short time gaps between system releases, focusing on incremental development.
3. **Test-First Approach**: Tests are developed for each task before writing the actual code.
4. **Pair Programming**: Programmers work in pairs to cross-verify and support each other.
  
#### XP Practices Aligned with Agile Manifesto Principles
1. **Incremental Development**: Small, frequent releases based on simple customer stories.
2. **Customer Involvement**: Constant customer engagement, with customer representatives defining acceptance tests.
3. **People Over Process**: Practices like pair programming, collective ownership, and sustainable work hours.
4. **Embracing Change**: Regular releases, test-first development, and continuous integration.
5. **Maintaining Simplicity**: Constant refactoring and using simple designs that are easily adaptable.

#### Extreme Programming Practices
1. **Collective Ownership**: All developers are responsible for all code; anyone can change anything.
2. **Continuous Integration**: Completed tasks are immediately integrated into the whole system, passing all unit tests.
3. **Incremental Planning**: Requirements are recorded on "story cards," prioritized based on time and importance.
4. **On-Site Customer**: A customer representative is part of the development team, responsible for conveying system requirements.
5. **Pair Programming**: Developers work in pairs, mutually verifying and supporting each other.
6. **Refactoring**: Code is continuously improved for simplicity and maintainability.
7. **Simple Design**: Only enough design is carried out to meet the current requirements.
8. **Small Releases**: Frequent and incremental releases that add functionality to the initial release.
9. **Sustainable Pace**: Avoiding excessive overtime to maintain code quality and productivity.
10. **Test-First Development**: An automated unit test framework is used to write tests before implementing functionality.

#### Adaptability and Challenges
- XP as originally proposed is difficult to integrate into the management practices and culture of most businesses.
- Companies often pick and choose XP practices that best suit them, sometimes integrating them into other agile methods like Scrum.
- XP's most significant contribution is likely the set of agile development practices it introduced.

![img_2.png](img_2.png)



![img_1.png](img_1.png)


#### 3.2.1 User Stories

#### Overview and Purpose
- User stories are scenarios of use developed to encapsulate customer needs.
- They integrate requirements elicitation with agile development, replacing separate requirements engineering activities.

#### Creation and Usage
1. **Collaborative Development**: The system customer and development team collaborate to develop a "story card" that briefly describes a user story.
2. **Task Breakdown**: Each story card is broken down into tasks, with estimations for effort and resources required.
3. **Customer Prioritization**: The customer prioritizes the stories based on immediate business value.
4. **Short Iterations**: The aim is to implement functionality from prioritized stories in about two weeks, aligning with the next system release.

#### Advantages
- **Dynamic Adaptability**: Unimplemented stories can change or be discarded as requirements evolve.
- **User Engagement**: User stories are more relatable than conventional requirements documents, fostering better user involvement.
  
#### Challenges and Limitations
1. **Completeness**: It's difficult to assess if enough user stories have been developed to cover all essential requirements.
2. **Accuracy**: User stories may not capture all aspects of an activity, especially if experienced users omit details.

#### Application in Requirements Elicitation
- User stories can serve as an initial step in pre-development requirements elicitation, a topic discussed further in future chapters.

![img_3.png](img_3.png)

![img_4.png](img_4.png)


#### 3.2.2 Refactoring

#### Concept and Rationale
- Refactoring is the practice of continually improving software code for better structure and readability.
- It deviates from the traditional software engineering principle of "designing for change," arguing that such anticipation often results in wasted effort.

#### Process
1. **Immediate Implementation**: When developers see code that can be improved, they make these improvements immediately, regardless of immediate necessity.
2. **Avoiding Structural Decay**: Refactoring counters the software structure degradation that naturally occurs in incremental development.
  
#### Types of Refactoring
- Examples include reorganizing class hierarchies, renaming attributes and methods, and replacing duplicated code with library methods.

#### Tools and Support
- Development environments often include tools that simplify the process of finding code dependencies and making global modifications.

#### Benefits
- Keeps the software easy to understand and modify, which is particularly useful as new requirements emerge.

#### Challenges and Limitations
1. **Development Pressure**: Sometimes, new feature implementation takes precedence over refactoring, causing a delay in improvements.
2. **Architectural Limitations**: Some new features and changes may require architectural modifications that cannot be addressed solely through code-level refactoring.


#### 3.2.3 Test-first Development (TDD)

#### Overview
- Originated from Extreme Programming (XP), test-first development is an approach where tests are written before the code that needs to be tested.
- It addresses challenges related to testing in incremental development methodologies.

#### Key Features in XP
1. **Test-First Development**: Tests are written before the code.
2. **Incremental Test Development from Scenarios**: Tests are developed based on user stories or scenarios.
3. **User Involvement**: Users are involved in test development and validation.
4. **Automated Testing Frameworks**: Use of frameworks like JUnit for automated testing.

#### Advantages
- Helps in discovering problems during development.
- Defines an interface and a specification of behavior implicitly.
- Helps in understanding specifications thoroughly before implementation.
- Avoids "test-lag" where implementation outpaces testing.

#### Test Development Process
- User stories are broken down into tasks, each generating one or more unit tests.
- Acceptance tests are developed with customer involvement to ensure the system meets real needs.

#### Role of Automation
- Test automation is essential for quickly and easily executing a large set of tests.
- Catches issues immediately when new functionality is added.

#### Challenges and Limitations
1. **Incomplete Tests**: Programmers may skip writing comprehensive tests.
2. **Difficulty in Incremental Testing**: Some elements, like complex user interfaces, are hard to test incrementally.
3. **Test Coverage**: Despite a large set of tests, it is difficult to ensure complete coverage, leaving potential bugs undetected.

#### Generalization
- The philosophy of test-first has evolved into more general test-driven development techniques.

![img_5.png](img_5.png)


#### 3.2.4 Pair Programming



### 3.3 Agile Project Management


### 3.4 Scaling Agile Methods

#### 3.4.1 Practical problems with agile methods

#### 3.4.2 Agile and plan-driven methods

#### 3.4.3 Agile methods for large systems

#### 3.4.4 Agile methods across organizations


### Summary

- Agile methods are iterative development methods that focus on reducing process overheads and documentation and on incremental software delivery. They involve customer representatives directly in the development process.

- The decision on whether to use an agile or a plan-driven approach to development should depend on the type of software being developed, the capabilities of the development team, and the culture of the company developing the system. In practice, a mix of agile and plan-based techniques may be used.

- Agile development practices include requirements expressed as user stories, pair programming, refactoring, continuous integration, and test-first development.

- Scrum is an agile method that provides a framework for organizing agile projects. It is centered around a set of sprints, which are fixed time periods when a system increment is developed. Planning is based on prioritizing a backlog of work and selecting the highest priority tasks for a sprint.

- To scale agile methods, some plan-based practices have to be integrated with agile practice.

- These include up-front requirements, multiple customer representatives, more documentation, common tooling across project teams, and the alignment of releases across teams.
