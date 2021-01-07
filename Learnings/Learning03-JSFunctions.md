Functions
function showMessage(){
    console.log('in a function');

}

showMessage(){}

function expression

function showMessage(){

}

let myFunction = function showMessage () {
    console.log('Here is a message');
}

myFunction(); // calls the function

You can call showMessage() anymore. Its only for debug purpose. 

Passing data to functions.

function showMessage(message1, message2){
    console.log(message1);
} //this message variable will receive the parameters 
showMessage('test1', 123);
showMessage('test2',456);
if you don't passing down value, it will not alert but showing undefined in the console for the function. 
return value

function getSecretCode(value){
    let code = value*42;
    return code;
}

console.log(getSecretCode(2));

You can create function within the functions. 


