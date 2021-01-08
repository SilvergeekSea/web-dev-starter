Creating and initializing Arrays

let values = [1,2,3];
This array has 3 elements.
let values = Array.of(1,2,3);


const values = ['a','b','c'];
console.log(Array.isArray(values));

You can also call Methods. Array.isArray()


Accessing Array Items
console.log(values[0]);

so array can be a constant. but you still able to change elements within the array.

add element in the array (you can call it list in the Python)
const values = ['a'];
values.push('d') //add the element to the end of array. the element is a,b

push can also take more than 1 arguments. so you can push values.push('e','f')

const last = values.pop(); // get last element of array to last variable and remove it from original array

# getting first element of array
const first = values.shift(); // a , the array will only contain 2 values, a is gone.
values.unshift('a'); // add a -> ['b','c']

slice() and splice()
slice() - slice array from (start,stop(but not include)) to get new array
const value = ['a','b','c']
const newValues = values.slice(1,2);
if there is arguments in slice, then it will copy array.

splice ( index want to delete, how many to delete, anything to add)
values.splice(1,0,'foo'); //a foo b c

Array searching and looping
const values = ['a','b','c']
console.lg(values.indexof('c')); // 2
if the letter is not there, you will get -1
const set = values.filter(function(item){
    return item > 'b';
})


// find()
const found = values.find (function(item){
    return item.length > 1;
}); // bbb

values.forEach(function(item){
    console.log(item);
})

Scope and hoisting
global Scope
function scope
undeclared variables
strict mode

# Global Scope
Global scope is crossing multiple js files.
don't define same variables all over the places.
best practice is to create a const app
const app = {
    productid: 1234,
    userName: 'Joe',
    orderNumber: 893
};

so we will put all variables in there instead of everywhere.

functions don't need to be predefined. It will be hoisted.
Javascript will run twice through your script. It check all functions first. then 2nd time, it will execute the function.

'use strict';
then you ust declar variable before your script