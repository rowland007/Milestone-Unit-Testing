# Milestone Unit Testing

### SNHU CS-405 4-2 Milestone: Unit Testing

[Milestone Unit Testing](https://github.com/rowland007/Milestone-Unit-Testing) by [Randall Rowland](https://randyrowland.me) is licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/?ref=chooser-v1) <img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/nc.svg?ref=chooser-v1">

# Overview

You are a senior software developer on a team of software developers who are responsible for a large banking web application. Your manager has recently learned about the best practice of creating unit tests for software and wants to see a full example of how it works. Another developer on the team started creating a unit test for the `std::vector` class, and he managed to get the `TextFixture` and a few tests completed before his vacation started. Your manager is impatient and has asked you to complete the task. He wants to see a number of tests, including positive and negative tests.

## Key Concepts

- Positive tests prove that functionality works when tested. For example, `Test(1+1) = 2`.
- Negative tests prove that an error or exception happens when provided bad data. For example, `Test(5/0) => Divide By Zero`.

The following are some essential notes:
- The source code has been commented using `TODO` to explain the detailed rules you must follow.
- You are provided the situation to create 13 unit tests, of which 11 are defined for you and 2 you will need to define.
- You only need a minimum of 2 negative tests, but can do more.
- Test names should reflect the purpose of a test. For example, to test that a number is positive, the test name would be something like `EnsureNumberIsPositive`.
- Do not confuse the C++ `assert` / `static_assert` with the Google Test `ASSERT` and `EXCEPT`.
    - When should you use the `EXPECT_xxx` or `ASSERT_xxx` macros?
        - Use `ASSERT` when failure should terminate processing, such as the reason for the test case.
        - Use `EXPECT` when failure should notify, but processing should continue.
- There are multiple ways to validate the test results, but each test must explicitly prove the defined condition of the test.
- Do not forget that you can leverage capabilities provided by the standard C++ library to help you achieve success.

You will learn to do the following:
- Name unit tests correctly
- Compile and run a Google unit test fixture
- Extend Google unit test fixture with a number of positive and negative tests
- Prove the test results

# Prompt

Test the existing source code in the test.cpp file using the Google unit testing framework. Include a brief written summary of the process you used, the issues you found, and how you managed the issues.

Specifically, address the following in a static testing summary:
- **Unit Test Names**: Define all unit test names to appropriately reflect the test condition.
- **Unit Testing**: Successfully implement the 13 unit tests, as part of the Google Test fixture; run Google Test `ASSERT` and `EXPECT` functionality to prove the tests. Each test you runmust explicitly prove the defined condition of the test.
- **Negative Unit Tests**: Complete at least 2 of the unit tests as negative tests that demonstrate capturing the appropriate unit test result based on an expected negative result of the test code.
- **C/C++ Program Functionality and Best Practices**: Demonstrate industry standard best practices, including in-line comments and appropriate naming conventions to enhance readability of code. Develop functional C/C++ code that illustrates a software design pattern approach.
- **Process Summary**: Provide a summary of the debugging that is thorough and systematic, including specific types of bugs, and that accurately describes the corrections.

To complete this assignment, download the test.cpp file and use the [Google Test Guide](https://learn.snhu.edu/content/enforced/796927-CS-405-X6390-OL-TRAD-UG.21EW6/course_documents/CS%20405%20Google%20Test%20Guide.pdf?_&d2lSessionVal=BCbuupcKI4cIhq25d2e7ncHcW&ou=796927) as guidance as you move through the activity. You will use your development environment to complete this activity. Google Test has a number of resources online, including the following:
- [Googletest Primer](https://google.github.io/googletest/primer.html)
- [How to Use Google Test for C++ in Visual Studio](https://docs.microsoft.com/en-us/visualstudio/test/how-to-use-google-test-for-cpp?view=vs-2019)