# 📦 Minigrep (Rust🦀)

A lightweight command-line tool written in Rust that searches for a string in a file—similar to a simplified version of grep.

## 🚀 Features

- 🔍 Search for a substring within a file
- ⚡ Fast and efficient (thanks to Rust)
- 🔠 Optional case-insensitive search
- 🧩 Simple and extensible codebase

## 🛠️ Installation

### Prerequisites

Install Rust using rustup

### Clone the repository

```rust
git clone https://github.com/harshd23/minigrep.git
cd minigrep
```

### Build the project

```rust
cargo build --release
```

### ▶️ Usage

```rust
cargo run -- <query> <filename>
```

### Example

```rust
cargo run -- hello sample_text.txt
```

This will print all lines in sample_text.txt that contain the word hello.

### 🔤 Case-Insensitive Search

- Set the environment variable IGNORE_CASE to enable case-insensitive matching.

### Linux / macOS

```rust
IGNORE_CASE=1 cargo run -- hello poem.txt
```

### Windows (PowerShell)

```rust
$env:IGNORE_CASE=1
cargo run -- hello poem.txt
```

## 📁 Project Structure

minigrep/
├── src/
│   ├── main.rs       # Entry point
│   └── lib.rs        # Core logic
├── Cargo.toml        # Project metadata
└── README.md         # Documentation

## 🧠 How It Works

- Parses command-line arguments
- Reads the file contents
- Searches for matching lines
- Prints results to stdout
- Core logic is separated into reusable functions for clarity and testability.

## 🧪 Running Tests

```rust
cargo test
```

## 📚 Learning Goals

This project demonstrates:

- Ownership and borrowing in Rust
- Error handling (Result, unwrap, expect)
- Working with environment variables
- Structuring Rust projects with modules
- Writing testable code

## 🔮 Future Improvements

- Support regex search
- Highlight matched text
- Add recursive directory search
- Improve CLI argument parsing (e.g., using clap)

## 📜 License

This project is licensed under the MIT License.
