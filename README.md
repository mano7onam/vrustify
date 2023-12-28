# Vrustify

Vrustify is a small but powerful library for data validation in Rust.

It provides validation functions for:

* Email addresses
* URLs
* Phone numbers
* Passwords

## Installation

You can include `Vrustify` library to your project, by adding following to your `Cargo.toml`:

```toml
[dependencies]
Vrustify = "0.1.0"
```

And then do a cargo build:

```bash
cargo build
```

## Usage

First, include the `Vrustify` in your Rust file:

```rust
extern crate Vrustify;
```

Then you can use the validation functions in your code as follows:

For email validation:

```rust
if Vrustify::email::validate("example@example.com") {
    println!("Valid email!");
} else {
    println!("Invalid email.");
}
```

For URL validation:

```rust
if Vrustify::url::validate("https://example.com") {
    println!("Valid URL!");
} else {
    println!("Invalid URL.");
}
```

And alike for other types of validation.

## License

`Vrustify` is distributed under the MIT license. See `LICENSE` file for additional information.

