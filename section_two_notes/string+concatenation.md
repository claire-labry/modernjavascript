# string methods & concatenation 


## Simple string method
        EXAMPLE: 
            const firstName = 'William'
            const lastName = 'Johnson'

            let val; 

            val = firstName + lastName

            console.log(val) --> console's output is WillamJohnson

## Concatenation
    ** https://medium.com/@endubueze00/javascript-basics-string-concatenation-with-variables-and-interpolation-deba239debbe ** 
    NOTE: to concatenate a string, simply add a + sign between the string / strings variable that you want to connect. 

        EXAMPLE: 
            const firstName = 'William'
            const lastName = 'Johnson'

            let val; 

            val = firstName + ' ' + lastName

            console.log(val) --> console's output is Willam Johnson

## Append 
    NOTE: Appending something means that user can add onto a variable, but not replace it. Simply adding a + next to = will append your strings. 

        EXAMPLE:
            let val; 

            val = 'Claire ';
            val += 'Labry';

            console.log(val) --> console's output is Claire Labry
        
    NOTE: This concatenation method below works with ES6/ES2015    
        EXAMPLE: 
            const firstName = 'William';
            const lastName = 'Johnson';
            const age = 36;

            let val;

            val = 'Hello, my name is ' + firstName + ' and I am ' + age;

            console.log(val) --> console's out put is Hello, my name is Willam and I am 36

## Escaping
    NOTE: Escaping is adding a special character such as a backslash or regexps type characters to help neutralize a string. 
 
        EXAMPLE: 
            val = 'That\'s awesome, I can\'t wait';
            
            console.log(val) --> outputs That's awesome, I can't wait. 
    
    NOTE: this is used to help with using single quotations because if you have multiple single quotations in a string, it will not translate correctly via your editor/server. 

## Length
    NOTE: the .length will count how many characters there are in the string

        EXAMPLE:
            val = firstName.length;

            console.log(val) --> outputs 7
    

## concat() Method
     NOTE: Works similarly as concatenation mentioned above (concatenating manually) This is a method(function) of concatenating strings. 

        EXAMPLE: 
            const firstName = 'William';
            const lastName = 'Johnson';
            
            val = firstName.concat(' ', lastName)

            console.log(val) --> outputs Willam Johnson

## changing cases
    NOTE: methods that change the string to upper or lowercase.

        EXAMPLE: 
            const firstName = 'William';
            const lastName = 'Johnson';
            
            val = firstName.toUpperCase();

            console.log(val) --> outputs WILLIAM
        
        EXAMPLE: 
            const firstName = 'William';
            const lastName = 'Johnson';
            
            val = firstName.toLowerCase();

            console.log(val) --> outputs william

## indexOf() Method
    NOTE: if user wants to find the index of a value or character 

        EXAMPLE: 
            val = firstName.indexOf('l')

            console.log(val) --> outputs 2 
    NOTE: l has an index of 2 in William. 

        EXAMPLE: 
            val = firstName.lastIndexOf('l')

            console.log(val) --> outputs 3
    NOTE: lastIndexOf finds the last index of l, which in William, it will be 3. 

## charAt() Method
    NOTE: this method returns the character at the specified index in a string

        EXAMPLE: 
            val = firstname.charAt('2')

            console.log(val) --> console's output will be l 

## getting the last char

        EXAMPLE: 
            val = firstName.charAt(firstName.length - 1)

            console.log(val) --> m 
    NOTE: adding the -1 gets you the last value of the string since index starts at 0. 

## substring()

        EXAMPLE:
            val = firstName.substring(0,4);

            console.log(val) --> console outputs Will 
    NOTE: substring() will get you the starting index (i.e. 0) to whatever index you will like to end at (i.e. 4) resulting to Will from William

## slice()

        EXAMPLE: 
            val = firstName.slice(-3);
            console.log(val) --> iam 
    NOTE: gets the last three letters of William

## split()

        EXAMPLE: 
            const str = 'Hello there my name is Claire';

            val = str.split(' ')

            console.log(val) --> outputs (6) ["Hello", "there", "my", "name", "is", "Claire"]

        EXAMPLE:
            const tags = 'web design,web development,programming'

            val = tags.split(',') --> outputs (3) ["web design", "web development", "programming"]

## replace()

        EXAMPLE: 
            val = str.replace('Claire', 'Ruan')

            console.log(val) --> outputs Hello there my name is Ruan

## includes()
    NOTE: includes() helps with trying to find if a word is contained in a string by boolean(true or false)

        EXAMPLE: 
            val = str.includes('Hello')

            console.log(val) --> true

        EXAMPLE: 
            val = str.includes('foo')

            console.log(val) --> false
