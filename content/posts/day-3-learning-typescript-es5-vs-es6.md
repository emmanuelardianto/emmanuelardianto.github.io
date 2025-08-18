---
date: '2025-08-14T11:42:38+09:00'
title: 'Day 3 Learning Typescript Es5 vs Es6'
categories:
- development
tags:
- typescript
- udemy
---

Essentially, all TypeScript code will be compiled into JavaScript. The compiler can be set to ES5 or ES6. ES5 is an older JavaScript syntax. The contrast differences are:

1. ES5 is primarily used var for variable declaration. ES6 using let or const.

2. When creating a class, ES5 uses prototyping. ES6 introduced class keyword.

3. ES6 supports arrow functions.

4. ES5 using callback for asynchronous, ES6 using promises.

```
class User {
    constructor(public name: string, public age: number) {}

    greet() {
        console.log('hello my name is ' + this.name);
    }
}
```

```Private``` and ```public``` keywords are exclusive to Typescript. It can’t be implemented in JavaScript.