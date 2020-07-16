# type conversion 

    NOTE: taking a variable and changing the data type 

## CONVERTING A NUMBER TO A STRING
    EXAMPLE: 
        let val;

        val = 5; 

#### output
        console.log(val); --> console outputs 5
        console.log(typeof val); --> console outputs number
        console.log(val.length); --> console outputs undefined

    NOTE: length only works on strings & gives you the number of characters in a string. length does not work on numbers hence why console.log(val.length) returns undefined
    NOTE: However if you wrap the number in a string, the console will output length 

    EXAMPLE: 
        let val;
    (string around a number)
        val = String(5); 
        console.log(val.length); --> console outputs 1 (number of characters)

### string around an expression
        val = String(4+4) --> console outputs 8 (in string format)

## CONVERTING A BOOLEAN TO A STRING
    EXAMPLE: 
        let val;

        val = String(true);

#### output
        console.log(val); --> console outputs true
        console.log(typeof val); --> console outputs string
        console.log(val.length); --> console outputs 4 (number of characters)

## CONVERTING DATE TO STRING
    EXAMPLE: 
        let val;

        val = String(new Date());

#### output
        console.log(val); --> console outputs Wed Jul 15 2020 18:22 (Central Standard Time)
        console.log(typeof val); --> console outputs string
        console.log(val.length); --> console outputs 44 (number of characters)

## CONVERTING AN ARRAY TO STRING
    EXAMPLE: 
        let val;

        val = String([1,2,3,4]);

#### output
        console.log(val); --> console outputs 1,2,3,4
        console.log(typeof val); --> console outputs string
        console.log(val.length); --> console outputs 7 (number of characters)

### toString() Method
    ** https://www.geeksforgeeks.org/javascript-tostring-function/ **

     EXAMPLE:        
        let val;
#### number
        val = (5).toString();
#### boolean
        val = (true).toString();

#### output for number
        console.log(val); --> console outputs 5 (in string format)
        console.log(typeof val); --> console outputs string
        console.log(val.length); --> console outputs 1 (number of characters)
#### output for boolean
        console.log(val); --> console outputs true (in string format)
        console.log(typeof val); --> console outputs string
        console.log(val.length); --> console outputs 4 (number of characters)

## CONVERTING A STRING TO A NUMBER

    EXAMPLE: 
        let val;

        val = Number('5');
#### output for number
        console.log(val); --> console outputs 5 (in number format)
        console.log(typeof val); --> console outputs number
        console.log(val.toFixed()); --> console outputs 5 (number of decimals)

    NOTE: toFixed() method only works on numbers and if you put a number in the parameters, i.e. 2, the console's output would be 5.00 instead of 5. 

### other ways of converting

    EXAMPLE: 
        let val;

        val = Number('5'); --> console outputs 5 (in number format)
        val = Number(true) --> console's output would be 1
        val = Number(false) --> console's output would be 0
        val = Number(null) --> console's output would be 0
        val = Number('hello') --> console outputs NaN
        val = Number ([1,2,3,4]) --> console outputs NaN

### parseInt() Method
    ** https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt ** 

    EXAMPLE: 
        let val;
        
        val = parseInt('100') --> console outputs 100
        val = parseInt('100.30') --> console outputs 100 

    NOTE: with 100.30, parseInt() is just going to parse the number into an integer i.e. 100 

### parseFloat() Method
    ** https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseFloat ** 
    
    EXAMPLE: 
        let val; 
        
        val = parseFloat('100.30') --> console's output is 100.3
        val = parseFloat('100.31') --> console's output is 100.31

        val = parseFloat('100.30') --> console.log(val.toFixed(2)) output is 100.30
        val = parseFloat('100.30') --> console.log(val.toFixed()) output is 100

## TYPE COERCION
    NOTE: Type coercion is the automatic conversion of values from one data type to another (i.e. strings to numbers)
    ** https://developer.mozilla.org/en-US/docs/Glossary/Type_coercion ** 

    EXAMPLE: 
        (without type coercion)
        const val1 = 5;
        
        (with type coercion)
        const val1 = String(5)
        
        const val2 = 6;
        
        (without type coercion to a string(black number in the console))
        const sum = val1 + val2;

        (with type coercion to a number (blue number in the console))
        const sum = Number (val1 + val2);

#### output
        console.log(sum) --> 11 (without type coercion)
        console.log(sum) --> 56 (with type coercion, in a string)
        console.log(sum) --> 56 (with type coercion, in a number)
        console.log(typeof sum) --> number