# 0x01. ES6 Promises

## Overview
This project focuses on learning and using ES6 Promises in JavaScript. Promises allow us to handle asynchronous operations in a more readable and manageable way. You'll be tasked with working on various promise methods such as `then()`, `catch()`, `resolve()`, and `reject()`, as well as understanding and implementing `async/await`.

## Learning Objectives
By the end of this project, you should be able to:

- Explain the concept of Promises: what they are, why they are used, and how they work.
- Use `.then()`, `.catch()`, and `.resolve()` methods of the `Promise` object.
- Handle errors in asynchronous code using `try/catch` blocks.
- Understand and use `async` and `await` for handling asynchronous operations.
- Manage multiple promises with functions like `Promise.all()`.
  
## Resources
- [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)
- [JavaScript Promise: An introduction](https://developers.google.com/web/fundamentals/primers/promises)
- [Async functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function)
- [Throw / Try](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/try...catch)

## Requirements
- All your files will be executed on Ubuntu 18.04 LTS using NodeJS 12.11.x.
- Allowed editors: `vi`, `vim`, `emacs`, `Visual Studio Code`.
- Your code should use the `.js` extension.
- Your code will be tested using Jest and run with `npm run test`.
- Your code will be verified using `ESLint`.

## Setup
1. Install NodeJS 12.11.x:
    ```bash
    curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh
    sudo bash nodesource_setup.sh
    sudo apt install nodejs -y
    ```

2. Check Node and npm versions:
    ```bash
    node -v
    npm -v
    ```

3. Install Jest, Babel, and ESLint:
    ```bash
    npm install
    ```

## Project Tasks

### 0. Keep every promise you make and only make promises you can keep
- Implement a function `getResponseFromAPI()` that returns a promise.

### 1. Don't make a promise...if you know you can't keep it
- Implement `getFullResponseFromAPI(success)` to return a promise based on a boolean parameter `success`. If `true`, resolve with an object `{ status: 200, body: 'Success' }`. If `false`, reject with an error message.

### 2. Catch me if you can!
- Create a function `handleResponseFromAPI(promise)` that adds three handlers to the given promise. Return `{ status: 200, body: 'success' }` on resolve, an empty error object on rejection, and log "Got a response from the API" for every resolution.

### 3. Handle multiple successful promises
- Use `uploadPhoto` and `createUser` from `utils.js` to implement `handleProfileSignup()`. Resolve both promises and log `body firstName lastName`. Log "Signup system offline" on error.

### 4. Simple promise
- Write a function `signUpUser(firstName, lastName)` that returns a resolved promise with an object `{ firstName: value, lastName: value }`.

### 5. Reject the promises
- Implement a function `uploadPhoto(fileName)` that returns a rejected promise with the error `$fileName cannot be processed`.

### 6. Handle multiple promises
- Write `handleProfileSignup(firstName, lastName, fileName)` that calls `signUpUser()` and `uploadPhoto()`, then returns an array of promise results.

### 7. Load balancer
- Implement `loadBalancer(chinaDownload, USDownload)` to return the result of the fastest promise.

### 8. Throw error / try catch
- Write a function `divideFunction(numerator, denominator)` that throws an error if the denominator is zero, or returns the division otherwise.

### 9. Throw an error
- Implement `guardrail(mathFunction)` which handles function execution, appends the result or error to an array, and always appends "Guardrail was processed".

### 10. Await / Async
- Write an `async` function `asyncUploadUser()` that calls `uploadPhoto()` and `createUser()` and returns an object with `photo` and `user` keys.

## Repository Structure
- **GitHub repository:** `alx-backend-javascript`
- **Directory:** `0x01-ES6_promise`
