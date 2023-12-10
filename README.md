# Typescript Labs

## Lab 13: Typing Errors in a Try-Catch

file: `/src/13-catch-blocks.problem.ts`

Take a look at this try-catch demo:

```ts
const tryCatchDemo = (state: "fail" | "succeed") => {
  try {
    if (state === "fail") {
      throw new Error("Failure!");
    }
  } catch (e) {
    return e.message;
  }
};
```

TypeScript is giving us an error on `e.message` that the object is of type `unknown`.

Challenge
Your challenge is to coerce the `unknown` type into one where we know what it is.

Hint: there are a few ways to solve this challenge-- see what you can come up with!