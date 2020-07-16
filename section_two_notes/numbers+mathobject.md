# numbers & the math object

## SIMPLE MATH WITH NUMBERS

### (addition)
        EXAMPLE:
            const num1 = 100;
            const num2 = 50;
            let val;

            val = num1 + num2;

            console.log(val); --> console's output 150 (primative type: number)

### (multiplication)
        EXAMPLE:
            const num1 = 100;
            const num2 = 50;
            let val;

            val = num1 * num2;

            console.log(val); --> console's output 5000 (primative type: number)

### (subtraction)
        EXAMPLE:
            const num1 = 100;
            const num2 = 50;
            let val;

            val = num1 - num2;

            console.log(val); --> console's output 50 (primative type: number)

### (division)
        EXAMPLE:
            const num1 = 100;
            const num2 = 50;
            let val;

            val = num1 / num2;

            console.log(val); --> console's output 2 (primative type: number)

### (modulus operator - leftover as a remainder)
        EXAMPLE:
            const num1 = 100;
            const num2 = 50;
            let val;

            val = num1 % num2;

            console.log(val); --> console's output 0 (primative type: number)

## MATH OBJECT 

    NOTE: Javascript Math object (method) allows users to perform mathematical tasks on numbers. Math Object is a method and .PI is a attribute. 
    NOTE: Property is basically like an attribute and method is just a function

        EXAMPLE: 
            val = Math.PI;

            console.log(val); --> console's output is Pi 3.14...
    
    NOTE: Math.round() rounds up numbers by the decimal point
        
        EXAMPLE:
            val = Math.round(2.8);

            console.log(val); --> console's output is 3.

    NOTE: Math.ceil() rounds up numbers upward to its nearest integer
        
        EXAMPLE:
            val = Math.round(2.4);

            console.log(val); --> console's output is 3.

    NOTE: Math.floor() rounds up numbers downward to its nearest integer
        
        EXAMPLE:
            val = Math.round(2.8);

            console.log(val); --> console's output is 2.

    NOTE: Math.sqrt() returns the square root of a number
        
        EXAMPLE:
            val = Math.round(64);

            console.log(val); --> console's output is 8.

    NOTE: Math.abs() returns the absolute value of a number
        
        EXAMPLE:
            val = Math.abs(-3);

            console.log(val); --> console's output is 3.

    NOTE: Math.pow() returns the value of the number (ie. 4) to the power of 3 (4*4*4)
        
        EXAMPLE:
            val = Math.pow(8,2);

            console.log(val); --> console's output is 64.

    NOTE: Math.min() returns the minimum number in the parameters
        
        EXAMPLE:
            val = Math.min(2,33,4,1,55,6,3,-2);

            console.log(val); --> console's output is -2.

    NOTE: Math.max() returns the maximum number in the parameters
        
        EXAMPLE:
            val = Math.max(2,33,4,1,55,6,3,-2);

            console.log(val); --> console's output is 55.

    NOTE: Math.random() returns a random number

    NOTE: val will output a randomly generated decimal in the console. if you keep reloading the browser, a new decimal will be generated.
        
        EXAMPLE:
            val = Math.random(); 

            console.log(val); --> random generated decimal number (only good if you want decimals but not for whole numbers)
            
    NOTE: Now, mulitplying 20 to Math.random() will generate a number that is between 1-20 with a decimal.

        EXAMPLE:
            val = Math.random() * 20;

            console.log(val); --> random generated decimal number between 1-230 (only good if you want decimals but not for whole numbers)

    NOTE: Now, mulitplying 20 + 1 to Math.random() and wrapping it around with Math.floor() will generate a whole number that is between 1-20. (very common in javascript)

        EXAMPLE:
            val = Math.floor(Math.random() * 20 + 1);

            console.log(val); --> --> random generated whole number between 1-20