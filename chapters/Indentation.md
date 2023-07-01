[Back to Contents](https://github.com/OIL-language/OIL-style-guide/blob/main/README.md)
# 1. Indentation

You should prouse four spaces for indentation, as opposed to a tab:
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

You can ignore the outer braces in functions if the function is small and pure:
```rust
fn max(x: int, y: int): int = if x > y { x } else { y };
```

But this becomes problematic when you want to add side effects, so should probably be avoided most of the time.
