# datatypes

##  primative datatypes 
    NOTE: these datatypes are usually directly stored in the variable accesses & on the stack
    NOTE: in javascript there are six primative datatypes: string, number, boolean, null, undefined, and symbols (ES6)

## reference datatypes / objects
    NOTE: accessed by reference, data isn't actually stored in the variable-- it's stored on the heap
    NOTE: in javascript reference datatypes are: arrays, object literals, functions, dates, anything else...

## dynamically typed language
    NOTE: types are associated with values not variables
    NOTE: the same variable can hold multiple types
    NOTE: no need to specify types
    NOTE: most other languages are statically typed (java, c#, c++)
    NOTE: there are supersets of javascript & add ons to allow static typing (typescript)


## PRIMATIVE TYPES

<!-- String -->
const name = 'John Doe'
console.log(typeof name) --> outputs in the console what primative datatype name is = string

<!-- Number -->
const age = 45
console.log(typeof age) --> outputs in the console what primative datatype name is = number

<!-- Boolean -->
const hasKids = true
console.log(typeof hasKids) --> outputs in the console what primative datatype name is = boolean

<!-- Null -->
const car = null
console.log(typeof car) --> outputs in the console what primative datatype name is = object (javascript 'bug')
** https://stackoverflow.com/questions/801032/why-is-null-an-object-and-whats-the-difference-between-null-and-undefined ** 

<!-- Undefined -->
let test;
console.log(typeof test) --> outputs in the console what primative datatype name is = undefined

<!-- Symbol -->
const sym = Symbol();
console.log(typeof sym) --> outputs in the console what primative datatype name is = Symbol

## REFERENCE TYPES - Objects

<!-- Array -->
const hobbies = ['movies', 'music']
console.log(typeof hobbies) --> outputs in the console what reference datatype name is = object

<!-- Object Literals -->
const address ={
    city: 'Boston',
    state: 'MA'
}
console.log(typeof address) --> outputs in the console what reference datatype name is = object

const today = newDate();
console.log(today) --> outputs in the console Wed Jul 15 2020 15:29 Central Standard Time
console.log(typeof today) --> outputs in the console what reference datatype name is = object