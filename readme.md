# Running Maven Tests

## Overview

Maven is a powerful build automation tool that is widely used for Java projects. One of its key features is the ability to execute tests as part of the build process. This document outlines the steps to run Maven tests using the command line interface.

## Prerequisites

- Java Development Kit (JDK) installed on your system.
- Maven installed on your system.
- A Maven project set up with unit tests.

## Procedure

1. **Open a Terminal or Command Prompt:**
   Open a terminal or command prompt window on your system.

2. **Navigate to Project Directory:**
   Use the `cd` command to navigate to the root directory of your Maven project. This directory should contain the `pom.xml` file.

   ```bash
   cd /path/to/your/project
   ```

3. **Run Maven Test Command:**
   Once you're in the project directory, execute the following command to run all unit tests in your project:

   ```bash
   mvn test
   ```

   Maven will compile your project's source code, execute the tests, and display the test results in the terminal.

4. **(Optional) Run Specific Tests:**
   If you want to run specific test classes or methods, you can use Maven's Surefire plugin to filter tests. Use the following command format:

   - To run specific test class:
     ```bash
     mvn -Dtest=TestClassName test
     ```

     Replace `TestClassName` with the name of the class containing the tests you want to run.

   - To run specific test method within a class:
     ```bash
     mvn -Dtest=TestClassName#testMethodName test
     ```

     Replace `testMethodName` with the name of the test method you want to run.

5. **Review Test Results:**
   After running the tests, review the output in the terminal. Maven will display information about the tests executed, including any failures or errors encountered.
