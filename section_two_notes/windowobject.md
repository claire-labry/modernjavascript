## a look at the window object

    NOTE: the DOM is a part of the window object

    NOTE: The window is the global object in client side javascript

    NOTE: node js and Chrome both use the same javascript engine: V8

## window methods / objects / properties

        EXAMPLE: 
            console.log();
            alerts --> alert();
            prompts --> prompt();
            confirm --> confirm();

## outer height & width

        EXAMPLE:
            let val;

            val = window.outerHeight;
            val = window.outerWidth;
            
            console.log(val); --> console outputs the client-side window's outer height or width

## inner height & width     
        EXAMPLE:
            let val;

            val = window.innerHeight;
            val = window.innerWidth;
            
            console.log(val); --> console outputs the client-side window's inner height or width

## scroll points 
        EXAMPLE: 
            let val;

            val = window.scrollY;
            val = window.scrollX;

            console.log(val); --> console outputs the scroll points in a page. 

## location object

        EXAMPLE: 
        
            let val;
            
            val = window.location; --> gets the information about the window's location/pathname
            
            val = window.location.hostname; --> gets the hostname of the window

            val = window.location.port --> gets the port of the window that is being served client-side
