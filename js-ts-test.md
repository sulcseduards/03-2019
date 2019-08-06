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
# Scope @ Closures @You Don't Know JS
function foo(a) {
	console.log( a + b ); // ?
	let b = a;
}
foo( 2 );
---------------------------------------------------
a) 4
b*) NaN
c) 2
d) Error

2.-------------------------------------------------
# this & Object Prototypes @You Don't Know JS
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
-----------------------------------------------------
a*) {a:2}
b) hello
c) 2
d) 4

3.----------------------------------------------------
# Handbook @typescriptlang.org
Which of these is correct type assertion syntax?
a*) <string>someValue
b*) someValue as string
c)both
d)none of these
------------------------------------------------------
# Handbook @typescriptlang.org
function buildName(firstName: string, lastName?: string) {
    if (lastName)
        return firstName + " " + lastName;
    else
        return firstName;
}
a*) let result1 = buildName("Bob");
b)  let result2 = buildName("Bob", "Adams", "Sr.");
c*) const result3 = buildName("Bob", "Adams");
d*) var result4 = buildName("Bob");