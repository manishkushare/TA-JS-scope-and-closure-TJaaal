Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.

- Take in account the different phases of execution, different execution contexts

1.

```js
var species = 'human';

function change() {
  var species = 'vampire';
  console.log(species);
}

console.log(species); // 1 human
change();
console.log(species); // 2 human
```

<!-- Put your image below -->

![](./img/IMG_20210316_161804.jpg)

- Create the execution context diagram
- What will be the value of species on 1 and 2

2.

```js
var topLevelVar = 'This is global scope!';

function topLevelFn() {
  var localVar = "This is local to topLevelFn's scope";

  function nestedFn() {
    var anotherLocalVar = "Local to nestedFn's scope.";

    console.log(localVar); // 1  This is local to topLevelFn's scope
    console.log(topLevelVar); // 2 This is global scope!'
  }

  nestedFn();
}

topLevelFn();
```

<!-- Put your image below -->

![](./img/IMG_20210316_161811.jpg)

- Create the execution context diagram
- What will be the value of 1 and 2

3.

```js
var one = 'One';
var two = 'Two';

function main() {
  var three = 'Three';

  function inner() {
    var four = 'Four';

    console.log(one); // 1 one
    console.log(two); // 2 two
    console.log(three); // 3 three
  }
  console.log(four); // 4  error reference error , four is not defined
  inner();
}

main();
console.log(one, two, three, four); //  one,two,reference error, reference error
```

<!-- Put your image below -->

![](./img/IMG_20210316_161834.jpg)

- Create the execution context diagram
- What will be the value of 1, 2, 3, 4 and 5 or error if the code does not work
