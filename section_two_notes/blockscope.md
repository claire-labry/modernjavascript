# block scope with let & const

## global scope
        EXAMPLE: 
            var a = 1;
            let b = 2;
            const c = 3;

            console.log('Global Scope: ', a,b,c) --> output is Global Scope: 1 2 3 

function test(){
            var a = 4;
            let b = 5;
            const c = 6;
            console.log('Function Scope: ' a,b,c)
            }

            test(); --> console's output is Function Scope: 4 5 6 

        if(true){
            *block scope* 
            var a = 4;
            let b = 5;
            const c = 6;
            console.log('If Scope: ' a,b,c)
            }
        }

        for(let a = 0; a < 10; a++){
            console.log(`Loop:{a}`)
        } --> outputs Loop: # 