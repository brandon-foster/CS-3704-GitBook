# Final Review


1. **Design:** activity following requirements and pior to coding, planning the inner workings of
the system and how they will be implemented
    * Answers "HOW" it will be built
    * instance of an Architecture
    * **Modular** - represents sub-systems of the Architecture
    * A **design pattern** is a way of reusing abstract
knowledge about a problem and its solution.
        * ex: the observer pattern: Display01 --> Object <-- Display02
    * Examples of **Design Diagrams**:
        * **Activity Diagram:** - depicts the dynamic behavior of a system or part of a system through the flow of control between actions that the system performs
        * **Business Process Model** -
        * **Class Diagram** - shows the layout of different classes, how they interact and any inheritance/polymorphic properties
        * **Use Case Diagram** - help you determine the functionality and features of the software from the user’s perspective
        * **Sequence Diagram** - steps/sequence of a function of the software, method calls as a particular function is carried out
        * **State Diagram** - outlines the behavior of a system at different times.

2. **Architecture:** the "structure of structures" of a system, externally visible components, a high level abstraction of a system
    * (Requirements) -> (Architecture) -> (Design)
    * **Characteristics:**
        * Performance
        * Security
        * Safety
        * Availiability
        * Maintainability
    * **4 + 1 View Model**:
        1. Logical View
        2. Process View
        3. Development View
        4. Physical View
        5. (+1) related use case scenarios
    * Architectural Styles:
        * Client/Server
        * Layered Architecture
        * Component-Based
    * Architectural Style vs. Pattern
        * Scope | Abstraction | Relationship
    * Examples:
        * Data Flow
        * Data Centered
        * Call and Return
        * Layered Architecture
        * Client-Server

3. **Testing:** testing the software
    * Reveals the presence of errors: not their absence
    * Validation Testing vs. Defect Testing
    * Verification vs. Validation (fit for purpose)
        * **Verification**: Are we building the product right?
        * **Validation**:  Are we building the right product?
    * **Inspection and Testing**
        * Inspection - static verification
        * Testing - dynamic verification
    * **Testing Stages**:
        * **Development Testing**
            * unit testing (Automated)
                * individual functions and classes
            * component testing
                * test combined component interfaces
            * Regression Testing
                * test that changes have not broken past functionality
            * system testing
                * testing of integrated componentsinto the system
        * **Release Testing**
            * testing software meant for use outside the dev team
        * **User Testing**
            * Alpha : testers work w/ dev team
            * Beta : release made available to users to experiment
            * Acceptence : customer tests and accepts/rejects the system

4. **Three Types of Component Composition:** Component Based SE
    1. **Sequential Composition**: new component from 2 existing components. Output from A -> glue code => B for formatting the output of A to necessary input for B
    2. **Heirarchical Composition**: One component calls another directly
    3. **Additive Composition**: 2 components put together to create a new component
5. **UML Diagrams** Standard language for writing the blueprints of a piece of software
    1. **Class Diagrams:** To model classes, including their attributes, operations, and their relationships and associations with other classes
    2. **Deployment Diagrams:** focuses on the structure of a software system and is useful for showing the physical distribution of a software system among hardware platforms and execution environments
    3. **Use-Case Diagrams:** determine the functionality and features of the software from the user’s perspective.
    4. **Sequence Diagrams:** a sequence diagram is used to show the dynamic com- munications between objects during execution of a task. It shows the temporal order in which messages are sent between the objects to accomplish that task.
    5. **Activity Diagrams:** depicts the dynamic behavior of a system or part of a system through the flow of control between actions that the system performs. It is similar to a flowchart except that an activity diagram can show concurrent flowlows.
    6. **State Diagrams:** The behavior of an object at a particular point in time often depends on the state of the object, that is, the values of its variables at that time.

6. **Project Management:** assures that software is delivered on-time, within budget and that it satifies the requirements of the customer
    * project planning
        * delegating tasks
        * project plan: how the work will be done
            * organize tasks concurrently
            * minimizing task dependencies
            * productivity !~ number of staff
    * reporting
    * risk management
        * identify risks and draw up plans to minimize their effects
        * common risks:
            * technology
            * people
            * organizational
            * requirements
            * estimation
    * Risk Management Process:
        * risk identification
        * risk analysis
            * probability?
        * risk planning
            * avoidance | minimization | contingency
        * risk monitoring
    * people management
    * proposal writing

7. **Process Improvement:** understanding
existing processes and changing these processes
to increase product quality and/or reduce costs
and development time.
    * Process Quality <-> Product Quality
    * Size, Maturity, Staff Skills
    * **Factors (Product Quality):**
        * Development Technology
        * Process Quality
        * People Quality
        * Cost, Time and Schedule
    *CMMI (Capability Maturity Model) process assessment and improvement framework
    * CMMI: an integrated process improvement model that supports both
staged and continuous process improvement.
    * Instantiations
        * Staged : the model is expressed in terms of
capability levels
        * Continuous : a capability rating is computed
    * Proccess Areas
        * 6-Point Scale
            * Not Performed
            * Performed
            * Managed
            * Defined
            * Quantitatively Managed
            * Optimizing
    * Goals
    * Practices
