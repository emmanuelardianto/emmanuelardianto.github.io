---
date: '2025-08-18'
draft: false
title: 'Day 5 Learning Typescript - Type Intersection'
categories:
- development
tags:
- typescript
- udemy
- type
- interface
---


### Intersection Type
Combines multiple types into a single new type that possesses all the properties of each of the individual types. It is created using the & operator.

```
type FileData = {
    path: string;
    content: string
} 

type Status = {
    isOpen: boolean;
    errorMessage?: string;
}

type AccessFileData = FileData & Status;
```


### Function Overload
Function overloading in TypeScript allows a single function name to have multiple "signatures," meaning it can be called with different types or numbers of arguments, leading to different return types. This provides enhanced type safety and clarity for consumers of the function.

```
function getLength(val: any[]): Number;
function getLength(val: string): string;
function getLength(val: string | any[]) {
    if(typeof val === 'string') {
        const numberOfWords = val.split(' ').length;
        return `${numberOfWords} words`;
    }
    return val.length;
}
```