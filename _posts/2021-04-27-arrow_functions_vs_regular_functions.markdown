---
layout: post
title:      "Arrow Functions vs. Regular Functions"
date:       2021-04-27 22:55:40 +0000
permalink:  arrow_functions_vs_regular_functions
---


When I first started using arrow functions I simply thought it was just the more modern & concise way to write functions after ES6. Well - I was wrong. Here's why:

## Syntax

So I wasn't TOTALLY off base when I thought arrow functions were just syntactically "sweeter". Because they are. It's just not the only difference. Here's a visual difference between both ways of writing a function.

```
// Regular Function (ES5)

var add = function (a, b) {
    return a + b
}

// Arrow Function (ES6)

let add = (a, b) => a + b
```

## Using 'new'

Regular functions by nature are both **callable** & **constructible**. This means that you can use the **'new'** operator which allows you to invoke them into a new instance.

Arrow functions are NOT **constructible**. This means that the **'new'** operator isn't an option. Here's an example snippet & the error you'll receive.

```
let add = (a + b) => console.log(a + b);

new add(6, 12);
```

![](https://i.ibb.co/TPrVjJM/arrow-function-new-keyword.png)

## Non-Binding 'this'

This is (in my opinion) the big difference between the two. 

Unlike regular functions - arrow functions **DO NOT** have their own **'this'**. So when **'this'** is used within an arrow function it wouldn't have the same value as using **'this**' within a regular function. This is because **'this'** within an arrow function is lexically bound (goes up a scope). 

This is something that I needed to see to understand. So lets look at an example:

![](https://i.ibb.co/fNBdyZY/arrow-function-this.png)

Notice how

## Final Thoughts

Arrow functions are definitely more 'fun' to write because well..they're usually more concise. But make no mistake - they don't replace regular functions. Both have their purpose & it's up to us to decide when we need each of them.
