# Boolean Logic Exercises

## **Part I**

Write down what the following statements will return. Try to figure this out before putting the commands in the chrome console.

1. ***2 == “2”;***
    - `true`
2. ***2 === 2;***
    - `true`
3. ***10 % 3;***
    - `1`
4. ***10 % 3 === 1;***
    - `true`
5. ***true && false;***
    - `false`
6. ***false || true;***
    - `true`
7. ***true || false;***
    - `true`

## **Part II**

Answer the following questions about this code block:

```jsx
let isLearning = true;
if(isLearning){
  console.log("Keep it up!");
} else {
  console.log("Pretty sure you are learning....");
}
```

1. What should the above code console.log?
    - `console.log` will output "Keep it up!" because `isLearning` is truthy.
2. Why do we not need to specify ***if(isLearning === true)***? Why does ***if(isLearning)*** work on its own?
    - `true` is truthy and is what if statements check for.

```jsx
let firstVariable;
let secondVariable = "";
let thirdVariable = 1;
let secretMessage = "Shh!";

if(firstVariable){
  console.log("first");
} else if(firstVariable || secondVariable){
  console.log("second");
} else if(firstVariable || thirdVariable){
  console.log("third");
} else {
  console.log("fourth");
}
```

1. What should the above code console.log? **Why?**
    - `third`
    - `firstVariable` is falsey and is skipped, `secondVariable` is also falsey and the first `else if` is skipped. `thirdVariable` is truthy, so "third" is printed. The else is skipped because the condition was met.
2. What is the value of ***firstVariable*** when it is initialized?
    - `undefined`

3. Is the value of firstVariable a “truthy” value? **Why?**
    - No, it is falsey. `firstVariable` is `undefined`
4. Is the value of secondVariable a “truthy” value? **Why?**
    - No, it is falsey. Empty strings are falsey.
5. Is the value of thirdVariable a “truthy” value? **Why?**
    - Yes, it is. Any number except `0` is truthy.

## **Part III**

1. Research  [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random)
    
    ***Math.random***
    
    Write an if statement that console.log’s “Over 0.5” if ***Math.random*** returns a number greater than 0.5.
    
    Otherwise console.log “Under 0.5”.

    ```js
    let rand = Math.random();
    if (rand > 0.5) {
        console.log("Over 0.5");
    } else {
        console.log("Under 0.5");
    }
    ```
    
2. What is a falsey value? List all the falsey values in JavaScript.
    - A falsey value is a value that is `false` in a conditional statement.
    - `undefined`, `null`, `0`, `""` (any empty string), `NaN`, and `false`. 