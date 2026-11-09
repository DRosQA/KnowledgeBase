Access to functions and attributes can be limited in some programming languages. What keywords are available differs by language.

## Csharp

| Caller's location                      | `public` | `protected internal` | `protected` | `internal` | `private protected` | `private` |
| -------------------------------------- | -------- | -------------------- | ----------- | ---------- | ------------------- | --------- |
| Within the class                       | ✔️️      | ✔️                   | ✔️          | ✔️         | ✔️                  | ✔️        |
| Derived class (same assembly)          | ✔️       | ✔️                   | ✔️          | ✔️         | ✔️                  | ❌         |
| Non-derived class (same assembly)      | ✔️       | ✔️                   | ❌           | ✔️         | ❌                   | ❌         |
| Derived class (different assembly)     | ✔️       | ✔️                   | ✔️          | ❌          | ❌                   | ❌         |
| Non-derived class (different assembly) | ✔️       | ❌                    | ❌           | ❌          | ❌                   | ❌         |
## Java
| Modifier    | Description                                                                                      |
| ----------- | ------------------------------------------------------------------------------------------------ |
| `public`    | The code is accessible for all classes                                                           |
| `private`   | The code is only accessible within the declared class                                            |
| _default_   | The code is only accessible in the same package. This is used when you don't specify a modifier. |
| `protected` | The code is accessible in the same package and **subclasses**.                                   |
## Python
Convention only, no language-side enforcement.

| Modifier    | Prefix | Access              |
| ----------- | ------ | ------------------- |
| `public`    |        | everywhere          |
| `protected` | `_`      | self and subclasses |
| `private`   | `__`     | self only           |
