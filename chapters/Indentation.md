[Back to Contents](https://github.com/OIL-language/OIL-style-guide/blob/main/README.md)
# 1. Indentation

Try to use four spaces for a tab as in this example

```rust
import stdout;

fn main(): void {
    stdout.println("Hello world!");
}
```

Curly braces should be placed like this:
```rust
fn add(x:int, y:int): int {
    z = x + y;
    return z;
}
```
or like this:
```rust
fn add(x:int, y;int): int { z = x + y; return z; }
```
When doing the latter try to keep spaces between the curly brackets and the contents;

## Examples

this is good:
```rust
fn timesByTwo(x:int): int { z = x * 2; return z; }
```
this is not good:
```rust
fn timesByTwo(x:int): int {z = x * 2;return z;]
```
