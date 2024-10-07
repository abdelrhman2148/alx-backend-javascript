# 0x03. ES6 Data Manipulation

## Project Overview
This project explores advanced JavaScript concepts including data structures like `Set`, `Map`, `WeakMap`, and their usage in data manipulation tasks. It also focuses on array manipulation techniques using `map`, `filter`, and `reduce`. The tasks are designed to provide hands-on experience with ES6 features for processing and handling collections of data efficiently.

## Table of Contents
1. [Getting Started](#getting-started)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Project Structure](#project-structure)
5. [Task Breakdown](#task-breakdown)
6. [Example Usage](#example-usage)

---

## Getting Started

To get started with the project, you will need to have `Node.js` installed and a few dependencies like `Jest`, `Babel`, and `ESLint` to ensure that your code works correctly and adheres to the required guidelines.

## Prerequisites

Before starting, ensure you have the following installed:

- **Node.js** v12.x
- **NPM** (Node Package Manager)
  
Verify installation by running:

```bash
$ node -v
v12.11.1

$ npm -v
6.11.3
```

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/YourUsername/alx-backend-javascript.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd 0x03-ES6_data_manipulation
   ```

3. **Install dependencies**:
   Run the following command to install the required packages, including `Jest` for testing, `Babel` for ES6 transpiling, and `ESLint` for linting.
   ```bash
   npm install
   ```

## Project Structure

```bash
.
├── 0-get_list_students.js        # Task 0: Basic list of objects
├── 1-get_list_student_ids.js     # Task 1: More mapping
├── 2-get_students_by_loc.js      # Task 2: Filter
├── 3-get_ids_sum.js              # Task 3: Reduce
├── 4-update_grade_by_city.js     # Task 4: Combine
├── 5-typed_arrays.js             # Task 5: Typed Arrays
├── 6-set.js                      # Task 6: Set data structure
├── 7-has_array_values.js         # Task 7: More Set data structure
├── 8-clean_set.js                # Task 8: Clean Set
├── 9-groceries_list.js           # Task 9: Map data structure
├── 10-update_uniq_items.js       # Task 10: More map data structure
└── 100-weak.js                   # Task 11: WeakMap and queryAPI
```

## Task Breakdown

### Task 11: Weak Link Data Structure

This task focuses on using the `WeakMap` data structure in JavaScript to track the number of API calls for each endpoint. If an endpoint is queried more than 5 times, an error is thrown.

#### Function Breakdown:

- **`weakMap`**: A `WeakMap` instance to store the count of API queries for each endpoint.
- **`queryAPI(endpoint)`**: This function takes an `endpoint` object as input, tracks how many times it’s called, and throws an error with the message _"Endpoint load is high"_ if called more than 5 times.

```javascript
const weakMap = new WeakMap();

function queryAPI(endpoint) {
  const count = weakMap.get(endpoint) || 0;
  
  if (count >= 5) {
    throw new Error('Endpoint load is high');
  }
  
  weakMap.set(endpoint, count + 1);
}
```

### Task Requirements:

- Use a `WeakMap` to track the number of times each endpoint is queried.
- If an endpoint is queried 5 or more times, throw an error: _"Endpoint load is high"_.

### Files Involved:
- **File**: `100-weak.js`
- **Test File**: `100-main.js`

## Example Usage

Here’s how you can run the task and test its functionality:

1. **Running the main test**:
   ```bash
   npm run dev 100-main.js
   ```

2. **Sample Output**:
   ```bash
   1
   2
   Error: Endpoint load is high
   ```

In this example, the endpoint is queried more than 5 times, resulting in an error being thrown after the fifth call.

## Testing

You can run the project’s tests by using:

```bash
npm run test
```

To check linting and ensure your code meets the required style guidelines:

```bash
npm run lint
```

## Conclusion

This project provides a practical understanding of ES6 data manipulation techniques, advanced data structures, and array methods. Completing these tasks equips you with the skills to manage and manipulate data efficiently in JavaScript.
