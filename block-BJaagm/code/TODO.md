1. What does thread of execution means in JavaScript?
Thread of execution measns , how code is executed in JS. JS is single threaded, that means only one line of code is executed at a time.

2. Where the JavaScript code gets executed?
% Javascript code is executed inside global execution context.
% Whenever any code runs, it first creates a global execution context only once.
% Global execution context have two colums, out of which one is memory, it stores all the global data and function    reference.
% It scans all the line one by one and stores the data inside memory.
% Whenever any function is defined it is also gets stored in the memory of GEC as the reference
% We don't go inside the function umless it gets called. 
% once function is called, the function name gets pushed inside the call stack. call stack has global() function at the bottom
%execution context gets created of that particular function inside GEC and function gets executed. After completionof it, that exceution context gets deleted and result is stored inside the apppropriate 
 
3. What does context means in Global Execution Context?
Execution context (EC) is defined as the environment in which the JavaScript code is executed. By environment, I mean the value of this, variables, objects, and functions JavaScript code has access to at a particular time.

4. When do you create a global execution context.
Global execution context get created only once at the beginning
5. Execution context consists of what all things?
Execution context cosnist of memeory and execution context
6. What are the different types of execution context?
Two diffrent types of excution context are there:
% Global execution context - whenever scipt loads the first file on browser, Global execution context gets created only once at the beginning. Global execution context is present at the bottom of the call stack. Once, script is ended, global execution contect gets poped up
% function execution context - whenever the function call is seen, the JS engine creates the function execution context and pushes the execution context onto stack. Whenever the function excution gets over, the value is
-7. When global and function execution context gets created?
global execution context is created in the beginning itself , only once, when first file is loaded in the browser.
whereas function execution context is the execution context created , when function call is seen.
8. Function execution gets created during function execution or while declaring a function.
Function executio context is created during function execution

9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.
```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user); 
<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
 -. return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)