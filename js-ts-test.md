# How to add question?

---
Question body goes here...

a) first choice
b*) second choice (correct answer is marked with a star)
c) third choice
d) fourth choice

# Up & Going @You Don't Know JS

---
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

# Scope @ Closures @You Don't Know JS

---
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

# this & Object Prototypes @You Don't Know JS

---
Which of these is correct type assertion syntax?

a*) <string>someValue
b*) someValue as string
c)both
d)none of these

# Handbook @typescriptlang.org

---
```typescript
function buildName(firstName: string, lastName?: string) {
    if (lastName)
        return firstName + " " + lastName;
    else
        return firstName;
}
```

# Which is the correct function call?

a*) let result1 = buildName("Bob");
b)  let result2 = buildName("Bob", "Adams", "Sr.");
c*) const result3 = buildName("Bob", "Adams");
d*) var result4 = buildName("Bob");


# Up & Going
---
Which of these are JavaScript types?

a*) object
b*) symbol
c) enum
d) array


# Scope @ Closures
---
Which of the following statement are not true about javascript closures?

a) gives access to an outers f(x) scope from an inner f(x)
b*) outer f(x) cant access global variables
c) inner f2(x) will have access to outers f1(x) variables even after outer f1(x) has returned something
d) inner f(x) cant access global variables

# .this & Object Prototypes
---
``` javascript
var strObject = new String( "I am a string" );
typeof strObject;
```

What is the expected output for typeof?

a*) “object”
b) “instance”
c) “function”
d) “string”

# TypeScript
---
Which of the scopes are available in TypeScript?

a) global scope
b) block scope
c) class scope
d*) all of them