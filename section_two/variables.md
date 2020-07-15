7. Variables - var, let & const Notes

var

    NOTE: var and let allow variables to be reassigned, const doesn't allow that.

        EXAMPLE: 
            var name = 'John Doe' 
            console.log(name) --> console will output John Doe
            name = 'Steve Smith'
            console.log(name) --> console will output Steve Smith

    NOTE: Initalizing variables means when you assign a variable something but don't give it a value just yet. It typically shows up undefined until you assign it something

        EXAMPLE:
            var greeting
            console.log(greeting) --> console shows undefined

    NOTE: Now if you define the var greeting a value, it will show the value in the console. 

        EXAMPLE: 
            greeting = 'hello'
            console.log(greeting) --> console outputs 'hello'

    NOTE: Typically programmers will initalize variables when using conditionals,such as an 'if statement' and wanting to say something is true equals an action / or else is false equals an action for a function (boolean)

letters, numbers, _, $

    NOTE: variables cannot start with a number
    NOTE: $ is typically used with jQuery
    NOTE: _ is typically used for private variables
    NOTE: letters are typically used to construct variables

Multi word vars
    NOTE: multi word vars are typically written in camelCase

        EXAMPLE: 
            var firstName = 'John' --> camelCase (MOST COMMON)
            var first_name = 'Sara' --> Underscore (Better for certain languages)
            var FirstName = 'Tom' --> Pascal case (used in special cases, such as object oriented cases)
            var firstname; --> AVOID USING! 


let (works similarly to var but is newer in the ES6 update)

        EXAMPLE:
            let name; --> initalizing variables (see line 49, name is assigned to 'John Doe' therefore it will not come out undefined)
            name = 'John Doe' 
            console.log(name) --> console will output John Doe
            name = 'Steve Smith'
            console.log(name) --> console will output Steve Smith

const 

     NOTE: const stands for constant therefore, variables cannot change or be reassigned like var and let

         EXAMPLE: 
             const name = 'John'
             console.log(name) --> console will output John
         CANNOT REASSIGN EXAMPLE: 
             name = 'Sara' --> console will scream at you and give you a Uncaught TypeError: Assignment to constant variable 

 NOTE: With const, you must assign a value, you cannot initalize with const

         EXAMPLE: 
             const greeting; --> console will scream at you and give you a Uncaught SyntaxError: Missing initializer in const declaration.

 NOTE: you can manipulate const values if the are in an object but you cannot change the const's variable (person in this example)

         EXAMPLE:    
             const person ={
              name: 'John'
              age: 30
             }
             console.log(person) --> console logs an object containing the values {name: 'John', age: 30}
         EXAMPLE OF MANIPULATION
         const person ={
              name: 'John'
              age: 30
             }
             person.name = 'Sara'
             person.age = 32
             console.log(person) --> console outputs object {name: 'Sara', age: 32}

 NOTE: you can assign const a variable and create an array of values

         EXAMPLE:
             const numbers = [1,2,3,4,5]
             console.log(numbers) --> console outputs an array of numbers 

 NOTE: You can add a value to an array that has been assigned to a const variable by 'pushing' it

         EXAMPLE: 
         const numbers = [1,2,3,4,5]
         numbers.push(6)
         console.log(numbers) --> console outputs [1,2,3,4,5,6]