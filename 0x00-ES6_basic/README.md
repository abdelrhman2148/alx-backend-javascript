
# 0x00. ES6 Basics

## Overview
This project focuses on ECMAScript 6 (ES6) features and practices in JavaScript programming. The goal is to learn and apply modern JavaScript constructs such as block-scoped variables, arrow functions, default parameters, and other key ES6 features.

## Learning Objectives
By the end of this project, you should be able to:
- Understand what ES6 is and identify its new features.
- Differentiate between constants (`const`) and variables (`let`).
- Utilize block-scoped variables.
- Implement arrow functions and function parameters with defaults.
- Use rest and spread parameters effectively.
- Apply string templating.
- Create objects using shorthand syntax and computed properties.
- Iterate through objects and arrays using `for-of` loops and iterators.

## Requirements
- Code will be executed on Ubuntu 18.04 LTS using NodeJS 12.11.x.
- You can use any of the following editors: `vi`, `vim`, `emacs`, `Visual Studio Code`.
- All files should end with a new line.
- Use the `.js` extension for all files.
- Your code will be tested using Jest and analyzed with ESLint.
- All functions must be exported.

## Setup Instructions

### Install NodeJS 12.11.x:
1. In your home directory, run the following:
   ```bash
   curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh
   sudo bash nodesource_setup.sh
   sudo apt install nodejs -y
   ```
2. Verify the installation:
   ```bash
   nodejs -v
   npm -v
   ```

### Install Jest, Babel, and ESLint:
- Run `npm install` in your project directory to install the necessary dependencies from `package.json`.

## Configuration Files
- Ensure the following configuration files are present in your project:
  - `package.json`
  - `babel.config.js`
  - `.eslintrc.js`

## Tasks

### 0. Const or let?
Refactor the code to use `const` for variables that shouldn't change, and `let` for variables that might change.

### 1. Block Scope
Refactor to ensure the variables inside the block aren't overwritten by using block-scoped variables.

### 2. Arrow Functions
Refactor the function to use ES6's arrow syntax.

### 3. Parameter Defaults
Condense function internals using default parameters.

### 4. Rest Parameter Syntax
Modify the function to return the number of arguments passed to it using rest parameters.

### 5. Spread Syntax
Concatenate arrays and characters of a string using the spread syntax.

### 6. Template Literals
Refactor the return statement to use ES6 template literals.

### 7. Object Property Shorthand
Modify the object creation to use property shorthand syntax.

### 8. Computed Property Names
Use computed property names for object properties based on dynamic values.

### 9. ES6 Method Properties
Use ES6 method property syntax for the object methods.

### 10. For...of Loops
Refactor the code to use the `for...of` loop for iterating over arrays.

### 11. Iterator
Write a function that returns an object using iterators.

### 12. Report Object
Create a report object with a method that returns the number of departments.

## Running Tests
To test the solutions:
bash
npm run dev <filename.js>
```

## Repository
- GitHub Repository: `alx-backend-javascript`
- Directory: `0x00-ES6_basic`

This `README.md` provides a comprehensive overview of the project, including setup instructions, task descriptions, and repository structure.
