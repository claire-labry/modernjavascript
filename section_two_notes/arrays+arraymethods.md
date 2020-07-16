# arrays & array methods

## creating some arrays

        EXAMPLE: 
            const numbers = [43,56,33,23,44,36,5];
            const numbers2 = new Array(22,45,33,76,54);
            const fruit = ['Apple', 'Banana', 'Orange', 'Pear'];
            const mixed = [22,'Hello', true, undefined, null, {a:1, b:1}, new Date()]

            console.log(mixed) --> outputs the array stored in the mixed variable in the console. 

            let val;

            console.log(numbers); --> outputs in the console the array of the numbers variable
            console.log(val); --> outputs undefined because it's not currently defined

## getting array length

        EXAMPLE:
            const numbers = [43,56,33,23,44,36,5];
            let val;

            val = numbers.length;

            console.log(numbers); --> outputs in the console the array of the numbers variable
            console.log(val); --> outputs 7

## check if it's an array

        EXAMPLE:
            const numbers = [43,56,33,23,44,36,5];
            let val;

            val = Array.isArray(numbers);

            console.log(numbers); --> outputs in the console the array of the numbers variable
            console.log(val); --> outputs boolean true

## get a single value

        EXAMPLE:
            const numbers = [43,56,33,23,44,36,5];
            let val;

            val = number[3];

            console.log(numbers); --> outputs in the console the array of the numbers variable
            console.log(val); --> 23

## inserting into an array

        EXAMPLE:
            const numbers = [43,56,33,23,44,36,5];
            let val;

            numbers[2] = 100;

            console.log(numbers); --> outputs in the console the array of the numbers variable, which now includes 100 in the index of 2 position in the numbers array i.e. [43,56,100,23,44,36,5]
            console.log(val); --> outputs boolean true

## find index of value

        EXAMPLE:
            const numbers = [43,56,33,23,44,36,5];
            let val;

            val = numbers.indexOf(36);

            console.log(numbers); --> outputs in the console the array of the numbers variable
            console.log(val); --> outputs 5

## mutating arrays
    
    NOTE: push() method will allow to add a value to the end of an array.

        EXAMPLE:
            numbers.push(250)

            console.log(numbers); --> outputs in the console the array of the numbers variable with 250 in the end i.e. [43,56,100,23,44,36,5,250]
            
    NOTE: unshift() method will allow to add a value to the beginning of an array.

        EXAMPLE:
            numbers.unshift(120)

            console.log(numbers); --> outputs in the console the array of the numbers variable with 120 in the beginning i.e. [120,43,56,100,23,44,36,5,250]

    NOTE: pop() method will allow to take off a value from the end of an array.

        EXAMPLE:
            numbers.pop()

            console.log(numbers); --> outputs in the console the array of the numbers variable with 250 deleted from the end i.e. [120,43,56,100,23,44,36,5]
    
    NOTE: shift() method will delete a value from the beginning of an array.

        EXAMPLE:
            numbers.shift()

            console.log(numbers); --> outputs in the console the array of the numbers variable deleting 120 in the beginning i.e. [43,56,100,23,44,36,5]

NOTE: splice() method will allow a value in array to be deleted.

        EXAMPLE:
            numbers.splice(1,1) (you will need to tell it which indexOf you want to start and end )

            console.log(numbers); --> outputs in the console the array of the numbers variable with 56 being deleted i.e. [43,100,23,44,36,5] 

NOTE: reverse() method will reverse the numbers in the array.

        EXAMPLE:
            numbers.reverse()

            console.log(numbers); --> outputs in the console the reversed array i.e. [5,36,44,23,100,43]

## concatenating arrays

        EXAMPLE:
            val = numbers.concat(numbers2)

            console.log(val) --> outputs the numbers array and numbers2 array added together resulting in 9 values in the array. 

## sorting arrays
        
        EXAMPLE:
            val = fruit.sort()

            console.log(val) --> outputs the fruits array in alphabetical order i.e. ['Apple', 'Banana', 'Orange', 'Pear'];

## using the compare function

        EXAMPLE (ascending order):
            val = numbers.sort()

            console.log(val) --> outputs the numbers out of order and can be fixed with the compare function

            val = numbers.sort(function(x,y){
                return x-y; 
            })
            
            console.log(val) --> outputs the numbers array in order from least to largest i.e. [5,23,36,43,44,56,100]

## reverse sort
        
        EXAMPLE (descending order):
            val = numbers.sort()

            console.log(val) --> outputs the numbers out of order and can be fixed with the compare function

            val = numbers.sort(function(x,y){
                return y-x; 
            })
            
            console.log(val) --> outputs the numbers array in order from least to largest i.e. [100,56,44,43,36,23,5]

## find
    NOTE: find() allows you to add a function to find a specific number in an array
        EXAMPLE:
           function under50(num) {
               return num < 50;
           }

           val = numbers.find(under50)

           console.log(val) --> outputs 43