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

## How does TypeScript help in improving code quality and project maintainability?
