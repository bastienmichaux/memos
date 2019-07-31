# TS

"primitives"

```typescript
const x: undefined = undefined;
const x: null = null;
const x: boolean = false;
const x: number = 0;
const x: string = '';

function impure (): void {}

// ok cause null & undefined are subtypes of all primitives
const x: number; // is actually undefined
const x; // type: any; value: undefined;

// when a function has an unreachable end point
function throwError (): never {}
```

arrays

```typescript
const x: number[] = [1,2,3];

// avoid this cause React
const x: Array<number> = [1,2,3];

// "immutable" array
const x: ReadonlyArray<number> = [1,2,3];

// from immutable array to normal array
const y = x as number[];
```

enum

```typescript
enum Color {Red, Green, Blue};
const c: Color = Color.Green;

// string enum, useful for debugging
enum Color {Red='Red', Green='Green', Blue='Blue'};
```

interface

```typescript
// use interface without declaring one
function x (p: {myProp: string}) {}

// interface declaration
interface x {
  label: string;
  optionalProperty?: string;
  readonly x: number; // mutable only when object is created
  [excessProperty: string]: any; // excess property, useful when converting js
}

// function call signature
interface addInterface {
  (num1: number, num2: number): number;
}

const add: addInterface = function (num1: number, num2: number): number {}

// class interface
interface ClockInterface {
  currentTime: Date;
  setTime(d: Date): void;
}
// implementation
class Clock implements ClockInterface {
  currentTime: Date = new Date();
  setTime(d: Date): void {
    this.currentTime = d;
  }
  constructor(h: number, m: number) { }
}
```

generics

```typescript
function x<T>(arg: T): T {
  return arg.length; // Error: T doesn't have .length
}

function x<T>(arg: T[]): T {
  return arg.length; // ok
}
```
