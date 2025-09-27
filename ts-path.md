# TypeScript Learning Roadmap

This roadmap is designed for someone with a solid JavaScript foundation, focusing on TypeScript-specific features to reach an intermediate level. It covers essential and commonly used concepts in development, with practical steps to apply them. Aim to spend 1-2 weeks per phase, using tools like the TypeScript Playground, VS Code, and the official documentation (typescriptlang.org/docs).

## Phase 1: Essentials (1-2 Weeks)
Master the core type system and setup to add type safety to your JavaScript code.

### 1. Setup and Basics
- Install TypeScript: `npm install -g typescript`.
- Learn `tsc` commands and configure `tsconfig.json` (`strict`, `target`, `module`).
- Understand type inference (TS guesses types from JS).
- **Practice**: Convert a simple JS script to TS and compile it.

### 2. Primitive and Basic Types
- Core types: `number`, `string`, `boolean`, `null`, `undefined`, `symbol`, `bigint`.
- Arrays (`string[]` or `Array<string>`) and tuples (`[string, number]`).
- Special types: `any` (avoid overuse), `unknown`, `void`, `never`.
- **Practice**: Type variables and function parameters in a utility script.

### 3. Objects and Interfaces
- Define object shapes: `interface User { name: string; age: number; }`.
- Use optional properties (`?`), `readonly`, and index signatures (`[key: string]: number`).
- Type aliases vs. interfaces (aliases for unions, interfaces for extendable shapes).
- **Practice**: Model API responses or configs.

### 4. Functions
- Type parameters, return types, optional/default parameters.
- Function types and overloads for multiple signatures.
- Arrow functions and `this` in classes.
- **Practice**: Write typed utility functions (e.g., string formatter, array sorter).

### 5. Classes and OOP
- Classes with typed properties, constructors, methods.
- Access modifiers: `public`, `private`, `protected`.
- Inheritance (`extends`, `super`) and implementing interfaces.
- **Practice**: Build a class hierarchy (e.g., Shape -> Circle).

### 6. Modules and Namespaces
- Use ES modules (`import/export`) with type declarations.
- Organize code with namespaces in larger files.
- Create `.d.ts` files for external JS libraries.
- **Practice**: Split code into modules and import types.

## Phase 2: Intermediate (2-3 Weeks)
Learn advanced type manipulation and patterns used in production (e.g., web apps, APIs).

### 1. Union and Intersection Types
- Unions: `string | number` for flexible typing.
- Intersections: `TypeA & TypeB` to combine types.
- Literal types: `type Direction = 'up' | 'down';`.
- **Practice**: Handle API responses with success/error objects.

### 2. Generics
- Generic functions/classes: `function identity<T>(arg: T): T`.
- Constraints: `T extends SomeType`.
- Generic interfaces and default types.
- **Practice**: Build a generic stack or fetch function.

### 3. Type Guards and Narrowing
- Use `typeof`, `instanceof`, `in` for built-in guards.
- Create user-defined guards (`arg is Type`).
- Use discriminated unions for tagged types.
- **Practice**: Safely process mixed-type arrays or optional props.

### 4. Advanced Types
- Conditional types: `T extends U ? X : Y`.
- Mapped types: `Readonly<T>`, `Partial<T>`.
- Utility types: `Pick`, `Omit`, `Record`.
- **Practice**: Create reusable type transformations for configs.

### 5. Decorators
- Apply decorators to classes, methods, properties (enable `--experimentalDecorators`).
- Use for logging, validation, or dependency injection.
- **Practice**: Add a logging decorator to class methods.

### 6. Integration and Best Practices
- Use `@types` packages (e.g., `npm install @types/node`).
- Mix JS/TS with `allowJs` for gradual adoption.
- Handle errors with custom types and assertions (`as`).
- Avoid `any`, enable strict null checks.
- Test with Jest/Vitest (`ts-jest`).
- **Practice**: Set up a Node.js or React project with TS and ESLint.

## Next Steps
- **Projects**: Build a CLI tool, Express API, or React app with TS.
- **Resources**:
  - TypeScript Handbook: typescriptlang.org/docs/handbook
  - TypeScript Deep Dive: basarat.gitbook.io/typescript
  - Courses: freeCodeCamp, egghead.io
  - Community: Stack Overflow, r/typescript, TypeScript GitHub
- **Tools**: Use VS Code IntelliSense, TS Playground.
- **Goal**: Refactor JS to TS, debug type errors, and use generics/guards confidently.
