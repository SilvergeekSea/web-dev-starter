1. clone a repo to local
2. get into cmd and into that folder
3. run npm install to install Java.
4. npm install will check package.json and check ddevDependencies: and found            lite-server is required.
5. start terminal and type npm run start
We will work on html page (index.html)

Error:
code UNABLE_TO_GET_ISSUER_CERT_LOCALLY
solution:
npm config set registry http://registry.npmjs.org/

npm audit fix


<script>
    // JavaScript code goes here...
</script>

We will put JS before closing body type.
</body>

Its best to put Java script into own file rather than embedded HTML.
so it can be shared with multiple pages.

<script src="./filename.js"></script>
# When you put JS at the end, it will be loaded after all html content loaded.
whitespace doesn't matter, but not recommened to put it.

You can use console.log("hi, Console..."); to putout into console (which is on website and right click to choose inspect and select console. )
Java Script is case sensitive.

comment code
//Single line comment, it can be anywhere.

/*
    Multiple lines comment

*/

You need to Declaring Variables
"let" define a variable
it's best practice to end line with ";"


let total = 149.99;
let product = 'Hiking Boots';
let discounted = true;

or
// remember the whitespace doesn't count
let welcome = 'Welcome',
     price = 49.99,
     name = 'Hiking boots',
     discounted = false;

clearly, you can't redefine the variable twice

You can't create a variables with keywords.

Valid Variable Names
start with one of those:
_, $ , letter

Followed by Zero or More:
_, $, letter, number

suggest to use lower case camel notation
account (recommend)
_account
account_99
accountNumber (recommend)
$accountNumber (not recommended as it can be used for automatically generated code)
_123
__proto__
if you don't give value to variable, then the value is none but no error.
You can see it in the console.log(price);

Constant doesn't change.
const priceCon = 22;
it will generate typeerror if you try to assign value to constant.
if there is no initial value, then you will get syntax error as constant is not assigned value.

try not to use var as keyword.
the difference between var and let:
showMessage(price)
let price = 25; // you will GET error and not get value.
if you use var price = 25; // you don't get value and  error.


show typeof
showMessage(typeof price);
get reminder
price = 12;
price = price % 5;
price += 5;
incremen
++price;
price++;

opeartion precedence (google it, high will run first)
Java 1.1+1.3 = 2.40000000000004 , so be careful on comparing.

string:
escape is \
\" = "
search string escape notation
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String

you can creat string with backtick `hello`;
let name = 'Silver';
let message = `hello, ${name}`;
It does able to create new lines (but may not showing on page as it automatically change it to space)
let message = `hello,


${name}`;
Parentheses

working on string
message = message.toLowerCase(); (method)
message.length (property)
amount.toString(); (convert to string)
number.parseFloat("123.12") (convert from string to number)
if you get wrong number(mixing with a letter), you will get NaN (not a number)
interesting enough it doesn't care about end 12.12A is fine. but not A12.12.

boolean
let saved = true;
saved = !saved;

null and undefined.
if you don't define a variable, you can see from console.log shows undefined.
but you can wipe out value as well,
saved = null;
but you get null not undefined.


Object and Symbols
let person = {
    firstName: 'John',
    lastName: 'Adams'
}
so this is object with attributes.
showMessage(person.firstName);
It also has method which can run it's own code.

Symobols
