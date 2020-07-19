# function declarations & expressions

 NOTE: functions are blocks of code that can be defined & then called at a later time or in some cases defined in a call. 

## function declarations
    NOTE: anything inside the function is the function's scope. 

        EXAMPLE: 
            function greet(){
                console.log('Hello')
            }
            
            greet(); --> console outputs Hello

        EXAMPLE:
            function greet(){
                return 'Hello';
            }
            
            greet(); --> console outputs nothing because the function is just merely returning the message. Look at the example below to understand how to fix it. 

        EXAMPLE: 
            function greet(){
                return 'Hello';
            }

            console.log(greet()); --> console outputs Hello. The console will need to wrap around the function. 

        EXAMPLE: 
            function greet(firstName, lastName){
                return 'Hello ' + firstName + ' ' + lastName;
            }

            console.log(greet('Claire', 'Labry')); --> console outputs Hello Claire Labry

    NOTE: if you take out arguments out of the greet() function, the console output would be Hello undefined undefined. That is because firstName and lastName have yet to be defined. Look at the below examples for ways to define those variables. 

        EXAMPLE (es6): 
        function greet(firstName = 'John', lastName = 'Doe'){
                return 'Hello ' + firstName + ' ' + lastName;
            }

            console.log(greet()); --> console outputs Hello John Doe

## function expressions

        EXAMPLE: 
            const square = function(x){
                return x*x
            };

            console.log(square(8)) --> console's output is 64

        EXAMPLE: 
            const square = function(x = 3){
                return x*x
            };

            console.log(square()) --> console's output is 9

## immediately invokable function expressions - IIFEs

    NOTE: IIFEs are useful when it comes to certain design patterns such as the module pattern. 

 (https://medium.com/@vvkchandra/essential-javascript-mastering-immediately-invoked-function-expressions-67791338ddc6)

        EXAMPLE: 
            (function(){
                console.log('IIFE ran..')
            })(); --> console's output IIFE ran..

        EXAMPLE: 
            (function(name){
                console.log('Hello ' + name)
            })('Claire') --> console's output is Hello Claire

## property methods

        EXAMPLE: 
            const todo = {
                add: function(){
                    console.log('Add todo..');
                },
                edit: function(id){
                    console.log(`Edit to do ${id}`);
                }
            }

            todo.delete = function(){
                console.log('Delete todo..')
            }

            todo.add(); --> console's output is Add todo..
            todo.edit(22); --> consoles's output is Edit todo 22
            todo.delete(); --> console's output is Delete todo..