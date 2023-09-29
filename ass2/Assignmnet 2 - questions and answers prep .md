
## Question 1 [10 marks]
**Describe how technological advancements can cause a software subsystem to undergo change or risk becoming useless?**

### Answer:
These advancements can lead to changes or obsolescence:

1. **Need for Continuous Testing:** Technological advancements necessitate continuous testing activities to ensure that the software subsystem remains compatible and functional. [1 mark, Chapter 8]
  
2. **Business and User Expectations:** Changes in business environments and user expectations require the software to evolve continuously. [1 mark, Chapter 9]

3. **Maintainability and Adaptability:** New requirements emerge over time, requiring the software to adapt and remain maintainable. [1 mark, Chapter 10]

4.**High Availability (HA):** Systems must evolve to meet high availability requirements, especially in critical applications. [1 mark, Chapter 11]

5. **Component Reuse:** Technological advancements allow for the reuse of components, which can be integrated into new or existing systems. [1 mark, Chapter 15]

6. **Web Services:** Advancements in web technologies have led to the development of web services, enabling more flexible system architectures. [1 mark, Chapter 18]

7. **System Evolution:** Over time, systems naturally evolve to incorporate new features and requirements, but they also risk becoming obsolete if they don't adapt to technological changes. [1 mark, Chapter 19]

In summary, technological advancements are a double-edged sword for software subsystems. On one hand, they offer new possibilities for improvement and adaptation; on the other hand, they introduce challenges that can make existing subsystems obsolete if not properly managed. Therefore, it's crucial for software subsystems to adapt to technological advancements to remain useful and relevant. [3 marks]

---
## Question 2 [15 marks]
**What are the strategic options for legacy system evolution?**

### Answer:
Based on extended information found in Chapter 9 (Software evolution) of "source_text_1," here are the strategic options for legacy system evolution:

1. **Scrap the System Completely**: This option should be chosen when the system is not making an effective contribution to business processes. This usually occurs when business processes have changed since the system was installed and are no longer reliant on the legacy system. [3 marks, Chapter 9]

2. **Leave the System Unchanged and Continue with Regular Maintenance**: This option should be chosen when the system is still required but is fairly stable, and the system users make relatively few change requests. [3 marks, Chapter 9]

3. **Reengineer the System to Improve its Maintainability**: This option should be chosen when the system quality has been degraded by change and where new change to the system is still being proposed. This process may include developing new interface components so that the original system can work with other, newer systems. [3 marks, Chapter 9]

4. **Replace All or Part of the System with a New System**: This option should be chosen when factors, such as new hardware, mean that the old system cannot continue. (Note: The text was cut off at this point, so further details are not available.) [3 marks, Chapter 9]

**Additional Option (Based on Domain Knowledge)**:
5. **Migrate to a Cloud-based Solution**: Organizations sometimes consider migrating legacy systems to the cloud to improve scalability and reduce costs. [3 marks, Domain Knowledge]

In summary, managing legacy systems involves a strategic approach that can range from scrapping the system entirely to reengineering or replacing it. These options need to be carefully evaluated based on the system's current state, user requirements, and technological advancements. [Total: 15 marks]

---
## Question 3 [15 marks]
**Explain why it is reasonable to assume that the use of dependable processes will lead to the creation of dependable software?**

### Answer:
Based on the information found in Chapter 10 (Dependable systems) of "source_text_1," here are the reasons why it's reasonable to assume that the use of dependable processes will lead to the creation of dependable software:

1. **Fewer Errors**: Dependable processes are likely to lead to delivered software that contains fewer errors. The reduction of errors is crucial for creating software that is less likely to fail in execution. [3 marks, Chapter 10]

2. **Proper Enactment and Documentation**: Companies using dependable processes can be sure that the process has been properly enacted and documented. This ensures that all development stages are traceable and accountable. [3 marks, Chapter 10]

3. **Appropriate Development Techniques**: Dependable processes ensure that appropriate development techniques have been used, especially for critical systems development. These techniques often adhere to industry standards and best practices. [3 marks, Chapter 10]

4. **Attributes of Dependable Software Processes**: Dependable processes possess attributes such as reliability, maintainability, and security, which are also essential for dependable software. [3 marks, Chapter 10]

**Additional Point (Based on Domain Knowledge)**:
5. **Quality Assurance**: Dependable processes usually include rigorous quality assurance methods like

 code reviews, testing, and validation, which contribute to software dependability. [3 marks, Domain Knowledge]

In summary, the use of dependable processes is crucial for achieving software dependability. These processes incorporate several aspects like error reduction, proper documentation, and the use of appropriate development techniques, all of which contribute to creating software that is reliable, secure, and maintainable. [Total: 15 marks]

---
## Question 4 [10 marks]
**What are the common characteristics of all architectural styles that are meant to supporting software fault tolerance?**

### Answer:
Based on the information found in Chapter 11 (Reliability engineering) of "source_text_1," here are the common characteristics of architectural styles meant for supporting software fault tolerance:

1. **Protection Systems**: One of the common features of architectural styles supporting fault tolerance is the inclusion of protection systems. These systems help in safeguarding the software against unexpected failures. [2 marks, Chapter 11]

2. **Self-Monitoring Architectures**: Another common characteristic is the use of self-monitoring architectures that can detect faults and trigger corrective actions automatically. [2 marks, Chapter 11]

3. **N-Version Programming**: The architectural styles often use N-version programming to create multiple versions of the system, aiming to ensure that not all versions fail simultaneously. [2 marks, Chapter 11]

4. **Software Diversity**: While difficult to achieve, architectural styles for fault tolerance aim for software diversity to ensure that each version of the software is independent, thereby reducing the chance of simultaneous failure. [2 marks, Chapter 11]

5. **Redundancy**: Dependable programming in these architectures often includes redundancy as checks on the validity of inputs and the values of program variables. [2 marks, Chapter 11]

In summary, architectural styles meant for supporting software fault tolerance often incorporate features like protection systems, self-monitoring architectures, N-version programming, software diversity, and redundancy. These features aim to ensure that the software remains operational even in the face of unexpected faults or failures. [Total: 10 marks]

---
## Question 5 [15 marks]
**List four types of systems that may require software safety cases, explaining why safety cases are required per each system?**

### Answer:
Based on the information found in Chapter 12 (Safety engineering) of "source_text_1," and supplemented by domain knowledge, here are four types of systems that may require software safety cases and why these safety cases are required:

1. **Aviation Systems**: Software in aviation systems controls critical aspects like navigation, communication, and flight control. Safety cases are required to demonstrate that the software meets strict safety standards and can handle a wide range of emergency situations. [3 marks, Chapter 12]

2. **Medical Devices**: Devices like infusion pumps and medical imaging systems are highly dependent on software. Safety cases are essential to ensure that the software doesn't malfunction, leading to incorrect diagnosis or treatment, which could be life-threatening. [3 marks, Chapter 12]

3. **Nuclear Power Plants**: Software controls various operations, including reactor temperature and security measures. A safety case is crucial to demonstrate that the software can handle failures without leading to catastrophic outcomes like a meltdown. [3 marks, Chapter 12]

4. **Automotive Systems**: Modern vehicles are equipped with various software-controlled systems like anti-lock braking systems (ABS) and airbags. Safety cases are needed to ensure these systems function correctly under all conditions, reducing the risk of accidents. [3 marks, Chapter 12]

**Additional Point (Based on Domain Knowledge)**:
5. **Reason for Safety Cases**: A common reason for requiring safety cases across these systems is that a high percentage of system malfunctions are the result of specification rather than design errors. Safety cases aim to identify and mitigate such errors. [3 marks, Domain Knowledge]

In summary, systems like aviation, medical devices, nuclear power plants, and automotive systems require software safety cases to ensure that they meet strict safety standards and can handle a wide range of operational and emergency situations. These safety cases are critical for demonstrating the system's ability to operate safely and effectively. [Total: 15 marks]

---
## Question 6 [10 marks]
**How is reuse and reconfiguration made easier by the product line's basic application design?**

### Answer:
Based on the information found in Chapter 15 (Software reuse) of "source_text_1," and supplemented by domain knowledge, here are the ways in which reuse and reconfiguration are made easier by the product line's basic application design:

1. **Standardized Components**: In a product line, the basic application design often includes standardized components that can be easily reused in various applications. This saves time and resources in development. [2 marks, Chapter 15]

2. **Modularity**: The basic design in a product line is usually modular, which allows for easier reconfiguration. Modules can be added, removed, or replaced without affecting the entire system. [2 marks, Chapter 15]

3. **Pre-configured Solutions**: Product lines often come with pre-configured solutions that can be fine-tuned to meet specific requirements, making the reconfiguration process quicker and less prone to errors. [2 marks, Chapter 15]

4. **Documentation**: Adequate documentation is usually available in a product line's basic application design, which makes it easier for developers to understand how to reuse or reconfigure components. [2 marks, Chapter 15]

**Additional Point (Based on Domain Knowledge)**:
5. **Design Patterns**: Product lines often utilize design patterns that are known to be reusable and easily configurable, which aids in both reuse and reconfiguration. [2 marks, Domain Knowledge]

In summary, the basic application design in a product line facilitates easier reuse and reconfiguration through standardized components, modularity, pre-configured solutions, and comprehensive documentation. [Total: 10 marks]

---
## Question 7 [15 marks]
**What are the significant benefits offered by the application system reuse approach over the custom software development approach?**

### Answer:
Based on the information found in Chapter 15 (Software reuse), specifically section 15.4 (Application system reuse), and supplemented by domain knowledge, here are the significant benefits offered by the application system reuse approach over the custom software development approach:

1. **Reduced Development Time**: One of the key benefits is the significant reduction in the time needed to develop a system. Since components are reused, less time is spent on development from scratch. [3 marks, Chapter 15]

2. **Cost-Efficiency**: Reusing existing application systems or components can lead to cost savings as compared to developing custom software. [3 marks, Chapter 15]

3. **Proven Reliability**: The components or systems being reused have usually been tested in real-world scenarios, offering a level of reliability that is hard to achieve with newly developed custom software. [3 marks, Chapter 15]

4. **Consistency and Standardization**: Application system reuse promotes consistency and standardization across multiple projects, making it easier to manage and maintain them. [3 marks, Chapter 15]

**Additional Point (Based on Domain Knowledge)**:
5. **Ease of Integration**: Reused systems often come with well-defined interfaces and are designed for integration, making it easier to incorporate them into existing architectures. [3 marks, Domain Knowledge]

In summary, application system reuse offers benefits like reduced development time, cost-efficiency, proven reliability, and consistency over custom software development. These advantages make it an appealing option for many organizations. [Total: 15 marks]

---
## Question 8 [10 marks]
**Give two significant application types that you would not advise using service-oriented design and explain why in your response?**

### Answer:
Based on the information found in Chapter 18 (Service-oriented software engineering) of "source_text_1," and supplemented by domain knowledge, here are two significant application types that are not advisable for using service-oriented design:

1. **Real-Time Systems**: Real-time systems require timely and deterministic responses. Service-oriented design often involves network communication, which can introduce latency and make the system's behavior unpredictable. This could be detrimental for applications where timing is critical, such as in automated manufacturing or medical devices. [4 marks, Domain Knowledge]

2. **Highly-Secure Systems**: Applications that require a high level of security, such as military or financial systems, might not be suitable for service-oriented design. The distributed nature of service-oriented architectures can introduce multiple points of vulnerability, making it challenging to secure the entire system comprehensively. [4 marks, Domain Knowledge]

**Additional Point (Based on Source Text)**:
3. **Payment Model Concerns**: The payment model for services in service-oriented design could make operation very expensive for certain types of applications. This is especially true for applications that require extensive service interactions, where costs could quickly escalate. [2 marks, Chapter 18]

In summary, real-time systems and highly secure applications are generally not suitable for service-oriented design due to issues like latency, unpredictability, and security vulnerabilities. Additionally, the cost associated with the service payment model can be a concern. [Total: 10 marks]

