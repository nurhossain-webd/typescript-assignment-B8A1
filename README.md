TypeScript Problem Solving Assignment

This repository contains solutions for the TypeScript Problem Solving and OOP assignment.

All eight coding problems are solved in a single file named solutions.ts.

The assignment covers the following topics:

1. Optional and default parameters
2. Union types and type narrowing
3. Readonly tuples
4. Generics and rest parameters
5. Interfaces and array filtering
6. Generics with keyof constraints
7. Classes, inheritance, and access modifiers
8. Asynchronous programming with Promises

Two blog posts are also included:

1. type-vs-interface.md - Explains the differences between type aliases and interfaces in TypeScript and when to use them.

2. type-narrowing.md - Explains type narrowing with practical examples using typeof, instanceof, and the in operator.

Technologies Used:

TypeScript
Node.js

How to Run:

First, make sure Node.js and TypeScript are installed.

Install TypeScript:

npm install -g typescript

Check the TypeScript version:

tsc --version

Compile the TypeScript file:

tsc solutions.ts --target ES2020 --lib ES2020,DOM

After successful compilation, a solutions.js file will be generated.

The functions return their results directly. No console.log statements or sample test calls are included in the solutions file.

Project Structure:

typescript-assignment/
solutions.ts
type-vs-interface.md
type-narrowing.md
README.md

This assignment focuses on practicing TypeScript fundamentals, writing reusable functions, applying object-oriented programming concepts, and handling asynchronous operations with Promises.
