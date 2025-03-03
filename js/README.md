# Some Useful JavaScript Notes

## CommonJS vs ES (ECMAScript) Modules
Both CommonJS and ES Modules (ESM) are systems for organising and reusing code in JavaScript

### CommonJS
- Default module system in Node.js
- Not supported natively in browsers
    - Use a bundler (e.g. webpack or browserify)
- Uses require and module.exports to import and export modules respectively

### ES Modules
- Default module system in browsers
- Note supported natively in Node.js
    - Use extension .mjs or set "type": "module" in package.json 
- Uses import and export to import and export modules respectively 

## Data Types
JavaScript is a dynamically and weakly typed programming language 

### Dynamically Typed 
- Variables can be declared using the following declarations keywords
    - **let** - block scoped and not accessible before its declaration (not hoisted)
    - **var** - function scoped and accessible before its declaration (hoisted)
    - **const** - block scoped and can requires value assignment upon declaration and cannot be re-assigned
- Can be assigned and re-assigned a value of any data type

### Weakly Typed 
- Doesn't enforce strict type-checking rules
- Uses automatic type conversion called coercion to implicitly convert the variable data type to the type of the value being assigned or re-assigned to the variable

### Type Checking 
- Check if a variable exists / has been declared
    - typeof var === "undefined"
- Check if a variable contains a string value
    - typeof var === "string"
- Check if a variable contains a number value
    - typeof var === "number"

### Error Handling 
The process of **anticipating**, **detecting**, and **managing** errors that occur during program execution. Its primary goal is to ensure that your application can gracefully deal with unexpected situations without crashing. This can be achieved using try 
- Try-catch 
    - Typical for handling unexpected and unpredictable errors
- Conditional checks
    - Typical for handling expected and predictable errors
