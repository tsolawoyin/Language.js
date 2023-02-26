# Expressions

Before we dive into *expressions* in the context of programming, let us briefly take a tour to a more familiar concept. 

The English language has 26 alphabets. A-Z. Although these letters individually don't make much sense, they combine differently to form the variety of words we have today. Take for instance the word *girl*

**girl** is an expression that is formed by concatenating four alphabets => g + i + r + l, and girl is just a combination of alphabets, we could as well rearrange these alphabets to form new words e.g

- i + g + r + l = igrl
- g + l + i + r = glir
- l + g + i + r = lgir
- l + i + r + g = lirg

Mathematically, we can have 4! arrangements of the word girl, i.e 4 * 3 * 2 * 1 = 24 possible arrangements. But obviously, it's girl that seem to make sense to you the most, which *translates* or *evaluates* to *a female figure, a young female precisely.* The word *girl* can be said to be a variable that points to a certain value in your brain (whichever way the word *girl* translates to you). In essence, it is not the word *girl* that matters, it is the meaning you give it. If a given word does not have a meaning to you, it is as good as useless. 

<!-- a picture of girl to girl image here -->

Other familiar words includes *government*, *bicycle*, *mountain*, *rain*, *sun*, *run*, *pretty*, and many more. You can actually find it easy to recognize these combinations of alphabets because they evaluate to some sort of real life object, as in the case of bicycle, mountain, rain, sun, or some abstract concept like pretty and government, or action like run. In summary,
<!-- a picture of the words and what they mean here -->
> We can define an ***expression*** as a phrase that can be evaluated to a particular value.

In JavaScript however, expressions is more concerned about the way the JS engine sees things. Take for instance
```javascript
let weird = %wjej38--fkii!3485
console.log(weird)
SyntaxError: Unexpected token '%'
←[90m    at internalCompileFunction (node:internal/vm:74:18)←[39m
←[90m    at wrapSafe (node:internal/modules/cjs/loader:1141:20)←[39m
←[90m    at Module._compile (node:internal/modules/cjs/loader:1182:27)←[39m
←[90m    at Module._extensions..js (node:internal/modules/cjs/loader:1272:10)←[39m
←[90m    at Module.load (node:internal/modules/cjs/loader:1081:32)←[39m
←[90m    at Module._load (node:internal/modules/cjs/loader:922:12)←[39m
←[90m    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:82:12)←[39m
←[90m    at node:internal/main/run_main_module:23:47←[39m

Node.js v19.2.0
```
You can easily see how the engine complained brutally that it doesn't recognize or understand the type of value you are trying to represent by throwing a **SyntaxError**.
<!-- a picture of a complaining person here -->
A high-level programming language like JavaScript allows you to write readable code, but also expects you to write what the computer can understand as well. The JS engine is the middle man (mediator) between you and the computer, and if the JS engine don't understand what you are trying to express, it's normal for it to complain.

In JavaScript, we have two major types of expressions

- Primary expressions
- Secondary expressions

> The simplest expressions, known as primary expressions, are those that standalone, they do not include any simpler subexpression. Primary expressions are constants or literal values, *certain* language keywords and variable references. <br> <br> JavaScript: The Definitive Guide

From the excerpt above, primary expressions are the most basic type of expressions in JavaScript, i.e, they cannot be subdivided into simpler expressions. Let's look at some example

```javascript
let string = "happiness";
let number = 34;
let isCool = true;

if(isCool) {
    return number + string;
}
```

Nevermind that we are adding a *number* object to a *string* object. In the simple program that we wrote, we have several primary expressions. The first obvious ones are the *constants* and *literals*. Can you identify the constant in this program? What about the literals? Hopefully you got it. *true* is a constant value in every javascript program, and it always evaluates to 1. When you type *true* in program, what the CPU sees is actually 1 and not the literal meaning of true. Where false evaluates to 0. Also, we have the literal values such as expression

<!-- I need to think straight to be able to write this to completion. I am trying to simplify things not confuscate them...I think I need to explain how types are pure objects in JavaScript... -->