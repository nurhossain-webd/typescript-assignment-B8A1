TypeScript Problem Solving Assignment

This repository contains my solutions for the TypeScript Problem Solving and OOP assignment. All eight coding problems are implemented in a single file named solutions.ts.

The assignment covers the following topics:

1. Optional and default parameters
2. Union types and type narrowing
3. Readonly tuples
4. Generics and rest parameters
5. Interfaces and array filtering
6. Generics with keyof constraints
7. Classes, inheritance, and access modifiers
8. Asynchronous programming with Promises

Blog Posts

I have also written two blog posts about important TypeScript concepts.

1. [Type Aliases vs Interfaces in TypeScript](./type-vs-interface.md)
2. [Understanding Type Narrowing in TypeScript](./type-narrowing.md)

Technologies Used

TypeScript
Node.js

How to Run

Make sure Node.js and TypeScript are installed.

Install TypeScript:

```
npm install -g typescript
```

Check the TypeScript version:

```
tsc --version
```

Compile the TypeScript file:

```
tsc solutions.ts --target ES2020 --lib ES2020,DOM
```

After successful compilation, a solutions.js file will be generated.

The functions return their results directly without console.log statements or sample test calls.

Project Structure

```
typescript-assignment/
    solutions.ts
    type-vs-interface.md
    type-narrowing.md
    README.md
```

This assignment helped me practice TypeScript fundamentals, reusable generic functions, object-oriented programming, and asynchronous operations using Promises.
