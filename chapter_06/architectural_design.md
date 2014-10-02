# Architectural Design

**Architectural Design:** concerned with understanding how a system should be organized and designing the overall structure of that system.

#### 2 levels of abstraction

1. Architecture in the small

    * how an individual program is decomposed into components<br><br>

2. Architecture in the large

    * how complex enterprise systems that include other systems,         programs and program components are arranged.

#### Three Advantages of explicit architecture

1. **Stakeholder Communication** - may be used to focus discussion

2. **System Analysis** - can it meet the requirements

3. **Large-Scale Reuse** - architecture can be the same for many systems

#### Modeling
* Block Diagrams
    * high level, informal design

* uses:
    * facilitating discussion about the system design
    * documenting an architecture that has been designed

#### Architectural Design Decisions
* Is there a generic application architecture that can be used as a template?
* How will the system be distributed?
* How will components be decomposed into sub-componments?
* How will the design be evaluated?
* How should the architecture be documented?

#### Architecture Style <=> Non-Functional Requierments

1. **Performance** - design should localize critical operations within a small number of components

2. **Security** - a layered structure should be used

3. **Safety** - compartmentalize safety operations into a single component

4. **Availability** - designed with redundant componments that can be swapped out without the system failing

5. **Maintainability** - self-contained components with low-coupling

#### Architectural Views

* **Logical View** - show key abstractions as objects of object classes

* **Process View** - show how at runtime the system is composed of interacting processes

* **Development View** - shows the breakdown of the software into components for developers

* **Physical View** - shows the system hardware and how software components are distributed across the processors in the system.

#### Architectural Patterns

1. **MVC (Model-View-Controller)**

2. **Layered Architecture**
    * supports incremental development
    * highest layer represents UI
    * lowest layer represents core services
    <br><br>

3. **Repository Architecture**
    * efficient for sharing large amounts of data
    <br><br>

4. **Client-Server Architecture**
    * concerned with the static structure of the system in mind
    * Client and Server connected through network
    <br><br>

5. **Pipe and Filter**
    * model of run-time organization
    <br><br>

#### Application Architectures

* Encapsulates the principal characteristics of a class of systems

 * **Uses:**
    * starting point for architectural design process
    * a design checklist
    * way of organizing the work of the dev team
    * means of assessing components for reuse
    * as a vocabulary for talking about types of applications

* **Types:**
    * Transaction Processing Applications
        * process user requests for information on a database
    * Language Processing Systems
        * Compilers (Scanner, Parser, Lexicon, Syntax, Semantics)


