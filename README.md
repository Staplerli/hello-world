# Compile.bat Usage Guide

This document provides usage examples and instructions for the `compile.bat` script.

## Overview

`compile.bat` is a Windows batch script designed to compile source code files. This guide demonstrates common usage patterns and examples.

## Basic Usage

### Simple Compilation

To compile a single source file:

```batch
compile.bat source.cpp
```

### Compile with Output Name

To specify a custom output executable name:

```batch
compile.bat source.cpp -o myprogram.exe
```

### Compile Multiple Files

To compile multiple source files:

```batch
compile.bat file1.cpp file2.cpp file3.cpp
```

## Common Examples

### Example 1: Compile C++ Program

```batch
compile.bat main.cpp
```

This will compile `main.cpp` and generate an executable (typically `main.exe`).

### Example 2: Compile with Custom Output

```batch
compile.bat app.cpp -o application.exe
```

This compiles `app.cpp` and creates `application.exe` as the output.

### Example 3: Compile with Debug Symbols

```batch
compile.bat program.cpp -g
```

Compiles with debug information enabled for debugging purposes.

### Example 4: Compile with Optimization

```batch
compile.bat program.cpp -O2
```

Compiles with optimization level 2 for better performance.

### Example 5: Compile Multiple Source Files

```batch
compile.bat main.cpp utils.cpp helper.cpp -o myapp.exe
```

Compiles multiple source files and links them into a single executable.

### Example 6: Compile with Include Directories

```batch
compile.bat source.cpp -I./include -I./libs
```

Compiles with additional include directories specified.

### Example 7: Compile with Library Linking

```batch
compile.bat main.cpp -L./lib -lmylib
```

Compiles and links against a library located in the `./lib` directory.

## Command Line Options

Common options that may be supported:

- `-o <name>` : Specify output executable name
- `-g` : Include debug symbols
- `-O<n>` : Set optimization level (0-3)
- `-I<path>` : Add include directory
- `-L<path>` : Add library directory
- `-l<lib>` : Link against library
- `-c` : Compile only (don't link)
- `-Wall` : Enable all warnings
- `-std=<standard>` : Specify C/C++ standard (e.g., `-std=c++17`)

## Notes

- Ensure you have the necessary compiler installed (e.g., GCC, Clang, MSVC)
- Make sure the compiler is in your system PATH
- Check the script's help message for specific options: `compile.bat --help` or `compile.bat -h`

## Troubleshooting

### Common Issues

1. **Compiler not found**: Ensure your compiler is installed and in PATH
2. **Missing dependencies**: Check that all required libraries are available
3. **Syntax errors**: Review your source code for compilation errors
4. **Permission errors**: Ensure you have write permissions in the output directory

## See Also

For more information about the compiler being used, refer to:
- GCC: `gcc --help`
- Clang: `clang --help`
- MSVC: `cl /?`
