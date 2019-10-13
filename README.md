# Short Input (S.I)
A simple CLI tool with short functions naming that asks for user input in meaningful way. Get your required rust input using short functions.

## Help

If you run into any issues or need help with using `si` in your project please email [uddinislam46@gmail.com](mailto:uddinislam46@gmail.com)

## Why you need it

When writing programs you will often need to take input from the user. User have to perform serveral things to get input ready with long names.

`si` attempts to make it easy to get input from the user without having to think about converting types or about long names.

## How to use

Add 
```toml
si = "0.1"
```
to your `cargo.toml` under `[dependencies]` and add
```rust
use si::input::*;
```
to your main file.

---

You can get input with.

```rust
input::as_i32()
```

Where `as_i32` is the type you want. This currently includes the standard library types `isize`, `usize`, `i8`, `u8`, `i16`, `u16`, `f32`, `i32`, `u32`, `f64`, `i64`, `u64`, `i128`, `u128`, and `String`.

For example, if you want to assign a valid unsigned 32bit value to a variable called `input`, you could write.

```rust
let input = input::as_u32();
```
