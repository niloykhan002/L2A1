# What are some differences between interfaces and types in TypeScript?

## Interface

- Best for defining object shapes
- Supports declaration merging
- Works well with classes using implements

## Type

- More flexible and powerful
- Can define unions, intersections, primitives, and tuples
- Cannot be merged or re-declared

## Basic Syntax

```ts
// Interface
interface User {
  name: string;
  age: number;
}

// Type
type User = {
  name: string;
  age: number;
};
```

## What is the use of the keyof keyword in TypeScript?

The keyof keyword in TypeScript is used to extract the keys of an object type as a union of string (or number) literal types.

```ts
type Person = {
  name: string;
  age: number;
  isActive: boolean;
};

type PersonKeys = keyof Person;

function getValue(obj: Person, key: keyof Person) {
  return obj[key];
}

const user: Person = { name: "Jhankar", age: 42, isActive: true };

getValue(user, "name"); // Output: Jhankar
```
