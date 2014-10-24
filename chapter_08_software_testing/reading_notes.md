# Reading Notes: Chapter 08 - Software Testing

## 8.1 Development testing

#### Unit Testing
individual program units or object classes are tested. Testing the functionality of objects or methods.
* test all object methods
* set and check the value of all attributes associated with the         object
*  put the object into all possible states. This means that you          should simulate all events that cause a state change.

* Automated Testing
    1. setup: initialize the system (inputs and expected outputs)
    2. call (call the object or method to be tested)
    3. assertion (compare the call with the expected result)
* Choosing Unit Tests
    * Partition Testing:
        * using groups of inputs that have common characteristics and         should be processed in a similar fashion
    * Guideline-Based Testing:
        * guidelines reflect previous experience of the kinds of              errors that program- mers often make when developing                  components
* Choose test cases on the boundaries of partitions
* Choose inputs that force the system to generate all error             messages;
* Design inputs that cause input buffers to overflow;
* Repeat the same input or series of inputs numerous times;
* Force invalid outputs to be generated;
* Force computation results to be too large or too small.

#### Component Testing
where several individual units are integrated to create composite components. Component testing should focus on testing component interfaces.

1. **Parameter interfaces** These are interfaces in which data or sometimes function references are passed from one component to another. Methods in an object have a parameter interface.

2. **Shared memory interfaces** These are interfaces in which a block of memory is shared between components. Data is placed in the memory by one subsystem and retrieved from there by other sub-systems. This type of interface is often used in embedded systems, where sensors create data that is retrieved and processed by other system components.

3. **Procedural interfaces** These are interfaces in which one component encapsu- lates a set of procedures that can be called by other components. Objects and reusable components have this form of interface.

4. **Message passing interfaces** These are interfaces in which one component requests a service from another component by passing a message to it. A return message includes the results of executing the service. Some object-oriented sys- tems have this form of interface, as do client–server systems.


* **Interface Errors**
    * interface misuse
    * interface misunderstandin
    * timing errors

* **Interface Testing Guidelines**

1. Examine the code to be tested and explicitly list each call to an external component. Design a set of tests in which the values of the parameters to the external components are at the extreme ends of their ranges. These extreme values are most likely to reveal interface inconsistencies.

2. Where pointers are passed across an interface, always test the interface with null pointer parameters.

3. Where a component is called through a procedural interface, design tests that deliberately cause the component to fail. Differing failure assumptions are one of the most common specification misunderstandings.

4. Use stress testing in message passing systems. This means that you should design tests that generate many more messages than are likely to occur in prac- tice. This is an effective way of revealing timing problems.

5. Where several components interact through shared memory, design tests that vary the order in which these components are activated. These tests may reveal implicit assumptions made by the programmer about the order in which the shared data is produced and consumed.


#### System Testing

* where some or all of the components in a system are integrated and the system is tested as a whole. System testing should focus on testing com- ponent interactions.

* system testing should focus on testing the interactions between the components and objects that make up a system

* focus on testing the features of the operational system

    1. All system functions that are accessed through menus should be tested.

    2. Combinations of functions (e.g., text formatting) that are accessed through the same menu must be tested.

    3. Where user input is provided, all functions must be tested with both correct and incorrect input.


## 8.2 Test-Driven Development

* interleave testing and code development. You develop the code incrementally, along with a test for that increment. You don’t move on to the next increment until the code that you have developed passes its test.

    1. identify an increment of functionality

    2. write a test for this functionality

    3. run the test along with all other tests

    4. implement the functionality and re-run the tests

    5. once the test passes, implement the next chunk of functionality

* Benefits of TTD
    1. **Code Coverage** : All code has been executed
    2. **Regression Testing** : check that changes have not introduced new bugs
    3. **Simplified Debugging** : when a test fails, it should be obvious where the problem is
    4. **System Documentation** : the tests themselve serve as documentation



## 8.3 Release Testing

the process of testing a particular release of a system that is intended for use outside of the development team.

**Two Important Distinctions**

1. A separate team that has not been involved in the system development should be responsible for release testing.

2. System testing by the development team should focus on discovering bugs in the system (defect testing). The objective of release testing is to check that the system meets its requirements and is good enough for external use (validation testing).


* **Requirements Based Testing**
    * requirements should be testable

* **Scenario Testing**
    *  Scenario testing is an approach to release testing where you devise typical scenarios of use and use these to develop test cases for the system. A scenario is a story that describes one way in which the system might be used. Scenarios should be realistic and real system users should be able to relate to them.

* **Performance Testing**
    * slowly increasing the load on the system, starting with below minimum requirements and increasing the stress on the system up to and beyond average usage
    * if the system reaches a point where the load proves too much and the system fails, test that the system has a soft-fail where there is not data corruption and/or loss and the system fails gracefully.
    * This type of stress testing can bring defects to light that may have otherwise remained hidden.


## 8.4 User Testing
a stage in the testing process in which users or customers provide input and advice on system testing

* **Alpha Testing**
    * where users work along side the development team to test the system at the developers worksite

* **Beta Testing**
    * when a realease of the software is made available to users to test and raies concerns and defects to the dev teams

    * mostly used for software products that are used in many different environments

    * also a form of marketing— customers learn about their system and what it can do for them.

* **Acceptance Testing**
    * where customers test the system and decide whether it is complete and ready to be released to the customer environment


1. Define acceptance criteria
2. Plan acceptance testing
3. Derive acceptance tests
4. Run acceptance tests
5. Negotiate test results
6. Reject/accept system


