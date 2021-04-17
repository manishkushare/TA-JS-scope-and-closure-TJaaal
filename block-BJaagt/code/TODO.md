Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); // output
```
In the above code, we are calling a variable "username" in the global scope, which is defined inside the block scope with the help of keyword "const".
Now, const is function as well as block scoped. Means, whenever we define a variable with keyword const inside a block scope ort function scope , it creates it's scope or in laymen term its private room. Now, username, is accessible inside the block scope itself.

Since we are trying to access the username from global scope, first will see, do we have a variable named username defined inside the global scope, if yes, bingo! will get result, if no will look for it to it's parent.

Means, we can bubble out to the parent, but, we can't bubble in inside the scope.

Output - username is not defined


3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(useranme); // output
```
username is defined inside the block scope, with the keyword "let". So, it create it's scope and restrict it's access upto that particular scope itself.

Now, we are trying to access the username from global scope, by bubbling in the block scope, which is not allowed.

output - username is not defined 

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); // output
```
we have defined the variable "username " inside the block scope, using the keyword "var".
Now, unlike let and const, variable declared by var is only function scoped.
That means , even though variable is defined insdie block scope using var, it will not create it's scope and can be accessed from the global scope.

hence, variable suername is accessible from global scope

output - "Arya"
5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); // output

```
error - username has already declared

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // output
```
"John"

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(useranme); // output
```
output - "John"
8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```
output - 
0 First
1 First
2 First
3 First
4 First
5 First
6 First
7 First
8 First
9 First

1 Second
2 Second
0 Second
3 Second
4 Second
5 Second
6 Second
7 Second
8 Second
9 Second


9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```
0 First
1 First
2 First
3 First
4 First
5 First
6 First
7 First
8 First
9 First

i is not defined