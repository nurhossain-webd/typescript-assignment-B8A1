Understanding Type Narrowing in TypeScript

In TypeScript, a variable can sometimes contain more than one type of value. This usually happens when we use union types. For example, a variable might contain either a string or a number. Before using methods that belong to a specific type, we need to check what kind of value we are working with. This process is called type narrowing.

One common way to narrow types is by using the typeof operator. It helps us identify primitive types such as strings, numbers, and booleans.

```typescript
function formatValue(value: string | number): string {
  if (typeof value === "string") {
    return value.toUpperCase();
  }

  return value.toFixed(2);
}
```

Here, TypeScript understands that the value is a string inside the if block. Otherwise, it treats the value as a number, allowing us to use number-specific methods safely.

Another useful operator is instanceof. It checks whether an object is an instance of a particular class or constructor.

```typescript
function handleError(error: Error | string): string {
  if (error instanceof Error) {
    return error.message;
  }

  return error;
}
```

This is helpful when handling errors because an error might be an Error object or a simple string.

We can also use the in operator to check whether an object contains a particular property.

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

In this example, TypeScript identifies the object type based on the available method.

Type narrowing makes working with union types easier and safer. By checking values before using them, we can reduce type-related errors and write more reliable TypeScript applications.
