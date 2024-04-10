# Theory of testing

## Test Driven Development(TDD) 

Test Driven Development (TDD) is a software development practice that focuses on creating unit test cases before developing the actual code.

The core idea behind TDD is to ensure that every piece of code is thoroughly tested, leading to higher code quality and reliability. 

TDD follows a simple and iterative cycle, often referred to as the “red-green-refactor” cycle.

TDD are typically written by developers, focusing on technical aspects. Collaboration primarily happens within the development team.

TDD focuses on unit testing, aiming to test individual units of code in isolation. It ensures high test coverage at the unit level.


### Concept and Benefits of TDD

 - TDD focuses on writing automated tests that specify the desired behavior of the code before implementing the code itself.

 - By writing tests first, developers gain a clear understanding of what needs to be implemented and how it should behave.

 - TDD reduces the likelihood of introducing bugs and allows for faster detection and resolution of issues.

 - It provides a safety net for making changes to the code by ensuring that existing functionality remains intact.

 - TDD encourages modular and loosely coupled code, leading to improved maintainability and easier refactoring.


### The TDD Cycle: Red, Green and Refactor

  - Red: In the initial “Red” phase, the developer writes a failing test case that highlights the desired behavior not yet implemented.

  - Green: In the “Green” phase, the developer writes the minimum amount of code necessary to pass the test.

   - Refactor: In the “Refactor” phase, the developer improves the code without changing its behavior. 
               This step enhances the design, removes duplication and improves maintainability.



## Behaviour Driven Development(BDD) 

BDD focuses on testing the behavior of the system as a whole from the **perspective of end-users** or stakeholders. 
It aims to ensure that the system behaves correctly in various scenarios.

BDD encourages collaboration between developers, testers and business stakeholders. 

Test scenarios are written collaboratively using a shared language, facilitating better communication and understanding among team members.

BDD covers different levels of testing, including unit, integration and acceptance testing. 
It aims to verify the behavior and interaction of various components in the system.


## Types of testing

So called pyramide of testing. There are several of them. Lets describe the common and simple one:


- **Unit tests**, low level
  Unit tests are very low level and close to the source of an application. They consist in testing individual methods and functions of the classes, 
  components, or modules used by your software. 
  Unit tests are generally quite cheap to automate and can run very quickly by a continuous integration server.

- **Integration tests**, middle level
  Integration tests verify that different modules or services used by your application work well together. 
  For example, it can be testing the interaction with the database or making sure that microservices work together as expected. 
  These types of tests are more expensive to run as they require multiple parts of the application to be up and running.

- **End-to-end tests(E2E)**, upper level
  End-to-end testing replicates a user behavior with the software in a complete application environment.
  It verifies that various user flows work as expected and can be as simple as loading a web page or logging in or much more 
  complex scenarios verifying email notifications, online payments, etc...


## What is a stub (test state)

A stub interface simulates an actual object by using a few methods. 

It's an **static object** with pre-existing data that delivers a **constant value regardless of input.**


## What is a mock (test behaviour) 

Mock is an interface that **we program to compare the outputs from the tests to the expected outcomes**. 

You can frequently use third-party libraries such as Mockito and JMock to accomplish this. 

It also comes in handy when you have an extensive test suite, and each test demands a different set of data.

The objects that hold method calls are mocks. The dynamic wrappers for dependencies utilized in the tests were referred to. 


## Test coverage

Test coverage defines what percentage of application code is tested and whether the test cases cover all the code. 
Should be ~90%.
