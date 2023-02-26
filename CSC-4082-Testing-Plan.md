# Test Plan

## Unit Tests
Provide a description of the object classes (or appropriate source level construct depending on the programming model chosen) and the corresponding methods to be tested. Each test should call various methods and use an array of expected, edge-case, and erroneous inputs (see section 8.1.2 of the Sommerville Software Engineering textbook for more information). Each test should be connected to one or more requirements.

Automated unit tests (preferred) should include the following:

1. Setup part (test case initialization, inputs, and expected outputs)
2. Call part (call object/method to be tested)
3. Assertion part (compare result of call w/ expected result)

There should be some form of output that shows the results of passed and failed tests (expected and actual outputs on failed tests).

## Component Tests
Next, provide a description of tests that ensure the correctness of interacting objects. The focus here is the component interface(s). The unit tests should all be passing before you start component testing. 

The types of interfaces to be aware of include:
1. Parameter interfaces (data/function references are passed between components)
2. Shared memory interfaces (if applicable)
3. Procedural interfaces (component has set of procedures callable by other parts of the code)
4. Message passing ionterfaces (one compoennts requests a service from another component)

You are looking for the following errors:
1. Interface misuse
2. Interface misunderstanding. 
3. Timing errors

For specifics, I refer you back to your software engineering textbook

## System Tests
Please describe how you will ensure that the major workflow(s) of your application are operating correctly. This will involve checking component capability, that interactions are operating according to your design, and that the data is flowing through all components as expected. The transformations that occur to inputs need to be verified at this point and overall outputs from the system should be verified as correct. 

The emergent behavior of your system should be sound once this phase of testing is complete. In other words, you need to tell me how your authenatication subsytem (if applicable) ties into your core application and how the core application ties into any backend components like a database or rendering system. 

It is recommended to use, **use case-based** testing at this point. It is also possible to draw on sequence diagrams to help you derive the needed test cases for this phase. 

Keep in mind that you only have so much time to dedicate to all levels of testing. It is not possible to be exhaustive with testing, just as complete as resources and time will allow. 

## User or Customer Tests

You should have several individuals not connected to the development of this project test your program at this point. The tests in this phase will include a script that exercises, at a minimum, the must-have requirements in your software. 

## Performance Tests
Once all other tests are complete, this section describes how the system will be stress tested. This includes placing high computational loads, high memory loads given a memory constrained environment, high levels of network traffic, and intermittent connectivity. 

## Tips (Remove if using this as a template on your Wiki)

1. Track failed tests beyond unit tests in the Issues section of a GitHub repository or some other bug tracking system like Bugzilla. This will help you in 
2. Try testing your software on non-development systems, including back-end components on client-server systems. You may find it helpful to create virtual machines or containers at this point to assist your testing efforts. 
3. Try using an operating system other than the one used for development (this includes back-end and front-end components if applicable)
4. Try using low-end hardware or a VM/container with highly restrained resources.
5. Try constraining network bandwidth and or pulling the network plug (virutal or physical)
6. Try pulling the power cable (or virtual switch). **Note that you may want to have backups in place before trying this step**. 

## References (feel free to add, modify, or remove this section as needed)
Sommerville, I. (2016). *Software Engineering* (K. Loanes, Ed.; 10th ed.). Pearson.
