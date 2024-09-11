# 🧮 Simple Calculator Web App with C and WebAssembly

## 📚 Overview

This tutorial demonstrates how to create a simple web calculator using C and WebAssembly (WASM). We will use Emscripten to compile C code into WebAssembly, enabling it to run in a web browser. The tutorial covers setting up the environment, writing C code, compiling it to WebAssembly, and creating a simple HTML and JavaScript interface to interact with the compiled code.

## 🚀 Prerequisites

- **Ubuntu with WSL (Windows Subsystem for Linux)**
- **VS Code** with Live Server extension
- Basic knowledge of **C**, **HTML**, and **JavaScript**

## 🛠️ Steps

1. **Install Emscripten**

   Open your VS Code terminal in Ubuntu (WSL) and run:

   ```bash
   sudo apt install emscripten
2. **Clone my repo**
3. **compile**
    ```bash
   "emcc calculator.c -o calculator.html -s EXPORTED_FUNCTIONS='["_add", "_subtract", "_multiply", "_divide"]' -s EXPORTED_RUNTIME_METHODS='["ccall", "cwrap"]'"
  (you may need to recopy my html)
4. **open html with Live Server**
