## Loops and Iteration

Loops are a fast way to do something repeatedly. For example in a game where you tell someone to take X steps in one direction and Y steps in another could be expressed as a loop <br>

ex: for (let step = 0; step <5; step++> { 
    //Run 5 imes, with values of step 0 through 4
    console.log('Walking east one step');
}
</br>


## Types Of Loop Statements

* for statement: repeats until specified condition evaluates to false <br>
ex:  for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement </br>
* do while statement
* while statement
* labeled statement
* break statement
* continue statement
* for...in statement
* for...of statement

//Operators in Use

//+,-,/,%

//multiplication uses the (*) symbol
//division used the (/) symbol

console.log(3 * 8);
console.log(4 / 2);
console.log(2 / 4);
console.log (3 + 8);


//modulo returns the remainder of a division operation

console.log(5 % 4);

//The comparison operators
// <,><=,>=,==,!=,===,!==

console.log(3 < 5)>);

var userAge = prompt("Enter your age");

console.log(userAge < 15);)


if (userAge < 15){
  alert("You need parental permission to use this site!");
}

//If user enters "15" they will not be alerted

if (userAge >= 15){
  alert("You are allowed to use this site!");
}


console.log (3==="3");

console.log(3 !== "3");
//in order to be stricly equal, types and values must be the same
//in order to be strictly not equal, one of them must be different


if(userAge < 12){
    if(userAge > 5) {
      alert("You are between 6 and 11 inclusive");
 }
else{
  alert("You are younger than 12 and younger than 6");
  }
}
else{
  alert("You are 12 or older than 12);
  }
}
else if (userAge > 15);{
  alert("You are older than 15");
}
else{
  alert("You are between 12 and 15");
}

//Logical operators
// && (and) || (or) !(not)

//The && returns true if both operands are true otherwise returns false
//The || operator returns true if one operand is true otherwise returns false
//The ! operator returns true if the operand is false otherwise returns false

var sleepy = true;
var hungry = false;

if(sleepy&&hungry){
  alert("You are sleepy and hungry!");

}

if (sleepy||hungry){
  alert("You are sleepy or hungry!");
}

if(!sleepy){
  alert("You are not sleepy");
}

if(!hungry)[
  alert(You are not hungry");
]

//the else if statement runs only if the if statement is false

