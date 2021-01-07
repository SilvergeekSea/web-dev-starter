DOM ( Document Object Model)
Object Properties
create a object

let mySymbol = Symbol(); // create a symbol
let person = {
    name: "john",
    age: 32,
    partTime: false,
    [mySymbol]: 'secretInformation' // using [] is to indicate this is a variable. 
};

console.log(person.name);

person.age = 33;
person['age'] = 33;


