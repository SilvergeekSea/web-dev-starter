if (5===5) {
    console.log('yes')
}

if (5>=5) {
    console.log('yes')
}
>=, >, ===, !==, (no double ==)
if (true) {

}

false list:
false, 0, empty string( eg: "", or '' or ``), null, undefined, NaN

if (+(1.1+1.3).toFixed(2) !==2.4){
    showMessage('true')
}
when you use xx.toFix, it actually converts it to a string. 
so we add + in front to convert it back to number. 
2 decimal spaces.

if (state ==='FL'){
    tx = 7;
}
else{
    tx =6;
}
if (){

}
else if (){

}

double == will convert and compare
if (1 == "1"){
    showMessage('true')
}
it converts 1 to "1" and compare, so best to avoid it. 

Ternar Operator

let message = (price > 10) ? 'expensive' : 'cheap';

if we define a variable in the code block, then when that block finished, so is the variable. 
if (true){
    let x = 3;
}

so if you use var, then it will leak out. 

for () loop
for (let i =0; i < 3; i++) {
    console.log(i)
}

while() Loop
Let count =1;
while (count < 5) {
    console.log(count);
    count++
}

let count =1 ;
do {
    console.log(count);
    count++;

} while (count<5);
