1. clone a repo to local
2. get into cmd and into that folder
3. run npm install to install Java. 
4. npm install will check package.json and check ddevDependencies: and found            lite-server is required. 
5. start terminal and type npm run start
We will work on html page (index.html)

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
account
_account
account_99
$accountNumber (not recommended as it can be used for automatically generated code)

