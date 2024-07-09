# Simple Practice Language (SPL)

SPL is a minimalistic programming language designed for practice and learning purposes. It aims to provide a straightforward syntax and basic programming constructs, making it easy to understand and implement.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Language Syntax](#language-syntax)
- [Example Code](#example-code)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Variables:** Support for integer (`int`) type.
- **Functions:** Define and call functions with parameters and return values.
- **Control Flow:** Conditional statements (`if-else`) and loops (`while`).
- **Input/Output:** Basic input and output operations.
- **Comments:** Single-line (`//`) comments supported.
- **New Keywords:** Introduced `box` for variable declaration and `back` for return statement.

## Installation

1. Ensure you have [Rust](https://www.rust-lang.org/tools/install) installed.
2. Clone this repository:
    ```sh
    git clone https://github.com/yourusername/rust-interpreter-compiler.git
    ```
3. Navigate to the project directory:
    ```sh
    cd rust-interpreter-compiler
    cd spl-interpreter
    ```
4. Build the project:
    ```sh
    cargo build --release
    ```

## Usage

To run the interpreter with one or more example scripts, use the following command:

```sh
./target/release/interpreter file1.spl file2.spl ...
```

## Language Syntax

The custom language includes the following syntax elements:

- **Function Definition:** Defined using the `fn` keyword.
    ```plaintext
    fn function_name(parameters) {
        // function body
    }
    ```
    Example:
    ```plaintext
    fn my_biggest(a, b) {
        if (a > b) {
            back a;
        }
        back b;
    }
    ```

- **Conditional Statements:** Using `if` for condition checks.
    ```plaintext
    if (condition) {
        // code if condition is true
    }
    ```
    Example:
    ```plaintext
    if (a > b) {
        back a;
    }
    ```

- **Variable Declarations:** Using the `box` keyword for declaring variables.
    ```plaintext
    box variable_name = value;
    ```
    Example:
    ```plaintext
    box x = 10;
    box y = 20;
    ```

- **Return Statements:** Using the `back` keyword to return values from functions.
    ```plaintext
    back value;
    ```
    Example:
    ```plaintext
    back a;
    ```

- **Print Statements:** Using `print` to output text to the console.
    ```plaintext
    print("text" + variable);
    ```
    Example:
    ```plaintext
    print("The biggest number is " + result);
    ```

## Example Code

Here is an example of a script written in the custom language:

```plaintext
// Simple practice language example with new keywords

fn my_biggest(a, b) {
    if (a > b) {
        back a;
    }
    back b;
}

fn main() {
    box x = 10;
    box y = 20;
    box result = my_biggest(x, y);
    print("The biggest number is " + result);
}
```

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, feel free to create a pull request or open an issue.

1. **Fork the repository.**
2. **Create a new branch** with your feature or fix:
    ```sh
    git checkout -b feature-branch
    ```
3. **Commit your changes**:
    ```sh
    git commit -m "Description of the changes"
    ```
4. **Push the branch** to your forked repository:
    ```sh
    git push origin feature-branch
    ```
5. **Create a pull request**.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

  
