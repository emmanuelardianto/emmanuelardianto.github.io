---
date: '2025-08-13T11:40:56+09:00'
title: 'Day 2 Learning Typescript -  Object Destructuring'
categories:
- development
tags:
- typescript
- udemy
---

Object destructuring allows the extraction of properties from an object.

```
const person = {
    firstName: 'Maxxx',
    age: 30
};

const { firstName: userName, age } = person;

console.log(userName, age, person);

//firstName: userName -> initialize userName variable with firstName of person value
```