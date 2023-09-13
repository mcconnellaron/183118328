# Aron's Snek Language Compiler

**Overview:**

Aron's Snek Language Compiler is a Rust-based compiler designed to compile a LISP-like language, called Snek, into assembly code. This compiler was developed as part of a course on compilers and aims to provide a robust and efficient tool for translating Snek code into executable assembly.

**Features:**

- **Snek Language Features:**
  - Numbers, Booleans, and Lists support.
  - Branching logic (if/else).
  - Looping constructs (e.g., `loop` `break`).
  - Function definitions and calls.
  - Input handling.
  - Output printing.
  - Safe for space tail calls.

**Installation:**

To install the Snek compiler, follow these steps:

1. Clone the repository:

2. Build the compiler:

   ```bash
   cargo build --release
   ```

3. Run the compiler:

   ```bash
   cargo run -- <your-snek-file.snek>
   ```

**Getting Started:**

To get started with using Aron's Snek Language Compiler, create a Snek source file (e.g., `example.snek`) and compile it using the commands mentioned in the installation section.

**Usage Examples:**

Here are some basic examples of Snek code:

```lisp
; Calculate the factorial of a number using recursion
(fun (factorial n)
  (if (< n 2)
      1
      (* n (factorial (- n 1)))))

(print (factorial 5))
```
