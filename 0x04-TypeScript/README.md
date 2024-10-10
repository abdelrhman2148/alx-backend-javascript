# 0x04. TypeScript

## Project Overview

This project focuses on TypeScript, a statically typed superset of JavaScript. The main goal is to enhance your JavaScript skills by using TypeScript for creating interfaces, classes, and generic types, working with the DOM, and managing type declarations. You'll also explore advanced TypeScript features like namespaces and declaration merging.

## Learning Objectives

By the end of this project, you should be able to:

- Understand basic types in TypeScript.
- Create and use interfaces, classes, and functions.
- Work with the DOM using TypeScript.
- Use generic types.
- Implement namespaces and declaration merging.
- Import external libraries with ambient namespaces.
- Apply basic nominal typing with TypeScript.

## Project Structure

The project is divided into multiple tasks, each building on your knowledge of TypeScript:

1. **Task 0: Creating an Interface for a Student**
    - Create a `Student` interface.
    - Render a table in the DOM using student data.

2. **Task 1: Building a Teacher Interface**
    - Create a `Teacher` interface.
    - Extend the `Teacher` interface with additional attributes.

3. **Task 2: Extending the Teacher Class**
    - Write a `Directors` interface extending the `Teacher` interface.

4. **Task 3: Printing Teachers**
    - Create a `printTeacher` function that returns formatted names.

5. **Task 4: Writing a Class**
    - Define a `StudentClass` with methods and constructor using TypeScript interfaces.

6. **Task 5: Advanced Types Part 1**
    - Implement advanced types with `Director` and `Teacher` classes.

7. **Task 6: Creating Functions Specific to Employees**
    - Implement functions to handle employee-specific logic.

8. **Task 7: String Literal Types**
    - Use string literal types to restrict variable values.

9. **Task 8: Ambient Namespaces**
    - Create an interface and use an external library (`crud.js`) through ambient declarations.

10. **Task 9: Namespace & Declaration Merging**
    - Merge namespaces and declare multiple interfaces across files.

11. **Task 10: Update main.ts**
    - Export constants and log outputs for different subjects.

12. **Task 11: Brand Convention & Nominal Typing**
    - Use nominal typing to ensure type uniqueness in `MajorCredits` and `MinorCredits`.

## Setup & Configuration

- **Allowed editors**: `vi`, `vim`, `emacs`, `Visual Studio Code`
- **Transpiling environment**: Ubuntu 18.04
- **Testing framework**: Jest (v24.9.\*)
- **TypeScript version**: 3.6.4 or later
- **Webpack**: 4.41.2 or later

### Configuration Files

The following configuration files are provided:

- `package.json`: Defines project dependencies.
- `.eslintrc.js`: Ensures code adheres to TypeScript and ESLint standards.
- `tsconfig.json`: Configures TypeScript compilation options.
- `webpack.config.js`: Manages bundling of JavaScript and TypeScript files.

## Running the Project

1. Install dependencies:

   ```bash
   npm install
   ```

2. Build the project:

   ```bash
   npm run build
   ```

3. Run tests:

   ```bash
   npm test
   ```

## Requirements

- Your TypeScript code should not display any compilation errors or warnings.
- Use TypeScript for all tasks as much as possible.
- Follow the instructions for each task closely to meet the project requirements.

## Author

Abdelrhman Fikri - ALX Software Engineering Program
