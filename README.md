# Clang Formatting and Tidy Rules

This repository contains configuration files for clang-format and clang-tidy to standardize C and C++ code formatting and static analysis.

## Files

- `.clang-format`: Configuration for clang-format, based on LLVM style with customizations for indentation, braces, etc.
- `.clang-tidy`: Configuration for clang-tidy with a set of enabled checks for static analysis.

## Usage

To use these configurations in your project:

1. Copy `.clang-format` and `.clang-tidy` to your project's root directory.
2. For formatting code with clang-format:
   - Format a single file: `clang-format -i yourfile.cpp`
   - Format all files in a directory: `find . -name "*.cpp" -o -name "*.h" | xargs clang-format -i`
3. For static analysis with clang-tidy:
   - Analyze a single file: `clang-tidy yourfile.cpp -- -I/path/to/includes`
   - For more options, refer to clang-tidy documentation.

These rules are designed for C and C++ projects to maintain consistent code style and catch common issues.
