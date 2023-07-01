[Back to Contents](https://github.com/OIL-language/OIL-style-guide/blob/main/README.md)
# 1. Cases

We use the common style of PascalCase for types, and snake_case for function names:
```rust
import std.io.File;

type TypeName { x: Int; };

fn snake_case_function_name(): TypeName = {
    File.stdout -> File.write "Whatever";
    TypeName {
        x: 10;
    };
};
```
