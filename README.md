# Boolean Logic Exercises

## **Part I**

Write down what the following statements will return. Try to figure this out before putting the commands in the chrome console.

1. ***2 == “2”;***
2. ***2 === 2;***
3. ***10 % 3;***
4. ***10 % 3 === 1;***
5. ***true && false;***
6. ***false || true;***
7. ***true || false;***

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
2. Why do we not need to specify ***if(isLearning === true)***? Why does ***if(isLearning)*** work on its own?

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
2. What is the value of ***firstVariable*** when it is initialized?
3. Is the value of firstVariable a “truthy” value? **Why?**
4. Is the value of secondVariable a “truthy” value? **Why?**
5. Is the value of thirdVariable a “truthy” value? **Why?**

## **Part III**

1. Research  [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random)
    
    ***Math.random***
    
    Write an if statement that console.log’s “Over 0.5” if ***Math.random*** returns a number greater than 0.5.
    
    Otherwise console.log “Under 0.5”.
    
2. What is a falsey value? List all the falsey values in JavaScript.