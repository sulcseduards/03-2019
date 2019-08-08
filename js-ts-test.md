# How to add question?

Question body goes here...

a) first choice  
b*) second choice (correct answer is marked with a star)  
c) third choice  
d) fourth choice  

# Up & Going @You Don't Know JS

```javascript
function foo(a) {
  console.log( a + b );
  let b = a;
}
foo( 2 );
```

What is the output?

a) 4  
b*) NaN  
c) 2  
d) Error  

***

How would you execute (call) this function?

```javascript
(function foo(){
  console.log( "Hello!" );
})();
```

a) This type of function expression syntax is not valid in JavaScript  
b) By calling it with foo();  
c*) No need to call it, it is immediately invoked by () at the end of the expression  
d) By calling it with foo.call();  
  
***

Which of these data types are not available in JavaScript?

a) String  
b) Boolean  
c) Number  
d*) Int  

***

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

---

```javascript
What will be the output for both comparisons?

var a = 41;
var b = "42";
var c = "43";

a < b;
b < c;
```

a*) true, true  
b) true, false  
c) false, true  
d) false, false  

# Scope @ Closures @You Don't Know JS

```javascript
function foo() {
  const a = 4;
  console.log( this.a );
}
var a = {
  a: 2
};
var b = {
  a:a,
  foo:foo,
  b: 'hello'
}
foo.call( b );
```

What is the output?

a*) {a:2}  
b) hello  
c) 2  
d) 4  

***

Which of the following statemenets are false?

a) A block (identified by a pair of curly braces) does not define a new scope for _let_ and _const_, but it does for _var_  
b) A variable defined as _const_ or _let_ is also visible outside that block where it resides  
c) A variable defined as _var_ inside a function is visible in every part of program  
d*) All of the above  

***

```javascript
a=2
var a
console.log(a)
```

What's the expected output?  
a) unidentified  
b) null  
c*) 2  
d) syntax error  

***

What will be in the second output?

var a = 2; (function IIFE( def ){ def( window ); })(function def( global ){ var a = 3; console.log( a ); console.log( global.a ); });

^^ Choice one answer ^^ 

a*) 2  
b) 1  
c) 3  
d) Null  

---

```javascript
a = "42";
b = 42;
c = a == b
console.log(c)
```

What will be printed out in console?

a) Undefined  
b) NaN  
c) False  
d*) True  

# this & Object Prototypes @You Don't Know JS

Which of these is correct type assertion syntax?

a*) <string>someValue  
b*) someValue as string  
c) both  
d) none of these  

***

What does the following code print to the console?

```javascript
var object = {
  foo: function() { return (this === object); }
}
console.log(object.foo());
```

a*) true  
b) false  
c) undefined  
d) ReferenceError: this is not defined  

***

```javascript
class MyClass{
     constructor(){
           this.useless = "UMP"
}
}
```
If you have this class what will happen if we execute this code?:
```javascript
MyClass.useless = "P90"
```
a) UMP" string changes to "P90  
b) syntax error  
c) creates a new variable in the object's instance  
d*) creates a new static variable in MyClass  

***

What will be in the output and what kind of function method is this?

```javascript
var globalObject = this; 
var foo = (() => this); 
console.log(foo() === globalObject);
```

^^ Choice one answer ^^ 

a) false, Simple call  
b) true, The Bind Method  
c*) true, The Arrow Function  
d) false, As an object method  

---

```javascript
var myObject = {};

Object.defineProperty( myObject, "a", {
	value: 2,
	writable: false,
	configurable: true,
	enumerable: true
} );
```

How would you change this objects value to 3?

a) myObject.a = 3;  
b) myObject.value = 3;  
c*) it's not possible  
d) a.value = 3;  

# Handbook @typescriptlang.org

```typescript
function buildName(firstName: string, lastName?: string) {
    if (lastName)
        return firstName + " " + lastName;
    else
        return firstName;
}
```

Which is the correct function call?

a*) let result1 = buildName("Bob");  
b)  let result2 = buildName("Bob", "Adams", "Sr.");  
c*) const result3 = buildName("Bob", "Adams");  
d*) var result4 = buildName("Bob");  

***

```typescript
function buildName(firstName = "Will", lastName: string) {
    return firstName + " " + lastName;
}
```

Which function call would not result in error?

a) let result1 = buildName("Bob");  
b) let result2 = buildName("Bob", "Adams", "Sr.");  
c*) let result3 = buildName("Bob", "Adams");  
d*) let result4 = buildName(undefined, "Adams");  

***

Why is it important to assign data types to variables?

a) The code executes faster, but is a little more complex  
b*) So you dont make a mistake by accidentally adding a different data type to a variable  
c) So the code looks more complex and you'll have bragging rights  
d) So you make less syntax errors  

***

Which are different data types that are supported by Typescript and explain how to implement inheritance? 

a) Boolean: This can have values as true or false Number: This allows creating a user-defined data type. String: This can be any character value Array: This can be a list of numbers together Enum: This can be any number value  
b*) Boolean: This can have values as true or false Number: This can be any number value String: This can be any character value Array: This can be a list of numbers together Enum: This allows creating a user-defined data type.  

***

```markdown
`...` allow us to define a set of named constants. Using `...` can make it easier to document intent, or create a set of distinct cases. TypeScript provides both numeric and string-based `...`.
```

Choose the right missing words for empty space `...`!

a*) Enums.  
b) Classes.  
c) Modules.  
d) Decorators.  