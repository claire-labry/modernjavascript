# general loops

## for loops
    NOTE: general rule of thumb, when using for loops is best to use it when you know how many iterations it's going to have. 

        EXAMPLE: 
            for(let i = 0; i < 10; i++){
                console.log('Number ' + i)
            } --> console's output is Number 0-9

        EXAMPLE: 
            for(let i = 0; i < 10; i++){
                if(i === 4){
                    console.log('Number 4 is my favorite number!')
                    continue; 
                }
                console.log('Number ' + i)
            } --> console's output: Number 4 is my favorite number!
        
        EXAMPLE: 
            for(let i = 0; i < 10; i++){
                if(i === 4){
                    console.log('Number 4 is my favorite number!')
                    continue; 
                } if(i === 5){
                    break;
                }
                console.log('Number ' + i)
            } --> console's output: Numbers 0, 1, 2, 3, Number 4 is my favorite number!

    NOTE: the continue statement tells the loop to pick up after the selected iteration. the break statement tells the loop to stop before the selected iteration.

## while loops
    NOTE: general rule of thumb, when using while loops is best to use it when you don't know how many iterations it's going to have. 

        EXAMPLE: 
            let i = 0; 

            while( i < 10){
                console.log('Number ' + i);
                i++
            } --> console's output is Number 0-9

## do while loops
    NOTE: a do while loop is different because it's always going to run at least once. regardless if you change the iteration to 100, and the while is left as is, the console will still say Number 100;
        EXAMPLE:
            let i = 0;

            do{
                console.log('Number ' + i);
                i++;
            }

            while(i < 10);

## loop thru array
        EXAMPLE:
    NOTE: the console will output the index numbers of the array.
            const cars = ['Ford', 'Chevy','Honda','Toyota'];

            for(let i = 0; i < cars.length; i++){
                console.log(i)
            } --> console's output is 0-3

        EXAMPLE:
    NOTE: the console will output the values in the array because its variable is being called in the console.log
            const cars = ['Ford', 'Chevy','Honda','Toyota'];

            for(let i = 0; i < cars.length; i++){
                console.log(cars[i])
            } --> console's output is 0-3

## forEach 
        EXAMPLE: 
            cars.forEach(function(car){
                console.log(car)
            }); --> loops through the array and the console shows car values

        EXAMPLE: 
            cars.forEach(function(car, index){
                console.log(`${index} : ${car}`)
            }); --> loops through the array and the console shows car values


## map
        EXAMPLE:
            const users = [
                {id: 1, name:'John'},
                {id: 2, name:'Sara'},
                {id: 3, name:'Bob'}
            ];
            
            const ids = users.map(function(user){
                return user.id;
            })

            console.log(ids); --> console outputs the indexes of users in an array

## for in loops

        EXAMPLE: 
            const user = {
                firstName: 'John',
                lastName: 'Doe',
                age: 40
            }

            for (let x in user){
                console.log(x)
            } --> console outputs firstName, lastName, age
            
        EXAMPLE: 
            const user = {
                firstName: 'John',
                lastName: 'Doe',
                age: 40
            }

            for (let x in user){
                console.log(`${x} : ${user[x]}`);
            } --> console outputs firstName : John , lastName : Doe , age : 40