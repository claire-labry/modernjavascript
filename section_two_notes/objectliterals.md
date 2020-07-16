# object literals

    NOTE: a javascript object literal is a comma-seperated list of name-value pairs wrapped in curly braces. object literals encapsulate data, enclosing it in a tidy package. minimizes the use of global variables in which could cause problems when combining code down the road. 

    * https://www.dyn-web.com/tutorials/object-literal/ *

        EXAMPLE: 
            const person = {
                firstName: 'Steve',
                lastName: 'Smith',
                age: 30,
                email: 'steve@aol.com',
                hobbies: ['music', 'sports'],
                address: {
                    city: 'Miami',
                    state: 'FL'
                },
                getBirthYear: function(){
                    return 1987;
                }
            }

            let val;

            val = person;

            console.log(val); --> outputs {firstName: "Steve"}

## getting a specific value

        EXAMPLE: 
            val = person.firstName; 
            val person['firstName']; (same output as above)

            console.log(val); --> outputs Steve

## getting a specific value (pt. 2)

        EXAMPLE: 
            val = person.firstName; (outputs Steve)
            val = person['lastName']; (outputs Smith)
            val = person.age;(outputs 30)
            val = person.hobbies[1]; (outputs sports)
            val = person.address.state; (outputs FL)
            val = person.address['city'] (outputs Miami)
            val = person.getBirthYear(); (outputs 1987)

            console.log(val); --> outputs all of the values mentioned in the person array. 

## getting a specific value (pt. 3)

        EXAMPLE(pulling function from person array from above): 

            getBirthYear: function(){
                    return 2017 - this.age;
                }
            
            val = person.getBirthYear(); (outputs 1987)

            console.log(val); --> outputs all of the values mentioned in the person array.

## an array of multiple people

        EXAMPLE: 
            const people = [
                {name: 'John', age: 30},
                {name: 'Mike', age: 23},
                {name: 'Nancy', age: 40}
            ];

            for(let i = 0; i < people.length; i++){
                console.log(people[i].name)
            } --> console outputs John Mike Nancy