1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let getPercentage = function (marks, total) {
  return (marks * 100) / total;
}
// arrow function
let getPercentage = (marks, total) => {
  return (marks * 100) / total;
}
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
// function declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
// function expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
// annonymous function expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
// arrow function
```

```js
let percentage = (marks, total) => (marks * 100) / total;
// arrow function without paranthesis
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
<!-- as we know that, function is an object in Javascript. And object is a value in JS. So, we can have a expression to the RHS of the assignment operator. Hence, function expression exist in JS.  -->
4. Why is a function call an expression in JavaScript?
<!-- because, function call will evaluate the code and return the value  -->
5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer 5
five = add; // Answer function reference
five = five(10, 11); // Answer 21
five = function () {
  return 'Hello';
}; // Answer function expression
```

6. What is the difference between function definition and function call? Explain with an example.
<!-- function defination is way of writing a function, where we give inputs to get the desired outputs whenever it gets called in the future.
Whereas, function call executes the function and returns the expression
 -->
7. What is the similarities between function definition and function call?
<!-- funtion is the procedure to achieve particular task whereas function call is using the same fynction to achievev the task result -->
8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid - since function is an object, we can add the user property with value "sam"

```

9. What is higher order function explain with an example.
<!-- Thumb rule to identify higher order function is:
1. whether the function is accepting the function refrence/defination as the arguments 
2. whether function returns function refrence not an function call
let numbers = [1,2,3,4,5,6,7,8,9];
let isEven = (n) => n%2 == 0;
let isOdd = (n) => n%2 !==0;
function seperateEvenOdd(numbers,odd,even){
    let evenArray = [];
    let oddArray = [];
    for(let num of numbers){
        if(odd(num)){
            oddArray.push(num);
        }
        else if(even(num)){
            evenArray.push(num);
        }
    }
    return [evenArray,oddArray];
}
seperateEvenOdd(numbers,isOdd,isEven);
here :
1. seperateOddEven is Higher order function
2. whereas isOdd, isEven is callback function
-->


10. Explain what is callback function. Why you can pass a function inside a function?
<!-- since function is an object and object is data type in JavaScript. Hence function is nothing but evaluated expression at the end. we can pass expression as a arguments inside the function. Hence we can pass function inside a function 

When a function reference is passsed as an argument to the Higher order function, keeping in mind that those function references may be called later in the future , if needed. Those refrences are called callback functions-->