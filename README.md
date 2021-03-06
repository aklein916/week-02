# Quiz #2

## Instructions

1. Fork this repo
2. Clone your fork
3. Fill in your answers by writing in the appropriate area, or placing an 'x' in
the square brackets (for multiple-choice questions).
4. Add/Commit/Push your changes to Github.
5. Open a pull request.

## JavaScript

### Question #1

**What of the following are JavaScript Data Types?**

Select all that apply:
```
[X] Strings
[X] Booleans
[X] Undefined
[] NaN
[X] Integers
[X] Arrays
[X] Null
```

## Question #2

Explain what is a REPL, and why is it important for us as developers and help with debugging?

```
REPL stands for read-eval-print-loop. When we use REPL we can run parts of the code to make sure they works before putting everything together and running it as whole.

```
### Question #3

**Given the Following Array**

var foods = [ ["apple","banana","strawberry"], ["pizza","fries","hamburger"] ];

Create a For Loop that outputs the following string for each piece of fruit in the console. "I want to eat a [fruit]"

```js
for (var i= 0; i< foods[0].length; i+=1) {
  console.log("I want to eat a " + foods[0][i]);
}
```
### Question #4

**Given the Following Array**

var foods = [ ["apple","banana","strawberry"], ["pizza","fries","hamburger"] ];

How would I go about accessing the string "pizza" in the above array?

js
foods[1][0];
```

## Scope/Context/Closures

### Question #5

Describe the rules of scope in JavaScript.

Your Answer:
```--When defined variable uses the var keyword, the variable can only able to be used within the local scope.
  --Variables that are not defined with the var keyword are global variables and can be called from anywhere inside or outside the function.
  --the largest scope includes all inner scopes.
```

### Question #6

Define an object and store it in a variable `pizza`. The object should have 2
properties: a temperature (set to 70), and a method called `bake`. When called,
this method should set the pizza's temperature to be 300. Note: you may not use
the variable pizza inside your method.

Your Answer:
```var pizza = {
    temperature: 70,
    bake: function(){
      this.temperature = 300;
    }
}
```

### Question #7

Define a global variable instructor and set it equal to your Squad Instructor's Name. Then, define the same as a local variable instead.

Your Answer:
```instructor = "Adrian" --global
  var instructor = "Adrian" -- local
```

## Objects and Functions

### Question #8

What are the differences between calling and referencing a function? Please provide examples of each.

```calling a function means executing all of the statements in the function. you call a function like: "myName();""

referencing a function means that you are describing it to use at a later time, rather than asking for the function to be executed and carried out at that moment in the code. "myName" 

```
### Question #9

Using the object literal notation, Define an object called student and give it the properties (your attributes) of name, age, and a method sayHello, that outputs "Hi, my name is [your_name]".

Your Answer:
```js
var student = {
  name: "Alexa",
  age: 25,
  sayHello: function() {
    console.log("Hi, my name is " + this.name);
  }
};
```

## Callbacks

### Question #10

**What is the difference between synchronous and asynchronous program execution?**

Select all that apply:
```
[] Synchronous code runs at an even pace, asynchronous code runs with uneven pacing.
[] Synchronous code runs all at the same time, asynchronous code runs completely randomly
[X] Synchronous code runs in order (as appears in the source), asynchronous code may run at a later time.
```
