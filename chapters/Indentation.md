[Back to Contents](https://github.com/OIL-language/OIL-style-guide/blob/main/README.md)
# 2. Indentation

You should use four spaces for indentation, as opposed to a tab:
```rust
import std.io.File;

fn main() {
/*
xxxx
*/
    File.stdout -> File.writeln "Hello world!";
}
```

Our language uses "egyptian curly braces" that are on the same line as the previous:
```rust
fn max(x: int, y: int): int = {
    if x > y {
        x
    } else {
        y
    }
};
```

You can ignore the outer braces in functions if the function is pure:
```rust
fn max(x: int, y: int): int = if x > y { x } else { y };
```

But this becomes problematic when you want to add side effects, so should probably be avoided most of the time.

`else` and `ifelse` statments are placed on the same line as the end bracket of the last statement as so:

```rust
if x < 10 {
    x++
} ifelse x = 10 {
    std.print("X is 10!");
} else {
    x--;
}
```
