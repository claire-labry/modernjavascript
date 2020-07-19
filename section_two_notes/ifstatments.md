# if statements & comparison operators

    NOTE: if statements are used to evaluate some kind of condition and then do something based on that condition. 

        EXAMPLE:
            if(something){
                do something
            } else{
                do something else
            }

## equal to
        EXAMPLE:
            const id = 100;

            if(id == 100){
                console.log('CORRECT');
            } else {
                console.log('INCORRECT')
            }
    NOTE: console outputs CORRECT 

## not equal to
        EXAMPLE:
            const id = 100;

            if(id != 101){
                console.log('CORRECT');
            } else {
                console.log('INCORRECT')
            }
    NOTE: console outputs CORRECT because 100 does not equal to 101

## equal to value and type
        EXAMPLE:
            const id = '100';

            if(id === 100){
                console.log('CORRECT');
            } else {
                console.log('INCORRECT')
            }
    NOTE: console outputs INCORRECT because id is a string not a number

## equal to value and type (pt. 2)
        EXAMPLE:
            const id = '100';

            if(id !== 100){
                console.log('CORRECT');
            } else {
                console.log('INCORRECT')
            }
    NOTE: console outputs INCORRECT because id not the right value but has the right type

## testing if undefined

        EXAMPLE: 
            const id = 100 (but this is 'commented out')

            if(typeof id !== 'undefined){
                console.log(`The ID is ${id}`)
            } else{
                console.log('NO ID')
            } --> console should output NO ID instead of throwing an error stating that id is undefined    

## greater or less than

        EXAMPLE: 
            const id = '100';

            if(id > 200){
                console.log('CORRECT');
            } else {
                console.log('INCORRECT')
            } --> output is INCORRECT

## if else

        EXAMPLE: 
            const color = 'yellow';

            if(color === 'red'){
                console.log('Color is red!')
            } else if(color === 'blue') {
                console.log('Color is blue!')
            } else{
                console.log('Color is not red or blue')
            }

## logical operators

### and &&
        EXAMPLE: 
            const name = 'Steve';
            const age = 20;

            if(age > 0 && age < 12){
                console.log(`${name} is a child`)
            } else if(age >= 13 && <= 19){
                console.log(`${name} is a teenager`)
            } else {
                console.log(`${name} is an adult`)
            } --> console outputs Steve is an adult. 
    
    NOTE: If you change Steve's age, the console will change based on what age he is. 

### or || 
        EXAMPLE: 
            if( age < 16 || age > 65){
                console.log(`${name} cannot run in race`)
            } else {
                console.log(`${name} is registered for the race`)
            }
    NOTE: If you change Steve's age, the console will change based on what age he is and whether he can run in the race or not.

### ternary operator
        EXAMPLE: 
            const id = 100;
            console.log(id === 100 ? 'CORRECT' : 'INCORRECT') --> console's output is CORRECT.