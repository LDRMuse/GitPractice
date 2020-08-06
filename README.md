//////////Numbers//////////

Numbers can be convented from a String using parseInt(), but if you want to output a number that always uses base 10, then parseFloat() is the way to go as it always uses base 10.

NaN means not a number

parseFloat("10.2abc") will output 10.2 because it stops after a non number is introduced

//////////Strings///////////

'supercalifragilistcexpialidocious'.length //33

'supercalifragilistcexpialidocious'.charAt(0); // "s"
means the first character of hello is 's'

null - is an on purpose non-value
undefined - is a value that has not been assigned which is false

////////Variables////////////

let, const or var declares a variable

let variables can be changed
const variables can only be declared once globally or once within a block

var does not have the same restrictions as let and const do. var can be visible outside of a scope.

/////////Operators/////////


+ - * / %

Values get assigned by using =
and === means whatever is before and after the === must be the same

++ increments as -- decrements

+ is used to concat


//////////////Control Structures////////////

if and else are conditional statements that check if something is true or false based on the condition

while and do-while is a loop that only works until a condition is met

for loop goes through s block of code a number of times until it goes as long as you want

/////////////Objects////////////////

key: value pairs (the values can also be objects)

to create an empty object, you would assign a variable name, use = operator and {} after the =
ex.)  const myObject = {}

to get nested data from an object, you would have to use [] notation. 

/////////////Arrays/////////////

Arrays are like objects but can use 'length' to go through the length of the array to return the data you want

you can go over each object in an array using a for loop or other methods like map() and filter()

you can add to an array using push()
... adds to an array


//////////////functions/////////////

functions are a type of object

there's static functions and functions created by the programmer

you must use 'return' in your function or else it will log undefined

this refers to the current object. if this was called using dot or bracket notation, this refers to the object that called this.

if not, this is called globally


*** below is something that confused me ****

var s = 'Simon';
s.reversed(); // TypeError on line 1: s.reversed is not a function

String.prototype.reversed = function() {
  var r = '';
  for (var i = this.length - 1; i >= 0; i--) {
    r += this[i];
  }
  return r;
};

s.reversed(); // nomiS


