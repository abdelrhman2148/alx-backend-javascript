# 0x05. NodeJS Basics

## Project Overview

This project explores foundational concepts of Node.js and Express.js, including creating HTTP servers, reading files synchronously and asynchronously, and utilizing ES6 features. It introduces tools like Babel, ESLint, Mocha, and Nodemon for efficient development and code quality assurance.

### Objectives

By completing this project, you will learn to:
- Execute JavaScript using Node.js.
- Work with Node.js modules.
- Use the Process API for environment and command-line argument handling.
- Build HTTP servers with Node.js and Express.js.
- Utilize ES6 features in Node.js with Babel.
- Develop and debug efficiently with Nodemon.
- Write and run tests using Mocha.

---

## Table of Contents

1. [Requirements](#requirements)  
2. [Setup Instructions](#setup-instructions)  
3. [Project Files and Tasks](#project-files-and-tasks)  
4. [Testing and Linting](#testing-and-linting)  
5. [Helpful Commands](#helpful-commands)  

---

## Requirements

- **Environment**: Ubuntu 18.04 LTS with Node.js version `12.x.x`.  
- **Code Style**: Must pass ESLint checks.  
- **Testing Framework**: Mocha and Chai.  
- **File Extensions**: All code files should use the `.js` extension.  
- **GitHub Repository**: `alx-backend-javascript`.  
- **Project Directory**: `0x05-Node_JS_basic`.

---

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/alx-backend-javascript.git
   cd alx-backend-javascript/0x05-Node_JS_basic
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run tests and lint checks:
   ```bash
   npm run full-test
   ```

---

## Project Files and Tasks

### 1. **Basic JavaScript Execution (`0-console.js`)**
- Function: `displayMessage(string)`
- Prints a string to the console.
- Example:
  ```bash
  node 0-main.js
  # Output: Hello NodeJS!
  ```

---

### 2. **Process Input Handling (`1-stdin.js`)**
- Prompts user input and prints a response.
- Handles program termination gracefully.
- Example:
  ```bash
  node 1-stdin.js
  Welcome to Holberton School, what is your name?
  Bob
  Your name is: Bob
  ```

---

### 3. **Reading Files Synchronously (`2-read_file.js`)**
- Reads and parses `database.csv`.
- Logs total students and categorized counts by field.
- Example:
  ```bash
  node 2-main_1.js
  Number of students: 10
  Number of students in CS: 6. List: Johann, Arielle, Jonathan, Emmanuel, Guillaume, Katie
  ```

---

### 4. **Reading Files Asynchronously (`3-read_file_async.js`)**
- Similar to Task 3 but uses promises for asynchronous operations.
- Logs student data.
- Example:
  ```bash
  node 3-main_1.js
  After!
  Number of students: 10
  ```

---

### 5. **Basic HTTP Server (`4-http.js`)**
- Creates a server using the `http` module.
- Serves plain text `Hello Holberton School!` on any endpoint.
- Example:
  ```bash
  curl localhost:1245
  # Output: Hello Holberton School!
  ```

---

### 6. **Complex HTTP Server (`5-http.js`)**
- Extends the previous server to handle two routes:
  - `/`: Returns `Hello Holberton School!`.
  - `/students`: Displays student data from `database.csv`.

---

### 7. **Express.js HTTP Server (`6-http_express.js`)**
- Recreates the basic HTTP server using Express.js.
- Serves `Hello Holberton School!` on `/`.

---

### 8. **Advanced Express.js HTTP Server (`7-http_express.js`)**
- Handles routes `/` and `/students` using Express.js.
- Outputs student data in plain text.

---

## Testing and Linting

1. **Run Tests**:
   ```bash
   npm test
   ```

2. **Run Lint Checks**:
   ```bash
   npm run lint
   ```

3. **Run Full Validation**:
   ```bash
   npm run full-test
   ```

---

## Helpful Commands

- **Start Development Server**:
  ```bash
  npm run dev
  ```
- **Run Babel Scripts**:
  ```bash
  babel-node <file>
  ```
- **Test with Mocha**:
  ```bash
  mocha
  ```

---

## Additional Resources

- [Node.js Documentation](https://nodejs.org/docs/latest-v12.x/api/)
- [Express.js Getting Started](https://expressjs.com/en/starter/installing.html)
- [Mocha Documentation](https://mochajs.org/)
- [Nodemon Documentation](https://nodemon.io/)
