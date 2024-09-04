This is 0x03-Unittests_and_integration_tests,

 Unit testing is the process of testing that a particular function returns expected results for different set of inputs. A unit test is supposed to test standard inputs and corner cases. A unit test should only test the logic defined inside the tested function. Most calls to additional functions should be mocked, especially if they make network or database calls.

The goal of a unit test is to answer the question: if everything defined outside this function works as expected, does this function work as expected?

Integration tests aim to test a code path end-to-end. In general, only low level functions that make external calls such as HTTP requests, file I/O, database I/O, etc. are mocked.

Integration tests will test interactions between every part of your code.

Unit tests and integration tests are both crucial in software development, but they serve different purposes and focus on different aspects of the codebase.

Unit Tests

Purpose: Unit tests are designed to test individual components or units of code in isolation. A unit is often the smallest testable part of an application, such as a function or method.
Scope: They focus on a single unit of code, ensuring that it behaves as expected under various conditions. The tests are usually narrow and specific.
Dependencies: Unit tests generally avoid external dependencies (like databases, file systems, or network calls) by using techniques like mocking or stubbing to isolate the unit.
Speed: Because they are testing isolated pieces of code, unit tests are typically fast to execute.
Granularity: They are fine-grained, targeting specific pieces of logic or functionality.

Integration Tests

Purpose: Integration tests verify that different modules or components of the application work together as expected. They focus on the interactions between these units.
Scope: They cover larger parts of the application than unit tests, often involving multiple units of code working together.
Dependencies: Integration tests usually involve real external dependencies (such as databases, web services, or APIs) to ensure that the integrated components work correctly in a realistic environment.
