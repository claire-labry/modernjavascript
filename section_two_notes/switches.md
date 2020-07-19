# switches

    NOTE: Switches are another way to validate conditions. 

        EXAMPLE: 
            const color = 'red';

            switch(color){
                case 'red':
                    console.log('Color is red');
                    break;
                case: 'blue':
                    console.log('Color is blue');
                    break;
                default:
                    console.log('Color is not red or blue');
                break;
            } --> console will output Color is red
    
    NOTE: if user changes colors in the color variable, switch will listen and change the message based on the color. 

        EXAMPLE: 
            let day;

            switch(new Date().getDay()){
            case 0:
                day= 'Sunday'
                break;
            case 1:
                day= 'Monday'
                break;
            case 2:
                day= 'Tuesday'
                break;
            case 3:
                day= 'Wednesday'
                break;
            case 4:
                day= 'Thursday'
                break;
            case 5:
                day= 'Friday'
                break;
            case 6:
                day= 'Saturday'
                break;
            }

            console.log(`Today is ${day}`) --> console will output Today is Saturday