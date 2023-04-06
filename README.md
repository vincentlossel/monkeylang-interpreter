# MonkeyLang Interpreter

![Build](https://github.com/vincentlossel/monkeylang-interpreter/actions/workflows/build.yml/badge.svg?event=push)

Implementation of a [Monkey](https://monkeylang.org) interpreter, as described in [Writing an Interpreter in Go](https://interpreterbook.com).

## Features
- Integers, booleans, strings, arrays, hash maps
- Arithmetic expressions, let statements, recursions, closures
- First-class and higher-order functions
- Built-in functions
- REPL

## Syntax

```monkey
let people = [{"name": "Anna", "age": 24}, {"name": "Bob", "age": 99}];

let getName = fn(person) { person["name"]; };
getName(people[0]);

let fibonacci = fn(x) {
  if (x == 0) {
    0
  } else {
    if (x == 1) {
      return 1;
    } else {
      fibonacci(x - 1) + fibonacci(x - 2);
    }
  }
};
```
