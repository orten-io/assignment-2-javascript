# JavaScript tasks

Below you'll find a few JavaScript tasks. For each task, you need to create a new CodePen and save it (but create them as you go).
  You'll find some code for some of the tasks, just paste that in to the CodePen you create and then follow the instructions to solve it.

## 1. Find the error

The code below is a solution of the counter we created during the "JavaScript from scratch" talk. However it contains a couple of errors,
  it is your task to resolve them and get the counter to work as expected. (You should have a plus button, a minus button, and a 0 in the
  HTML. When you click on the plus button the number should increment to 1, when you click it again it should increment to 2 and so on.
  And same for the minus button - the number should decrement to 1, then 0, -1 etc when you click on it)

HTML:

```html
<button id="minus">-</button>
<span id="number>0</span>
<div id="plus">+</div>
```

JavaScript:

```js
var counter = 0;

document.getElementById(minus').onclick = function () (
  document.getElementById('counter').innerHTML = counter = counter - 1;
  counter = counter - 1;
);

document.getElementById('plus').onclick = function () {
  counter = counter + 1;
  document.getElementById('number').innerHTML = counter;
}
```

## 2. Ordered arrays

Create an input where the user can input things they like. When the user adds an item, add it to an array and use
  [`.sort()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort) to sort it
  alphabetically. Then use `.join(' and ')` to `console.log` a message like `"You like: Thing A and thing B and thing C"`
  and so on every time they add an item.

## 3. Car and speed limits

Create an object called `car` that has the properties `brand` and `maxSpeed`. It should also have the property `gas`, which
  should be a function that takes the parameter `speed`. That function should `console.log` the message "Broom, a `<brand>` moving forward
  at `<speed>` kmph". However, a car can't move faster than it's maxSpeed, so check `if (speed > maxSpeed) {` ("if speed is more than maxSpeed").
  If that's the case, `console.log` "Sorry, a `<brand>` cant go that fast" instead. You can access `maxSpeed` and `brand` by using
  `this.maxSpeed` and `this.brand` inside the `gas` function.

Here's some help on the way:

```js
// The function below should be assigned to the property "gas" on the "car" object
function(speed) {
  if (speed > this.maxSpeed) { // `this.maxSpeed` will give you the car's maxSpeed
    console.log('Sorry, a ' + this.brand + 'can\'t go that fast'); // `this.brand` will give you the car's brand
  }
```

## 4. Text length

Create an input where the user can enter any text. Then, when the user changes the text, show a text inside a `<div>` that
  says "The text you entered is `text.length` long". Also, if the text is more that 10 characters long, make it red.

Here is a snippet to help you out:

```js
document.getElementById('your-id').onchange = function () { // .onchange runs the function every time the user types something in the input
  var text = /* something that reads the user's input text */;
  if (text.length > 10) {
    // make the text red here
  } else {
    // make the text not red
  }
}
```
