Understanding Type Narrowing in TypeScript

Introduction

In TypeScript, a variable can sometimes hold different types of values. This usually happens when we use union types. Before performing an operation, we need to know the actual type of the value. Type narrowing helps TypeScript identify the correct type based on certain conditions.

Type Narrowing with typeof

The typeof operator checks the type of a value at runtime. It is commonly used with strings, numbers, and booleans.

```typescript
function formatValue(value: string | number): string {
  if (typeof value === "string") {
    return value.toUpperCase();
  }

  return value.toFixed(2);
}
```

Here, TypeScript understands that value is a string inside the if block. Otherwise, it treats the value as a number. This helps prevent type-related errors.

Type Narrowing with instanceof

The instanceof operator checks whether an object belongs to a particular class or constructor.

```typescript
function handleError(error: Error | string): string {
  if (error instanceof Error) {
    return error.message;
  }

  return error;
}
```

This is useful when handling errors because we can safely access the message property of an Error object.

Type Narrowing with the in Operator

The in operator checks whether a specific property exists in an object.

```typescript
interface Car {
  drive(): void;
}

interface Boat {
  sail(): void;
}

function startVehicle(vehicle: Car | Boat): void {
  if ("drive" in vehicle) {
    vehicle.drive();
  } else {
    vehicle.sail();
  }
}
```

In this example, TypeScript checks whether the object has a drive method. Based on that condition, it allows us to call the appropriate method.

Conclusion

Type narrowing is an important feature of TypeScript because it makes working with different data types safer. By using typeof, instanceof, and the in operator, we can avoid common mistakes and write more reliable code.
