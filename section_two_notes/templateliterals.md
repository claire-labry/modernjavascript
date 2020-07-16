# template literals

(https://www.javascripttutorial.net/es6/javascript-template-literals/)

NOTE: prior to ES6, you had the ability to use single or double quotes to wrap a string literal. those have very limited functionality. to be able to solve more complex problems, ES6 template literals provides the syntax (backticks) that allows to write code in a safer & cleaner way. 
    * this allows for: 
        - multiline strings: a string that can span multiple lines
        - string formatting: the ability to substitute part of the string for the values of variables or expressions. (string interpolation)
        - HTML escaping: the ability to transform a string that it is safe to include in HTML. 

## without template strings (es5)
        EXAMPLE:
            const name = 'John';
            const age = 30;
            const job = 'Web Developer';
            const city = 'Miami';
            let html;

            html = '<ul><li>Name: ' + name + '</li><li>Age: ' + age + '</li><li>Job: ' + job + '</li><li>City: ' + city + '</li></ul>'

            document.body.innerHTML = html;

    NOTE: this will output on the server as an unordered bulleted list outlining the details mentioned in the variable, html. 
            * Name: John
            * Age: 30
            * Job: Web Developer
            * City: Miami

        EXAMPLE: 
            html: '<ul>' +
                    '<li>Name: ' + name + '</li>' +
                    '<li>Age: ' + age + '</li>' +
                    '<li>Job: ' + job + '</li>' +
                    '<li>City: ' + city + '</li>' +
                  '</ul>';
    NOTE: Outputs the same thing on the server, but this code is much more prettier than the above code, but it is time consuming (aka pain in the neck). 

## with template strings (es6)
        EXAMPLE: 
            html = `
                <ul>
                    <li>Name: ${name}</li>
                    <li>Age: ${age} </li>
                    <li>Job: ${job}</li>
                    <li>City: ${city}</li>
                </ul>
            `;
    NOTE: Outputs the same thing on the server, but this code is much more prettier and simpler than the above code, and is way less time consuming. Much more efficient. 

        EXAMPLE:

            function hello(){
                return 'hello';
            }


            html = `
                <ul>
                    <li>Name: ${name}</li>
                    <li>Age: ${age} </li>
                    <li>Job: ${job}</li>
                    <li>City: ${city}</li>
                    <li>${2+2}</li> (simple addition)
                    <li>${hello()}</li>(adding function)
                    <li>${age > 30 ? 'Over 30' : 'Under 30'}</li> (conditionals)
                </ul>
            `;

    NOTE: This outputs on the server: 

            * Name: John
            * Age: 30
            * Job: Web Developer
            * City: Miami
            * 4
            * hello
            * Under 30
