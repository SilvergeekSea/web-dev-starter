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

let person = {
    name: "john",
    age: 32,
    partTime: false,
    showInfo: function(){
        showMessage(this.name);
    }
};
person['age'] = 45;

person.showInfo();

this = current object.
let person = {
    name: "john",
    age: 32,
    partTime: false,
    showInfo: function(realAge){
        showMessage(this.name+ 'is '+ realAge);
    }
};
person['age'] = 45;

person.showInfo(34);

Passing Objects to functions.
in short, string, integer, boolean are immutable. but object is mutable.
so when you pass object into function, it does change.
let person = {
    name: "john",
    age: 32,
    partTime: false,
    showInfo: function(realAge){
        showMessage(this.name+ 'is '+ realAge);
    }
};
function incredmentAge(person){
    person.age++;
}
incredmentAge(person);
showMessage(person)

# Standard Build-in object
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects


let now = new Date();

//incredmentAge(person);
showMessage(now.toDateString());

showMessage(Math.abs(-42));
let s = "Hello";

//incredmentAge(person);
showMessage(s.charAt(0));


DOM (Document Object Model)
events , actions regarding web page.
document = webpage.
.getElementbyId('message')
it called mehtod textcontext
https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model
check DOM interfaces
check element
element is something like with tag on website like <h2 id='message'> <div> then you can tag it with a tag.

function showMessage(message){
    document.getElementById('message').textContent = message;
}

style with JS
search MTMLElement in MDN
check style
HTMLElement.style
const header = document.getElementById('message');
header.style.color = 'red';
header.style.fontWeight = 100;

Detecting Button Clicks
const button = document.getElementById('see-review');
button.addEventListener('click', function(){
    console.log('click');
}

# add/remove review
const button = document.getElementById('see-review');
button.addEventListener('click', function(){
    console.log('click');
    const review = document.getElementById('review');
    if (review.classList.contains('d-none')){
        review.classList.remove('d-none');
    }
    else {
        review.classList.add('d-none');
    }

}


const button = document.getElementById('see-review');
button.addEventListener('click', function(){
    console.log('click');
    const review = document.getElementById('review');
    if (review.classList.contains('d-none')){
        review.classList.remove('d-none');
        button.textContent='CLOSE REVIERW';
    }
    else {
        review.classList.add('d-none');
        button.textContent='see REVIERW';
    }

}


)