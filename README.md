# Simple Practice Language (SPL)

SPL is a minimalistic programming language designed for practice and learning purposes. It aims to provide a straightforward syntax and basic programming constructs, making it easy to understand and implement.

## Features

- **Variables:** Support for integer (`int`) and boolean (`bool`) types.
- **Functions:** Define and call functions with parameters and return values.
- **Control Flow:** Conditional statements (`if-else`) and loops (`while`).
- **Input/Output:** Basic input and output operations.
- **Comments:** Single-line (`//`) and multi-line (`/* */`) comments supported.
- **Constants:** Declare constants using `const`.
- **New Keywords:** Introduced `box` for variable declaration and `back` for return statement.

## Example

Here’s an updated example program in SPL with the new keywords:

```rust
// Simple practice language example with new keywords

fn main() {
    box x = 10;
    box y = 20;
    box result = add(x, y);
    print(result);
}

fn add(a: int, b: int) -> int {
    back a + b;
}

fn print(value: int) {
    // Print function for outputting the value
    // For simplicity, we'll just print to console
    println("Result is: ", value);
}```

## Getting Started

To run programs written in SPL:

1. **Setup:**
   - Ensure you have Rust installed on your system. If not, download and install Rust from [rust-lang.org](https://www.rust-lang.org/).

2. **Clone Repository:**
   ```bash
   git clone <repository-url>
   cd spl-interpreter```

3.
