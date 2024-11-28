# 0x06. Unit Tests in JavaScript

## Table of Contents
1. [Introduction](#introduction)
2. [Learning Objectives](#learning-objectives)
3. [Requirements](#requirements)
4. [Project Setup](#project-setup)
5. [Tasks Overview](#tasks-overview)
6. [Usage Instructions](#usage-instructions)
7. [File Structure](#file-structure)
8. [Tips and Best Practices](#tips-and-best-practices)

---

## Introduction
This project focuses on creating **unit tests** and **integration tests** in JavaScript using tools like **Mocha**, **Chai**, and **Sinon**. Testing is a critical part of software development to ensure code quality and reliability. By the end of this project, you’ll have developed a strong foundation in writing and organizing unit tests and integration tests in a Node.js environment.

---

## Learning Objectives
By completing this project, you will learn:
- How to use **Mocha** to write test suites.
- How to use assertion libraries like **Node’s assert** and **Chai**.
- Organizing test cases using `describe` and `it` blocks.
- When and how to use **spies**, **stubs**, and **hooks**.
- Writing unit tests for **synchronous** and **asynchronous** functions.
- Performing integration testing on a small Express.js application.

---

## Requirements
- **Environment**: Ubuntu 18.04, Node.js 12.x.x.
- **Editors**: Any code editor (e.g., `vi`, `vim`, `emacs`, `Visual Studio Code`).
- **Node.js Dependencies**: 
  - Mocha
  - Chai
  - Sinon
  - Request
  - Express (for integration tests)
- All tests must pass without errors or warnings.

---

## Project Setup
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd 0x06-unittests_in_js
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Run tests:
   ```bash
   npm test <test_file>
   ```

---

## Tasks Overview

### 1. Basic Tests with Mocha and Node Assertion Library
- Implement a basic function `calculateNumber(a, b)` that rounds the inputs and returns their sum.
- Write test cases using **Node’s assert library**.

### 2. Enhanced Calculation Function
- Extend `calculateNumber` to include operations: `SUM`, `SUBTRACT`, `DIVIDE`.
- Write organized test cases using `describe`.

### 3. Using Chai for Better Readability
- Rewrite the test suite for the extended calculation function using **Chai’s expect API**.

### 4. Spies
- Use **Sinon’s spy** to monitor function calls.
- Test a function (`sendPaymentRequestToApi`) that depends on the `Utils.calculateNumber`.

### 5. Stubs
- Replace the real implementation of `Utils.calculateNumber` with a **stub** that returns a controlled value.
- Use a **spy** to verify console logs.

### 6. Hooks
- Use `beforeEach` and `afterEach` hooks for repetitive tasks in your test suite.
- Test multiple calls to `sendPaymentRequestToApi` with different inputs.

### 7. Async Testing
- Test an asynchronous function (`getPaymentTokenFromAPI`) using the `done` callback to ensure proper execution.

### 8. Skipping Tests
- Learn how to skip failing tests temporarily using the `skip` feature.

### 9. Basic Integration Testing
- Create a simple Express.js server with a root endpoint.
- Write integration tests to validate the server’s behavior using the **request** module.

### 10. Regex Validation in Routes
- Extend the Express.js app to include a dynamic route `/cart/:id`.
- Write tests for valid and invalid route parameters.

---

## Usage Instructions

1. Run a specific test:
   ```bash
   npm test <test_file>
   ```
   Example:
   ```bash
   npm test 1-calcul.test.js
   ```

2. Run all tests:
   ```bash
   npm test
   ```

3. Start the Express.js server (for integration tests):
   ```bash
   node <server_file>
   ```

4. Test API endpoints using `curl` or integration tests.

---

## File Structure

```plaintext
0x06-unittests_in_js/
├── 0-calcul.js
├── 0-calcul.test.js
├── 1-calcul.js
├── 1-calcul.test.js
├── 2-calcul_chai.js
├── 2-calcul_chai.test.js
├── 3-payment.js
├── 3-payment.test.js
├── 4-payment.js
├── 4-payment.test.js
├── 5-payment.js
├── 5-payment.test.js
├── 6-payment_token.js
├── 6-payment_token.test.js
├── 7-skip.test.js
├── 8-api/
│   ├── api.js
│   ├── api.test.js
│   └── package.json
├── 9-api/
│   ├── api.js
│   ├── api.test.js
│   └── package.json
└── README.md
```

---

## Tips and Best Practices
1. **Write Descriptive Tests**: Use clear and meaningful descriptions in your test cases.
2. **Test Edge Cases**: Always consider edge cases for robust testing.
3. **Isolate Unit Tests**: Avoid dependencies on external systems during unit testing.
4. **Restore Spies/Stubs**: Always clean up spies and stubs to prevent unexpected behaviors in subsequent tests.
5. **Async Testing**: Use `done` or return a promise to handle asynchronous operations correctly.
6. **Use Hooks**: Simplify repetitive setup/cleanup tasks with `beforeEach` and `afterEach`.

---

With this structure and guidance, you’re ready to implement and test robust JavaScript applications! 🚀
