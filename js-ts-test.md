# How to add question?

---
Question body goes here...

a) first choice
b*) second choice (correct answer is marked with a star)
c) third choice
d) fourth choice

# Up & Going @You Don't Know JS

# Scope @ Closures @You Don't Know JS

# this & Object Prototypes @You Don't Know JS

# Handbook @typescriptlang.org

1.-------------------------------------------------
function foo(a) {
	console.log( a + b );
	let b = a;
}
foo( 2 );

What is the output?
a) 4
b*) NaN
c) 2
d) Error

2.-------------------------------------------------
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

What is the output?
a*) {a:2}
b) hello
c) 2
d) 4

3.----------------------------------------------------
Which of these is correct type assertion syntax?
a*) <string>someValue
b*) someValue as string
c)both
d)none of these

4------------------------------------------------------
function buildName(firstName: string, lastName?: string) {
    if (lastName)
        return firstName + " " + lastName;
    else
        return firstName;
}
which is the correct function call?
a*) let result1 = buildName("Bob");
b)  let result2 = buildName("Bob", "Adams", "Sr.");
c*) const result3 = buildName("Bob", "Adams");
d*) var result4 = buildName("Bob");

Which expression is true?
a) typeof {a:"Meow", b:666, "cat"} == 'object' b*) typeof ["Meow", 666, "cat"] == 'object' c) typeof {"cat"} == 'object' d) all are true

Which two mechanisms in JavaScript can "cheat" lexical scope?
a*) eval(..) and with b) setTimeout(..) and with c) eval(..) and setTimeout(..) d) all answers are correct

What is a constructor?
a*) A special method of the class used to construct instances of classes b) Another name for programmer c*) A method of the class which initializes any information (state) the instance will need. d) A function that is called when a class property is read from or written to.

How would this expression be written using typescript? 
let a=[[1,2],[3,4]];

a) let a: Array[]=[[1,2],[3,4]]; b) let a: number[]=[[1,2],[3,4]];  c*) let a: number[][]=[[1,2],[3,4]]; d) let a: Array[][]=[[1,2],[3,4]];