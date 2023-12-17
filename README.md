# RusticSync 🔁

<img alt="language" src="https://img.shields.io/badge/Lang-Rust-orange.svg"> <img alt="version" src="https://img.shields.io/badge/Version-1.0.0-green.svg">

_RusticSync_ is a file synchronization tool written in Rust that computes and compares file hashes to **identify duplicates** and **synchronize files** across two file systems (local and NAS).

## Features

- Recursively computes SHA-256 hashes for all files in a given directory.
- Detects and reports duplicated files based on their hashes.
- Compares two file systems to identify common files for synchronization.

## Dependencies

- [walkdir](https://crates.io/crates/walkdir): For easy directory traversal.
- [crypto](https://crates.io/crates/crypto): For computing SHA-256 hashes.

## Usage

1. **Build the Project:**

```bash
cargo build --release
```

2. **Launch it!**

```bash
cargo run --release
```

Make sure to replace /path/to/your/directory with the actual path of the directory you want to scan.

3. **View Duplicated Files:**

The program will display duplicated files based on their SHA-256 hashes.

4. **Compare File Systems:**

Adjust the file system paths in the build_file_map function and use the compare_file_systems function to identify common files for synchronization.

## License

This project is licensed under the **MIT License**.

**made by neigebaie, with love 💙❄️**
