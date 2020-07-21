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

            val = window.location.href --> gets the link of the window. 

            val = window.location.search --> outputs search parameters

## redirect
        EXAMPLE: 
            window.location.href = 'http://google.com' --> redirects your page to google.com

## reload
        EXAMPLE: 
            window.location.reload() --> reloads the page

## history object
    NOTE: the history method will allow the user to go back a page (-1) or several (-2) i.e. first page is Google, second page is Facebook, third page is Twitter. If -1, it will go back to Facebook, if -2 it will go back to Google.
        EXAMPLE:
            window.history.go() 
            
            val = window.history.length; --> console's output is the number of sites that are behind the current site the user is on.

## navigator object

        EXAMPLE:
            val = window.navigator; --> will give the user information about the current navigator is being run, i.e Mozilla or Chrome

            val = window.navigator.appName; --> will give what app name is for the navigator i.e. Netscape

            val = window.navigator.appVersion; --> will give the version/generation of the browser the user is using

            val = window.navigator.userAgent; --> similar to window.navigator.appVersion

            val = window.navigator.platform; --> gives what platform the user is using. 

            val = window.navigator.vendor; --> gives the vendor of the navigator

            val = window.navigator.language; --> gives the language of the navigator i.e. en-US 