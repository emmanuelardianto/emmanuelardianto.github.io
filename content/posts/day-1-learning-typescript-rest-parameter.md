---
title: 'Day 1 Learning Typescript Rest Parameter'
date: '2025-08-12T12:00:00+09:00'
tags:
- typescript
- udemy
---

### Rest Parameter
rest parameter (…args) allows a function to accept an indefinite number of arguments as an array.

```
const add = (...numbers: number[]) => {
  return numbers.reduce((curResult, curValue) => {
    return curResult + curValue;
  }, 0);
};

const addedNumbers = add(5, 10, 2, 3.7);
```