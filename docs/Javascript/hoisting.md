# Hoisting

Hoisting is a behavior in JavaScript where variable and function declarations are moved to the top of their containing scope during the compilation phase, before the code is executed. This means that regardless of where variables and functions are declared in the code, they are actually processed first by the JavaScript engine.

#### Example 

```bash 
console.log(x); // undefined
var x = 5;

```

Under the hood, JavaScript actually interprets this code as:

```bash 
var x;
console.log(x); // undefined
x = 5;

```

This behavior of moving variable declarations to the top is what is referred to as hoisting. However, it's important to note that only the declarations are hoisted, not the initializations or assignments. So while variable and function declarations are hoisted, assignments and initializations remain where they are in the code.

Hoisting can sometimes lead to unexpected behavior if not understood properly, so it's important for JavaScript developers to be aware of how it works in order to write predictable and maintainable code.