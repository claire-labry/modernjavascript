# dates & times

(https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)

## Date() object

        EXAMPLE:
            let val;

            const today = new Date();

            val = today;

            console.log(val) --> console outputs Thu Jul 16 17:57 (Central Standard Time)

        EXAMPLE: 

            let birthday = new Date('9-10-1981 11:25:00')
            let birthday = new Date('September 10 1981')
            let birthday = new Date('9/10/1981')

            val = birthday

            console.log(val) --> outputs Thu Sep 10 1981 00:00:00 (Central Standard Time)

        EXAMPLE: 
    
    NOTE: Months are index based meaning Jan is 0 

            val = today.getMonth()

            console.log(val) --> 6 (July)

        EXAMPLE: 

            val = today.getDate(); (outputs today's date)
            val = today.getDay(); (outputs day, i.e. Monday, Tuesday)
            val = today.getFullYear(); (gets the year, i.e. 2020)
            val = today.getHours(); (gets the hour)
            val = today.getMinutes(); (gets minutes)
            val = today.getSeconds(); (gets seconds)
            val = today.getMilliseconds; (gets milliseconds)
            val = today.getTime; (gets the amount of seconds that have past since 01/01/1970)

        EXAMPLE: 

            val = birthday

            birthday.setMonth(2);
            birthday.setDate(12);
            birthday.setFullYear(1985);
            birthday.setHours(3);
            birthday.setMinutes(30);
            birthday.setSeconds(25)

            
            console.log(birthday) --> Tue Mar 12 1985 03:30:25 GMT-0400 (Eastern Daylight Time)