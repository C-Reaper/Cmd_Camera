## Overview
The project appears to be a C-based application that captures images from a camera and saves them as JPEG files. It includes support for multiple platforms, including Linux, Windows, Wine, and WebAssembly.

## Features
- Captures images from a camera.
- Saves captured images as JPEG files.
- Supports multiple build targets: Linux, Windows, Wine, and WebAssembly.

## Project Structure
- `build/`: Directory where compiled executables are stored.
- `src/`: Source code directory containing the main entry point file (`Main.c`).
- `Makefile.linux`, `Makefile.windows`, `Makefile.wine`, `Makefile.web`: Makefiles for building on different platforms.

### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools
- Libraries needed in specific projects (JPEG library)

## Build & Run
To build the project:
```sh
cd <Project>
make -f Makefile.(os) all
```

For a clean rebuild:
```sh
make -f Makefile.(os) clean
make -f Makefile.(os) all
```

To execute the built application:
```sh
make -f Makefile.(os) exe
```

### Build Options
- `make -f Makefile.(os) all`: Builds the output executable.
- `make -f Makefile.(os) do`: Builds the output and executes it.
- `make -f Makefile.(os) clean`: Removes build artifacts.