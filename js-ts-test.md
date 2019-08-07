# Up & Going @You Don't Know JS
1. What is the output? 
var a = [1,2,3]; 
var b = [1,2,3]; 
var c = "1,2,3";

a == c; 
b == c; 
a == b;

^^ Choice one answer ^^ 
a) NaN 
b) false, true, true 
c*) true, true, false 
d) Undefiend

#Scope @ Closures @You Don't Know JS
2. What will be in the second output?

var a = 2; (function IIFE( def ){ def( window ); })(function def( global ){ var a = 3; console.log( a ); console.log( global.a ); });

^^ Choice one answer ^^ 
a*) 2 
b) 1 
c) 3 
d) Null

#this & Object Prototypes @You Don't Know JS
3. What will be in the output and what kind of function method is this?

var globalObject = this; 
var foo = (() => this); 
console.log(foo() === globalObject);

^^ Choice one answer ^^ 
a) false, Simple call 
b) true, The Bind Method 
c*)true, The Arrow Function 
d) false, As an object method

#Handbook @typescriptlang.org
4. Which are different data types that are supported by Typescript and explain how to implement inheritance? 

a)Boolean: This can have values as true or false Number: This allows creating a user-defined data type. String: This can be any character value Array: This can be a list of numbers together Enum: This can be any number value
b*) Boolean: This can have values as true or false Number: This can be any number value String: This can be any character value Array: This can be a list of numbers together Enum: This allows creating a user-defined data type.