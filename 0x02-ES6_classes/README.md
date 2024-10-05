# 0x02. ES6 Classes

## Project Overview
This repository contains a set of exercises focused on Object-Oriented Programming (OOP) in JavaScript, specifically leveraging the features of ES6 (ECMAScript 2015). The project demonstrates the usage of ES6 classes, static methods, getters and setters, inheritance, and other OOP principles, alongside metaprogramming techniques.

### Key Topics Covered
- ES6 Class syntax and structure
- Getters and Setters for encapsulation
- Static methods
- Inheritance and method overriding
- Metaprogramming with Symbols and class hoisting
- Abstract classes and method implementation

## Learning Objectives
By the end of this project, you should be able to:
1. Define and create ES6 classes.
2. Add methods to a class, including static methods.
3. Extend a class from another and override methods.
4. Use metaprogramming techniques with symbols and hoisting.
5. Understand and implement class inheritance and abstract classes.

## Requirements
- All files are executed on Ubuntu 18.04 LTS using NodeJS 12.11.x.
- Files should end with a new line.
- The repository must contain a `README.md` file.
- Code must use the `.js` extension.
- Code will be tested using `Jest` and `npm run test`.
- Code must pass `ESLint` checks.
- You can verify the project with `npm run full-test`.

## Setup Instructions
1. **Install NodeJS** (v12.11.x):
   ```bash
   curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh
   sudo bash nodesource_setup.sh
   sudo apt install nodejs -y
   nodejs -v  # Should output v12.11.x
   npm -v     # Should output 6.11.x
   ```

2. **Install Project Dependencies**:
   Run the following in your project directory:
   ```bash
   npm install
   ```

## Configuration Files
The project includes the following configuration files:
- **package.json**: for managing project dependencies.
- **babel.config.js**: for Babel transpilation.
- **.eslintrc.js**: for linting with ESLint.

Make sure to run `npm install` to install the dependencies specified in `package.json`.

## Project Tasks

### Mandatory Tasks
1. **ClassRoom Class**: 
   - Implements a class that defines the maximum size of a classroom.
   
2. **Initialize ClassRooms**: 
   - A function that returns an array of 3 `ClassRoom` objects with different sizes.

3. **HolbertonCourse Class**: 
   - A class with name, length, and students attributes, and their getters and setters.

4. **Currency Class**: 
   - A class that defines currency with its name and code.

5. **Pricing Class**: 
   - Combines a price amount with a currency and includes a static conversion method.

6. **Building Class**: 
   - An abstract class that must be extended by other building classes with a method for evacuation messages.

7. **SkyHighBuilding Class**: 
   - Extends the `Building` class, adding floors and overriding the evacuation message method.

8. **Airport Class**: 
   - A class that returns the airport code as the default string representation.

9. **HolbertonClass Casts**: 
   - A class where casting to a number returns the size and casting to a string returns the location.

10. **Car Class**: 
    - Defines a car with a method to clone the object.

### Advanced Tasks
11. **EVCar Class**:
    - Extends `Car` class with an additional `range` attribute. When cloned, it returns an instance of `Car`.

## Running Tests
To run tests:
```bash
npm run test
```

To run lint checks and tests:
```bash
npm run full-test
```

## Repository Structure
- **0-classroom.js**: ClassRoom implementation.
- **1-make_classrooms.js**: Function to initialize classrooms.
- **2-hbtn_course.js**: HolbertonCourse class.
- **3-currency.js**: Currency class.
- **4-pricing.js**: Pricing class.
- **5-building.js**: Building class (abstract).
- **6-sky_high.js**: SkyHighBuilding class.
- **7-airport.js**: Airport class.
- **8-hbtn_class.js**: HolbertonClass with casting.
- **9-hoisting.js**: Fixed class hoisting code.
- **10-car.js**: Car class.
- **100-evcar.js**: EVCar class extending Car.

## Author
Abdelrhman Fikri Elrhmany
