# Quiz 2

1. One implication of values having different data types is that operators will behave differently depending on whether the data is numerical, string, array, etc.
2. 
        ```javascript

        console.log('My cat\'s kitty car has "Hello Kitty" on it!')

        // Also just use the template string back ticks instead of quotes
        console.log(`"My cat's kitty car has "Hello Kitty" on it!"`)

        ```
3. As mentioned in answer 1, we are using different data types. 3 and 5 can thus be added as numerical data, but because "8" is string, it is tacked on sequentially.
<!-- OK, it's concatenated as a string. -->

4. This is because a single equals sign is used as an assignment operator. Equality should be tested using a three-character equals sign.
<!-- And, variable names cannot start with a number. -->
5. 
        ```javascript

        var myMap = ["map","thousand","is","A","worth","a","pictures","."]
        console.log(myMap[3]);
        console.log(myMap[0]);
        console.log(myMap[2]);
        console.log(myMap[4]);
        console.log(myMap[5]);
        console.log(myMap[1]);
        console.log(myMap[6]);
        console.log(myMap[7]);


        var words = ["map","thousand","is","A","worth","a","pictures","."];
        // Example using a template string
        var sentence = `${words[3]} ${words[0]} ${words[2]} ${words[4]} ${words[5]} ${words[1]} ${words[6]}${words[7]}`;
        console.log(sentence);

        ```
6. 
        ```javascript

        var x = 20;
        var y = 40;
        if(x === y) 
        console.log("equal")
        else if(x > y) 
        console.log("x is greater than y")
        else if(x < y)
        console.log("x is less than y")

        ```

### Optional solution to if/else blocks

A JS shortcut you'll likely see is the use of the ternary operator, `?`

It takes three arguments:
```js
(condition) ? "if true do this" : "if not true, do this"
``` 

It's quite flexible. In the below example, we are assigning value to `myEval` 
based on comparing x to y. 
It's good to recognize this concise syntax.

```js
var x = 70
var y = 50

// Simple syntax
(x == y) ? console.log("same") : console.log("not same")

// Assign value based on comparison
var myEval = (x == y) ? "same"
  : (x > y) ? "x greater"
  : (y > x) ? "y greater"
  : "not same";
console.log(myEval)
```